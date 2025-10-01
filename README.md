# Automated Image Captioning Tool

This project implements an **AI-powered image captioning tool** using the **BLIP (Bootstrapping Language-Image Pretraining)** model from Hugging Face.  
It can automatically generate meaningful captions for images found on a webpage, saving them into a text file for review and use.  

---

##  Features
- **Automated Webpage Captioning**: Scrapes all `<img>` tags from a webpage, downloads the images, and generates captions.
- **BLIP Model**: Uses Hugging Face’s pretrained BLIP model for high-quality captions.
- **SEO & Accessibility Benefits**:
  - Generates **alt text** for images → improves accessibility for visually impaired users.
  - Enhances SEO ranking by including descriptive captions in articles.
- **Business Use Case (News/Media)**:
  - Journalists no longer need to manually caption hundreds of images.
  - AI-generated captions speed up publishing, improve content reach, and save time.

---

##  Architecture

flowchart TD
    A[Webpage URL] --> B[Requests + BeautifulSoup]
    B --> C[Image URLs Extracted]
    C --> D[BLIP Processor + Model]
    D --> E[Caption Generated]
    E --> F[Captions.txt Output]

---

##  Getting Started

1. Clone the repo
git clone https://github.com/Sanjayyellina/automated-image-captioning.git
cd automated-image-captioning
2. Create a virtual environment
python3 -m venv my_env
source my_env/bin/activate
3. Install dependencies
pip install -r requirements.txt
4. Run the script
python3 automate_url_captioner.py

---

##  Output
Captions are written into captions.txt.
Example snippet:
https://upload.wikimedia.org/wikipedia/commons/c/c9/IBM_Research_Almaden.jpg: a modern glass office building
https://upload.wikimedia.org/wikipedia/commons/5/51/Thomas_J._Watson.jpg: a portrait of a man in a suit

---

## Tech Stack
Python 3
Transformers (Hugging Face) — BLIP model for captioning
Requests — HTTP requests
BeautifulSoup (bs4) — HTML parsing
PIL (Pillow) — Image processing

---

##  Why this project is impressive
Shows practical application of Vision + Language AI.
Connects AI with real-world business needs (news/media SEO + accessibility).
Integrates modern AI libraries: Transformers, BLIP, BeautifulSoup.
Portfolio-ready: demonstrates your ability to build end-to-end AI solutions beyond just chatbots.

---

## Author
Abhinav Sanja (sanjayyellina)
Graduate Student · Business Analytics / Computer Science ·  Generative AI & Cybersecurity Enthusiast
