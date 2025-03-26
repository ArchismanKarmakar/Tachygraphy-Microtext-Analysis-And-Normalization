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
graph LR;
    %% Input and normalized text nodes
    A["Input Text: i don't know for real y he's sooo sad"]
    B["Normalized Text: i do not know for real why he's so sad"]
    C["Sentiment"]

    A --> B
    A -->|Sentiment| C

    %% Sentiment value nodes (values inside the boxes)
    C -->|Negative| D["0.99587"]
    C -->|Neutral| E["6.23e-05"]
    C -->|Positive| F["2.10e-05"]

    %% Converge sentiment nodes to Emotion stage
    D -->|Emotion| G
    E -->|Emotion| G
    F -->|Emotion| G

    %% Emotion nodes: arrow labels show emotion category; node boxes show numeric values.
    G -->|Anger| H["0.0"]
    G -->|Disgust| I["0.0"]
    G -->|Fear| J["0.01028"]
    G -->|Joy| K["0.0"]
    G -->|Neutral| L["0.02194"]
    G -->|Sadness| M["1.0"]
    G -->|Surprise| N["0.02158"]

%% Style the Neutral and Positive sentiment arrows with a lighter stroke.
linkStyle 2 stroke:#cccccc, stroke-width:1px;
linkStyle 3 stroke:#cccccc, stroke-width:1px;

```

### Sample Example 2
```mermaid
graph TD;
    %% Input and normalized text nodes
    A["Input Text: you rlly think all that talk means u tough? lol, when I step up, u ain't gon say sh*t"]
    B["Normalized Text: you really think all that talk makes you tough [lol](laughed out loud) when i step up you are not going to say anything"]
    C["Sentiment"]

    A --> B
    A -->|Sentiment| C

    %% Sentiment value nodes
    C -->|Negative| D["0.99999"]
    C -->|Neutral| E["6.89e-06"]
    C -->|Positive| F["1.11e-05"]

    %% Converge sentiment nodes to Emotion stage
    D -->|Emotion| G
    E -->|Emotion| G
    F -->|Emotion| G

    %% Emotion nodes: arrow labels show emotion category; nodes show numeric values.
    G -->|Anger| H["0.14403"]
    G -->|Disgust| I["0.03928"]
    G -->|Fear| J["0.01435"]
    G -->|Joy| K["0.04897"]
    G -->|Neutral| L["0.49485"]
    G -->|Sadness| M["0.02111"]
    G -->|Surprise| N["0.23741"]

%% Style the Neutral and Positive sentiment arrows with a lighter stroke.
linkStyle 2 stroke:#cccccc, stroke-width:1px;
linkStyle 3 stroke:#cccccc, stroke-width:1px;
```

### Sample Example 3
```mermaid
graph TD;
    %% Input and normalized text
    A["Input Text: i don't know for real y he's sooo sad"]
    B["Normalized Text: i do not know for real why he's so sad"]

    %% Sentiment stage
    C["Sentiment"]
    
    A --> B
    A --> C

    %% Sentiment value nodes with values inside the box;
    %% The arrow labels carry the category names.
    C -->|Negative| D["4.43e-05"]
    C -->|Neutral| E["0.9999"]
    C -->|Positive| F["7.09e-05"]

    %% All sentiment nodes feed into the Emotion stage.
    D -->|Emotion| G
    E -->|Emotion| G
    F -->|Emotion| G

    %% Emotion stage: arrows label the emotion category, nodes contain the numeric value.
    G -->|Anger| H["0.0801"]
    G -->|Disgust| I["0.0152"]
    G -->|Fear| J["0.0103"]
    G -->|Joy| K["0.0"]
    G -->|Neutral| L["0.0219"]
    G -->|Sadness| M["1.0"]
    G -->|Surprise| N["0.0216"]

%% Style the edges for lower-probability sentiment arrows with a lighter stroke
%% (Assuming the second and third edges from C are "Neutral" and "Positive")
linkStyle 2 stroke:#cccccc, stroke-width:1px;
linkStyle 3 stroke:#cccccc, stroke-width:1px;



```

