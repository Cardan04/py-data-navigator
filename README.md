# py-data-navigator 

O **Data Navigator** é uma ferramenta de automação inteligente desenvolvida em Python que utiliza o modelo **Gemini 2.5 Flash** para analisar capturas de tela de dados (como planilhas do Excel), extrair insights críticos e converter o relatório final em áudio (MP3).

Ideal para acessibilidade e auditoria rápida de dados visuais.

---

##  Funcionalidades

* **Análise de Imagem (Computer Vision):** Identifica tabelas, colunas, status e erros em capturas de tela.
* **Geração de Insights:** O modelo Gemini categoriza o que aparece na tela, destaca informações importantes, aponta problemas (como falhas de licença de software) e sugere melhorias.
* **Acessibilidade (Text-to-Speech):** Utiliza a biblioteca `gTTS` para transformar a análise textual em um arquivo de áudio `resposta.mp3`.
* **Processamento de Linguagem Natural:** Respostas estruturadas em português com foco em tomada de decisão.

---

##  Tecnologias e Ferramentas

* **Linguagem:** Python.
* **Modelo de IA:** Gemini 2.5 Flash (Google AI Studio).
* **Ambiente de Desenvolvimento:** Google Colab Enterprise / Jupyter Notebook.
* **Bibliotecas Principais:**
    * `google-generativeai`: Integração com a API do Gemini.
    * `Pillow (PIL)`: Manipulação e carregamento de imagens.
    * `gTTS (Google Text-to-Speech)`: Conversão de texto para áudio.

---

##  Como Funciona

O fluxo do notebook segue estas etapas:

1.  **Configuração:** Instalação das dependências e autenticação via API Key.
2.  **Input:** Carregamento de uma imagem (ex: `exemplo.png`).
3.  **Processamento:** Envio da imagem + Prompt estruturado para o Gemini 2.5 Flash.
4.  **Output Textual:** Exibição da análise detalhada no console.
5.  **Output Sonoro:** Geração e salvamento do arquivo `resposta.mp3`.

---

##  Pré-requisitos

Antes de rodar o notebook, você precisará de:

* Uma **API KEY** do Google AI Studio.
* Um ambiente Python (local ou Colab).
* As bibliotecas instaladas:

```bash
pip install -q -U google-generativeai gtts pillow
```
prompt = """
Analise essa imagem e gere insights:
1 - O que aparece na tela
2 - Informações importantes
3 - Possíveis problemas
4 - Sugestões
"""

Este projeto foi desenvolvido para fins de estudo e demonstração de capacidades de IA Multimodal.

---

# py-data-navigator 

The **Data Navigator** is an intelligent automation tool developed in Python that uses the **Gemini 2.5 Flash** model to analyze screenshots of data (such as Excel spreadsheets), extract critical insights, and convert the final report into audio (MP3).

Ideal for accessibility and quick auditing of visual data.

---

##  Features

* **Image Analysis (Computer Vision):** Identifies tables, columns, statuses, and errors in screenshots.

* **Insight Generation:** The Gemini model categorizes what appears on the screen, highlights important information, points out problems (such as software license issues), and suggests improvements.

* **Accessibility (Text-to-Speech):** Uses the `gTTS` library to transform the text analysis into an audio file `response.mp3`.

* **Natural Language Processing:** Structured responses in Portuguese focused on decision-making. ---

##  Technologies and Tools

* **Language:** Python.

* **AI Model:** Gemini 2.5 Flash (Google AI Studio).

* **Development Environment:** Google Colab Enterprise / Jupyter Notebook.

* **Main Libraries:**

* `google-generativeai`: Integration with the Gemini API.

* `Pillow (PIL)`: Image manipulation and loading.

* `gTTS (Google Text-to-Speech)`: Text-to-audio conversion.

--

##  How it Works

The notebook flow follows these steps:

1. **Configuration:** Installation of dependencies and authentication via API Key.

2. **Input:** Loading an image (e.g., `example.png`).

3. **Processing:** Sending the image + structured prompt to Gemini 2.5 Flash.

4. **Textual Output:** Displaying the detailed analysis in the console.

5. **Audio Output:** Generating and saving the `response.mp3` file.

---

##  Prerequisites

Before running the notebook, you will need:

* A Google AI Studio **API KEY**.

* A Python environment (local or Colab).

* The following libraries installed:

```bash
pip install -q -U google-generativeai gtts pillow
```
prompt = """
Analyze this image and generate insights:
1 - What appears on the screen
2 - Important information
3 - Possible problems
4 - Suggestions
"""

This project was developed for study and demonstration purposes of Multimodal AI capabilities.
