# Clash of Clans Language Model 🏰🧠

[![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Issues](https://img.shields.io/github/issues/YUGESHKARAN/Clash_of_Clans_Language_Model.svg)](https://github.com/YUGESHKARAN/Clash_of_Clans_Language_Model/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/YUGESHKARAN/Clash_of_Clans_Language_Model.svg)](https://github.com/YUGESHKARAN/Clash_of_Clans_Language_Model/pulls)
[![Stars](https://img.shields.io/github/stars/YUGESHKARAN/Clash_of_Clans_Language_Model.svg)](https://github.com/YUGESHKARAN/Clash_of_Clans_Language_Model/stargazers)
[![Forks](https://img.shields.io/github/forks/YUGESHKARAN/Clash_of_Clans_Language_Model.svg)](https://github.com/YUGESHKARAN/Clash_of_Clans_Language_Model/network)

---

A mini language model built from scratch using **PyTorch**, fine-tuned on a supervised custom Clash of Clans dataset (`clash_finetune_chat_700.jsonl`).  
The model contains **~2.96 million** trainable parameters and is designed for NLP tasks related to Clash of Clans heroes, defenses, and troops.

---

## 🚀 Features

- **From-Scratch Implementation:** PyTorch-based, no external LLM dependencies.
- **Custom Dataset:** Fine-tuned on Clash of Clans-specific data.
- **Jupyter Notebooks:** Easy exploration and experimentation.
- **Lightweight:** Only 2.96M parameters—perfect for education and experimentation.

## 📦 Prerequisites

- 🐍 Python **3.8+**
- 📓 Jupyter Notebook
- 💡 (Recommended) `virtualenv` or `conda` for environment management

## ⚡ Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/YUGESHKARAN/Clash_of_Clans_Language_Model.git
   cd Clash_of_Clans_Language_Model
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   # Or, for conda users:
   # conda env create -f environment.yml
   ```

## 📁 Project Structure

```plaintext
Clash_of_Clans_Language_Model/
├── clash_finetune_chat_700.jsonl      # Custom supervised dataset
├── index.py                           # Model code (training and inference)
├── requirements.txt                   # Python dependencies
├──language_model_class.py             # model architecture and hyperparameters
├──clash_transformer_finetuned.pth     # model pretrained weights
├──tokenizer.pkl                       # pre-saved tokenizer map (dictionary)
└── README.md                          # Project documentation
```

## ⚙️ Model Hyperparameters

- `batch_size`: 64
- `block_size`: 256
- `n_embed`: 256
- `n_heads`: 8
- `n_layer`: 6
- `learning_rate`: 1e-4
- `max_iters`: 3000
- `eval_interval`: 100

## 🤝 Contributing

Contributions are welcome! Please open issues or pull requests for suggestions, bug fixes, or improvements.

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- **Supercell** – for Clash of Clans inspiration
- The open-source ML & NLP communities
- Special thanks to **Andrej Karpathy** for his [GPT-2 reproduction lecture](https://www.youtube.com/watch?v=kCc8FmEb1nY)

---

> _This project is not affiliated with or endorsed by Supercell. For educational and research purposes only._
