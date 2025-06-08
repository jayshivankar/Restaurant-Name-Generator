# 🍽️ Restaurant Name Generator

A fun and simple Streamlit app that generates creative restaurant names and menu items based on your selected cuisine using the power of LangChain and LLMs!


## 🛠️ Features

- Easy-to-use Streamlit UI
- Dynamic name and menu generation
- Supports 5 cuisines: Indian, Italian, Mexican, Arabic, American
- Powered by [LangChain](https://github.com/langchain-ai/langchain) and an LLM backend

## 📂 Project Structure

```
restaurant-name-generator/
├── main.py                  # Streamlit frontend
├── langchain_helper.py      # LangChain logic for generating names & items
├── requirements.txt          # Required dependencies
└── README.md                # Project documentation
```

## 📦 Requirements

- Python 3.8+
- Streamlit
- LangChain
- OpenAI (or any LLM provider integrated in `langchain_helper.py`)

Install dependencies with:

```bash
pip install -r requirements.txt
```

## ▶️ How to Run

```bash
streamlit run main.py
```

## 🧠 Behind the Scenes

The function `generate_restaurant_name_and_items(cuisine)` in `langchain_helper.py` queries a language model with a prompt based on the selected cuisine. The model responds with a creative restaurant name and a comma-separated list of menu items.

> Make sure to add your API key and configuration in `langchain_helper.py` for the LLM to work correctly.

## 📌 To Do

- Add more cuisines
- Include restaurant descriptions or themes
- Enable user-specified cuisine or fusion styles
- Add LLM parameter tuning options

