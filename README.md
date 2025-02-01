# 🏆 AI-Powered Tech Job Resume Analyzer  

### 🚀 Get AI-generated job matches & resume summaries instantly!  

This project leverages **Natural Language Processing (NLP)** and **Deep Learning** to:  
✅ **Analyze a given resume** and generate a **concise summary** of its contents.  
✅ **Match the resume to the most relevant tech job** based on skill alignment.  

---

## 📌 Features  
✔️ **AI-Powered Resume Analysis** → Generates a summary that highlights key skills, experience, and expertise.  
✔️ **Tech Job Matching** → Uses NLP-based embeddings to suggest the **best-matching tech job**.  
✔️ **Runs on Google Colab** → No setup required—just open the notebook and run!  
✔️ **Google Drive Integration** → Model & datasets are stored in **Google Drive** for easy access.  

---

## 🛠️ How It Works  
1. **Resume Embeddings** → Converts resumes into numerical representations using **Sentence Transformers**.  
2. **Resume Summarization** → Uses `bart-large-cnn` to generate a concise summary.  
3. **Job Matching** → Compares resume embeddings to job descriptions via **cosine similarity** and suggests the best fit.  

---

## 🚀 Running on Google Colab  

### **1️⃣ Upload Required Files to Google Drive**  

## 📁 File Structure (Google Drive + Google Colab)  
Ensure your files are **uploaded to Google Drive** in the following structure:  

- **My Drive/**
  - **trained_resume_model/** (Trained model directory)
    - `config.json`
    - `tokenizer.json`
    - `model.safetensors`
  - `resumes.csv` (Resume dataset)
  - `job_descriptions.csv` (Job descriptions dataset)
  - `deploy_model.ipynb` (Google Colab notebook)

---

## 📁 GitHub Repository Structure
Your **GitHub repository** should be structured as follows:

- **resume-matching-LLM/**
  - `train_model.ipynb` (Notebook for training the model)
  - `deploy_model.ipynb` (Google Colab notebook for running the app)
  - `README.md` (Project documentation)
  - `requirements.txt` (Dependencies for Colab)
  - `.gitignore` (Ignore unnecessary files)

---

### **2️⃣ Open & Run the Colab Notebook**  
1. **Open Google Colab** → [Google Colab](https://colab.research.google.com/).  
2. Upload **`app.ipynb`** to Colab.  
3. **Mount Google Drive** when prompted.  
4. Run all cells in the notebook.  
5. A **Gradio web app** will launch with a public link where you can **paste a resume and get job matching results + a summary**.  

---

## 📊 Model Training  

### **🔹 How I Trained It**  
- **Dataset**: Used a dataset of **tech resumes and job descriptions**.  
- **Embeddings Model**: `all-MiniLM-L6-v2` for **resume-job similarity**.  
- **LLM for Summarization**: Used `bart-large-cnn` to generate **resume summaries**.  

---

## 📌 Future Improvements  
🚀 **Expand to Other Job Sectors** (Right now, it’s focused on tech jobs).  
🚀 **Enhance Resume Feedback** by fine-tuning a more powerful LLM.  
🚀 **Deploy on Hugging Face for Public Access** (Currently runs only on Google Colab).  

---

## 🤝 Contributing  
If you'd like to contribute:  
1. **Fork the repository**.  
2. **Make your changes**.  
3. **Submit a pull request**.  

---

##
