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


# Sample Example 1

```mermaid
graph TD;
    A["Input Text:\n i don't know for real y he's sooo sad"]
    B["Normalized Text:\n i do not know for real why he's so sad"]
    C["Sentiment"]
    
    D["negative: 0.995874803543091"]
    E["neutral: 6.232635259628296e-05"]
    F["positive: 2.0964847564697266e-05"]

    G["Emotion"]
    
    H["anger: 0.0"]
    I["disgust: 0.0"]
    J["fear: 0.010283803842246056"]
    K["joy: 0.0"]
    L["neutral: 0.021935827255129814"]
    M["sadness: 1.0"]
    N["surprise: 0.02158345977962017"]

    A --> B
    A --> C
    C --> D
    C --> E
    C --> F

    D --> G
    E --> G
    F --> G

    G --> H
    G --> I
    G --> J
    G --> K
    G --> L
    G --> M
    G --> N

%% Style the edges from "neutral" and "positive" to "Emotion" with a lighter stroke.
linkStyle 6 stroke:#cccccc, stroke-width:1px;
linkStyle 7 stroke:#cccccc, stroke-width:1px;

```

### Sample Example 2
digraph {
    graph [bgcolor="white", rankdir=TB, splines=true, nodesep=0.8, ranksep=0.8];
    node [shape=box, style="rounded,filled", fontname="Helvetica", fontsize=9, margin="0.15,0.1"];

    Input [label="Input:\nu rlly think all that talk means u tough? lol, when I step up, u ain't gon say sh*t", fillcolor="#ffe6de", fontcolor="black"];
    Output [label="Output:\nyou really think all that talk makes you tough [lol](laughed out loud) when i step up you are not going to say anything", fillcolor="#ffe6de", fontcolor="black"];
    Sentiment [label="Sentiment:\nNEGATIVE", fillcolor="#ecdeff", fontcolor="black"];

    Anger [label="Anger: 0.14403291", fillcolor="#deffe1", fontcolor="black"];
    Disgust [label="Disgust: 0.039282672", fillcolor="#deffe1", fontcolor="black"];
    Fear [label="Fear: 0.014349542", fillcolor="#deffe1", fontcolor="black"];
    Joy [label="Joy: 0.048965044", fillcolor="#deffe1", fontcolor="black"];
    Neutral [label="Neutral: 0.494852662", fillcolor="#deffe1", fontcolor="black"];
    Sadness [label="Sadness: 0.021111647", fillcolor="#deffe1", fontcolor="black"];
    Surprise [label="Surprise: 0.237405464", fillcolor="#deffe1", fontcolor="black"];

    edge [color="#7a7a7a", penwidth=3];

    Input -> Output;
    Input -> Sentiment;
    Sentiment -> Anger;
    Sentiment -> Disgust;
    Sentiment -> Fear;
    Sentiment -> Joy;
    Sentiment ->
::contentReference[oaicite:0]{index=0}
```

