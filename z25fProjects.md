---
layout: page
title: ProjectGuide
desc: "Final Project Information for 2025 Fall UVa CS -ML-Undergraduate"
---



## Detailed requirements on Final Project and required artifacts: 

+ Each team includes up to three students.
+ The final project should be technical, employing methods including, but not limited to, those covered in class (e.g., identify a real-world problem and apply relevant algorithms learned). Please keep your code and visualized results in Jupyter notebooks or well-organized code structure. Teams with multiple students may divide experiments across several notebooks. Each team is also required to present their project detailing the project's background (motivation), methodology, and results.

+ On what to create / submit for your final project: 
  - 1. A mini demo "Shark Tank" presentation to the instructors on your project idea is expected. The mini presentation is expected to explain  (WHY/ WHAT/ HOW on your project!) -- intended to be a more conceptual, idea-based pitch; please use [a given template]({{ site.baseurl }}/Lectures/ProjPresentationTemplate-1.pptx) to help you pitch the idea! 
  - 2. A slide deck (Due in Canvas on xx ) summarizing your project  and describing the results you reproduce; Filling in the template slide pages will be enough enough (more is better!). Here is the [given template]({{ site.baseurl }}/Lectures/ProjPresentationTemplate-1.pptx)
  - 3. A python Jupyter notebook (Due in Canvas on Xxx, together with the slide deck) to present the code, data visualization, and obtain the results and analysis through step by step code cell run. 
  - On the final project day, you are expected to present a formal / complete demo using your slide deck and your code demo during the project poster session. 
  - You are expected to go through and show the notebook file and your final project presentation to the instructors via a team video demo. 
  
+ What to submit as the final artifacts of your project: 
    1. your project iPython Notebook and you cell run it in the demo video (TA will host a course project Github, you are expected to PullRequest to add yours into this Github)
    2. To minimize the overhead time cost (switching, wrong setup, ….), we will expect you to record a demo video to present your project / We recommend you to submit your video demo to youtube and share the link in the Canvas project submission. (Please practice the whole process for a few times before you make video demos.) 
    3. your project slide deck as your final report into Canvas (the slide deck is required to have your video links and your git-PR information)

+ On how we grade the projects: 
  - Here is the grading rubrics we will use to grade your final report 
  - Good slide deck (aka also via final presentation ) (60%)
    1. Clear definition of problem and importance (10%)
    2. Clear explanation of approach and code runs (15%)
    3. clear summary of results (and/or difficulties) (15%)
    4. Well-organized, polished as a whole (10%) 
    5. Great delivery of content at the final demo session and the "shark tank" sessions (10%)
  - Good coding artifacts (aka also via final presentation) (40%)
  - Good video demo (Extra credits: 20%)


## Each week, Prof.Qi share one idea on potential projects or project domain: for example, 

<hr>

#### Week2 Idea: 
- [Working with AI: Measuring the Occupational Implications of Generative AI](https://arxiv.org/abs/2507.07935)
- Summary: Given the rapid adoption of generative AI and its potential to impact a wide range of tasks, understanding the effects of AI on the economy is one of society's most important questions. In this work, we take a step toward that goal by analyzing the work activities people do with AI, how successfully and broadly those activities are done, and combine that with data on what occupations do those activities. We analyze a dataset of 200k anonymized and privacy-scrubbed conversations between users and Microsoft Bing Copilot, a publicly available generative AI system. We find the most common work activities people seek AI assistance for involve gathering information and writing, while the most common activities that AI itself is performing are providing information and assistance, writing, teaching, and advising. Combining these activity classifications with measurements of task success and scope of impact, we compute an AI applicability score for each occupation. We find the highest AI applicability scores for knowledge work occupation groups such as computer and mathematical, and office and administrative support, as well as occupations such as sales whose work activities involve providing and communicating information. Additionally, we characterize the types of work activities performed most successfully, how wage and education correlate with AI applicability, and how real-world usage compares to predictions of occupational AI impact.



<hr>

#### Week4 Project ideas: 

- Machine Learning at UVA ([ML@UVA](https://mlatuva.org/)), the university's leading machine learning club with 300+ members and faculty advisors. We collaborate with UVA departments, research labs, and industry partners to tackle real-world challenges through data-driven innovation.  

- This year, they are collaborating on joint projects with Logistics Management Institute (LMI) and Johns Hopkins APL. Since your course covers machine learning fundamentals and AI techniques, and we are pursuing projects in neural networks, computer vision, graph analysis, and anomaly detection



<hr>


#### Week6 : [Claude Builder Club](https://docs.google.com/presentation/d/1MBfwvX18LSz7pkR4hv2k-bJ44JnUKlO0wB3UG0bAFBw/edit?slide=id.g378ece762da_0_699#slide=id.g378ece762da_0_699)   


- Pierce Brookins email is byd5ur@virginia.edu  if you have any questions
- Resume Book: https://forms.gle/Uo453kf9KAWG2oYN6
- Member Form: https://forms.gle/A96i6mNNoQ58zAEK9



<hr> 

#### Week 8 Tutorial: [Huggingface](https://huggingface.co/docs)
- tutorial slide deck: [TA's slide deck](https://qiyanjun.github.io/2025Fall-UVA-CS-MachineLearningDeep//contents/S2-L20-invite-hugginface/)
- a tutorial on huggingface model zoo and platform ---The  best platform where the machine learning community collaborates on models, datasets, and applications.


<hr>

#### Week 8 Extra readings to help your project ideas: 
- <a href="https://github.com/qiyanjun/2025Fall-UVA-CS-MachineLearningDeep/blob/main/Lectures/S3-25recentLLM-extra.pdf"> [Recent LLM-survey] </a> 
- <a href="https://github.com/qiyanjun/2025Fall-UVA-CS-MachineLearningDeep/blob/main/Lectures/S3-deepNNSurvey.pdf"> [A survey of 10 advanced DNN topics] </a>  


<hr> 

#### Week 9 to Week 14: Project "Shark Tank"

- The instructor team is hosting the "Shark Tank" Sessions to screen your project ideas! 
- Plese select your session in the signup sheet! 


### Potential project ideas: 


## 1. Machine Learning (ML) Project Ideas

### 1.1 ML for Fraud and Risk Detection (Finance & Cybersecurity)

- **Problem:** Detect fraudulent or risky transactions or behaviors.
- **Application:** Build an interpretable ML classifier (e.g., **XGBoost**, **LightGBM**, **AutoGluon**) for credit card fraud, insurance claim anomalies, or phishing detection.
- **Data:** [Credit Card Fraud Detection (Kaggle)](https://www.kaggle.com/mlg-ulb/creditcardfraud), [IEEE-CIS Fraud Detection](https://www.kaggle.com/c/ieee-fraud-detection).
- **Extension (2025 trend):** Incorporate **explainable AI (SHAP, LIME)** for financial regulators' interpretability requirements.

### 1.2 ML for Predictive Maintenance (Industry 4.0)

- **Problem:** Predict machine or component failure using sensor data.
- **Application:** Develop a **time-series forecasting** model (e.g., **Temporal Fusion Transformer**, **Prophet**, **LSTM**) to schedule maintenance.
- **Data:** [NASA Turbofan Engine Degradation dataset](https://ti.arc.nasa.gov/tech/dash/groups/pcoe/prognostic-data-repository/).
- **Extension:** Add **anomaly detection** using **autoencoders or isolation forests** for early-warning alerts.

### 1.3 ML for Smart Healthcare Analytics

- **Problem:** Predict patient outcomes, readmissions, or disease risk from tabular and text data.
- **Application:** Build ML pipelines integrating **structured EHR + clinical notes** with feature engineering.
- **Data:** [MIMIC-IV dataset](https://physionet.org/content/mimiciv/).
- **Extension:** Include **fairness analysis** or **privacy-preserving ML (DP, federated learning)**.

### 1.4 ML for Recommendation and Personalization

- **Problem:** Personalized content recommendations.
- **Application:** Implement **hybrid recommenders** combining **collaborative filtering + transformer encoders (BERT4Rec, SASRec)**.
- **Data:** [MovieLens](https://grouplens.org/datasets/movielens/), [Amazon Product Data](https://jmcauley.ucsd.edu/data/amazon/).
- **Extension:** Integrate **LLM-based retrieval-augmented ranking** (e.g., use OpenAI or Gemini embeddings).

## 2. Deep Learning (DL) Project Ideas

### 2.1 DL for Medical Imaging (Vision + Health)

- **Problem:** Disease detection from X-ray, MRI, or histopathology images.
- **Application:** Use **Vision Transformers (ViT)** or **CNNs (EfficientNet, ResNet-50)** for classification or segmentation.
- **Data Example:** [RSNA Pneumonia Detection Challenge](https://www.kaggle.com/c/rsna-pneumonia-detection-challenge), [BRATS 2021 MRI dataset](https://www.med.upenn.edu/cbica/brats2021/).
- **Extension:** Use **Grad-CAM or Segment Anything (SAM)** for explainable medical segmentation.

### 2.2 DL for NLP (Transformer-based Sentiment & Topic Analysis)

- **Problem:** Understanding opinions, toxicity, or stance in text.
- **Application:** Fine-tune **Llama-3, Mistral, or DistilBERT** for sentiment or stance detection.
- **Data Example:** [IMDb Reviews](https://ai.stanford.edu/~amaas/data/sentiment/), [TweetEval](https://github.com/cardiffnlp/tweeteval).
- **Extension:** Compare **zero-shot** vs **fine-tuned LLM** performance using OpenAI or Claude APIs.

### 2.3 Multimodal Deep Learning (Vision + Text)

- **Problem:** Align visual and textual information for classification or retrieval.
- **Application:** Train a **CLIP-like model** or fine-tune **OpenCLIP** on custom domain (e.g., art, products, medical).
- **Data:** [Flickr30k](https://shannon.cs.illinois.edu/DenotationGraph/), [LAION-400M/5B](https://laion.ai/blog/laion-5b/).
- **Extension:** Apply **Contrastive Learning** + **cross-attention fusion** modules for task-specific adaptation.

## 3. Generative AI (GenAI) Project Ideas

### 3.1 GenAI for Creative Media (Text, Image, Music, Video)

- **Problem:** Generate creative or branded content automatically.
- **Applications:**
  - **Text:** Story or blog generation with **GPT-4o or Claude 3.5** fine-tuned via OpenAI's fine-tuning API.
  - **Image:** **Stable Diffusion XL**, **DALL·E 3**, or **Ideogram** for text-to-image.
  - **Music:** Use **MusicLM**, **Suno**, or **Mubert API** for audio generation.
  - **Video:** Explore **OpenAI Sora (text-to-video)** or **Runway Gen-3 Alpha** for cinematic short clips.
- **Data:** Creative commons datasets (e.g., COCO Captions, LAION-Aesthetics, MusicCaps).

### 3.2 GenAI for Data Augmentation and Simulation

- **Problem:** Improve ML robustness with synthetic data in low-data regimes.
- **Application:** Use **Diffusion models** or **tabular GANs (CTGAN, TVAE)** to generate synthetic examples.
- **Data:** Any small real dataset (medical, fraud, sensor).
- **Extension:** Evaluate using **TSTR/TSTS metrics** and **privacy leakage testing**.

### 3.3 GenAI for Explainable AI (LLMs as Explainers)

- **Problem:** Explain model predictions and surface reasoning traces.
- **Application:** Build an **LLM-based explainer agent** that interprets model outputs using Chain-of-Thought prompting.
- **Tools:** OpenAI function calling, LangChain, or LlamaIndex integration.

## 4. AI Agent and Systems Project Ideas

### 4.1 AI Agents for Information Retrieval or Research Assistants

- **Problem:** Automate retrieval, summarization, and reasoning over long documents.
- **Application:** Build a **Retrieval-Augmented Generation (RAG)** agent using **LangChain**, **LlamaIndex**, and **Qdrant/FAISS** vector stores.
- **Extension:** Add **multi-agent debate** (via **AutoGen**, **CrewAI**, or **OpenDevin**) to improve factual accuracy.

### 4.2 Simulation Agents for Cybersecurity or Finance

- **Problem:** Model adversarial or autonomous agent behavior (e.g., attacker vs defender).
- **Application:** Create **red-team vs blue-team agents** to simulate phishing or intrusion responses using **AutoGen** or **SuperAGI**.
- **Extension:** Integrate **policy engine (Cedar / Guardrails)** for enforcing compliance and ethical constraints.

### 4.3 Personal Productivity or Education Agent

- **Problem:** Build an AI tutor, assistant, or planner that interacts naturally with users.
- **Application:** Combine **speech recognition (Whisper)**, **LLMs (GPT-4o / Claude)**, and **tool-use frameworks (LangGraph)**.
- **Extension:** Add **memory and scheduling** via vector databases and gcal integration.

## Potential Tools & Frameworks you may explore/learn for team Projects

### For ML & DL

- **Scikit-learn** – easy ML modeling and evaluation.
- **PyTorch Lightning / TensorFlow Keras** – structured DL training.
- **Hugging Face Transformers** – for NLP and vision transformers.
- **Weights & Biases** – for experiment tracking and visualization.
- **Streamlit / Gradio** – for building interactive demos.

### For GenAI & Agent Projects

| Tool | Description |
|------|-------------|
| **OpenAI GPT-4o / GPT-4o-mini** | Free-tier LLM access via ChatGPT or API for text, image, and code. |
| **Claude 3.5 Sonnet (Anthropic)** | Strong at summarization and reasoning. |
| **Google Gemini 1.5** | Integrates text + image + code tasks. |
| **LangChain** | Framework for building LLM workflows. |
| **LlamaIndex** | Simplifies data ingestion and RAG for custom knowledge. |
| **Gradio** | Quick web app demos for ML models. |
| **GitHub Copilot / CodeWhisperer** | AI coding partners for faster development. |


### Many many more! 


#### Looking forward to your demos and artifacts! 
