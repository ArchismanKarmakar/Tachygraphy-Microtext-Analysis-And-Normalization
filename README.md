# Tachygraphy Micro-text Analysis And Normalization
<!---
---
title: "Tachygraphy Micro-text Analysis & Normalization"
emoji: "⚡"
colorFrom: "pink"
colorTo: "blue"
sdk: "static"
pinned: false
---
--->

<!-- ---
title: README
emoji: 😻
colorFrom: yellow
colorTo: red
sdk: static
pinned: false
---
 -->
 
<div align="center">
  
<!-- ![Project Logo](https://via.placeholder.com/150) -->

# Tachygraphy Micro-text Analysis & Normalization

*Welcome to the Tachygraphy Micro-text Analysis & Normalization Project. This page outlines our project’s key stages, sources, sample analysis examples, and team information.*

</div>

---

## Dashboard

### Project Stages

1. **Sentiment Polarity Analysis**
2. **Emotion Mood-tag Analysis**
3. **Text Transformation & Normalization**
4. **Stacked all 3 stages with their best models**
5. **Data Correction & Collection**

### Sources & Deployment Links

| **Training Source** | **Kaggle Collections** | **Hugging Face Org** |
| ------------------- | ---------------------- | -------------------- |
| [GitHub @ Tachygraphy Micro-text Analysis & Normalization](https://github.com/ArchismanKarmakar/Tachygraphy-Microtext-Analysis-And-Normalization) | [Kaggle Dataset](https://www.kaggle.com/datasets/archismancoder/dataset-tachygraphy/data?select=Tachygraphy_MicroText-AIO-V3.xlsx) | [Hugging Face @ Tachygraphy Micro-text Normalization](https://huggingface.co/Tachygraphy-Microtext-Normalization-IEMK25) |

| **Deployment Source** | **Streamlit Deployment** | **Hugging Face Space Deployment** |
| --------------------- | ------------------------ | --------------------------------- |
| [GitHub Deployment Repo](https://github.com/ArchismanKarmakar/Tachygraphy-Microtext-Analysis-And-Normalization-Deployment-Source-HuggingFace_Streamlit_JPX14032025) | [Streamlit App](https://tachygraphy-microtext.streamlit.app/) | [Hugging Face Space](https://huggingface.co/spaces/Tachygraphy-Microtext-Normalization-IEMK25/Tachygraphy-Microtext-Analysis-and-Normalization-ArchismanCoder) |

---

## Project Overview

Tachygraphy—originally developed to expedite writing—has evolved over centuries. In the 1990s, it reappeared as micro‑text, driving faster communication on social media with its “Anytime, Anyplace, Anybody, and Anything (4A)” characteristic. This project focuses on the analysis and normalization of micro‑text (the prevalent informal communication today) to improve NLP tasks such as sentiment analysis, emotion detection, and overall text transformation for clear 4A message decoding.

---

## Sample Examples

### Sample Example 1

Below is a Graphviz diagram illustrating a sample analysis:


### Sample Example 1

```mermaid
graph TD;
    A["Input Text: i don't know for real y he's sooo sad"]
    B["Normalized Text: i do not know for real why he's so sad"]
    C["Sentiment"]
    G["Emotion"]

    A --> B
    A --> C

    C -- "Negative: 0.9959" --> G
    C -- "Neutral: 6.23e-05" --> G
    C -- "Positive: 2.10e-05" --> G

    G -- "Anger" --> H["0.0"]
    G -- "Disgust" --> I["0.0"]
    G -- "Fear" --> J["0.0103"]
    G -- "Joy" --> K["0.0"]
    G -- "Neutral" --> L["0.0219"]
    G -- "Sadness" --> M["1.0"]
    G -- "Surprise" --> N["0.0216"]

%% Style the edges from "Neutral" and "Positive" to "Emotion" with a lighter stroke.
linkStyle 1 stroke:#cccccc, stroke-width:1px;
linkStyle 2 stroke:#cccccc, stroke-width:1px;



```

### Sample Example 2
```mermaid
graph TD;
    A["Input Text: you rlly think all that talk means u tough? lol, when I step up, u ain't gon say sh*t"]
    B["Normalized Text: you really think all that talk makes you tough [lol](laughed out loud) when i step up you are not going to say anything"]
    C["Sentiment"]
    G["Emotion"]

    A --> B
    A --> C

    C -->|"Negative: 0.99999"| G
    C -->|"Neutral: 6.88e-06"| G
    C -->|"Positive: 1.11e-05"| G

    G -->|"Anger"| H["0.144"]
    G -->|"Disgust"| I["0.039"]
    G -->|"Fear"| J["0.014"]
    G -->|"Joy"| K["0.048"]
    G -->|"Neutral"| L["0.494"]
    G -->|"Sadness"| M["0.021"]
    G -->|"Surprise"| N["0.237"]

%% Style the edges from "Neutral" and "Positive" to "Emotion" with a lighter stroke
linkStyle 2 stroke:#cccccc, stroke-width:1px;
linkStyle 3 stroke:#cccccc, stroke-width:1px;



```

### Sample Example 3
```mermaid
graph TD;
    A["Input Text: bruh, floods in Kerala, rescue ops non‑stop 🚁"]
    B["Normalized Text: Brother, the floods in Kerala are severe, and rescue operations are ongoing continuously."]
    C["Sentiment"]
    G["Emotion"]

    A --> B
    A --> C

    C -->|Negative: 4.43e-05| G
    C -->|Neutral: 0.9999| G
    C -->|Positive: 7.09e-05| G

    G -->|Anger| H["0.0801"]
    G -->|Disgust| I["0.0152"]
    G -->|Fear| J["0.0103"]
    G -->|Joy| K["0.0"]
    G -->|Neutral| L["0.0219"]
    G -->|Sadness| M["1.0"]
    G -->|Surprise| N["0.0216"]

%% Style the edges from "Neutral" and "Positive" to "Emotion" with a lighter stroke
linkStyle 2 stroke:#cccccc, stroke-width:1px;
linkStyle 3 stroke:#cccccc, stroke-width:1px;


```

