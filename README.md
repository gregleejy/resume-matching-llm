# 🏆 AI-Powered Tech Job Resume Matcher

### 🚀 Match your resume to the best tech jobs using AI & NLP!

This project uses **Natural Language Processing (NLP)** and **Deep Learning** to **match tech-related resumes to the most relevant job descriptions** and provide AI-generated suggestions for improvement.

---

## 📌 Features
✔️ **Tech Job Matching** → Uses NLP-based embeddings to find the best-matching **tech job** for a given resume.  
✔️ **AI-Powered Resume Analysis** → Analyzes your resume.  
✔️ **Runs on Google Colab** → No setup needed—just open the Colab notebook and run!  
✔️ **Uses Google Drive** → Model & datasets are stored in **Google Drive** for easy access.

---

## 🛠️ How It Works
1. **Resume Embeddings** → Converts resumes into numerical representations using **Sentence Transformers**.
2. **Job Embeddings** → Converts tech job descriptions into embeddings.
3. **Matching Algorithm** → Uses **cosine similarity** to find the closest matching job description.

---

## 🚀 Running on Google Colab
### **1️⃣ Upload Required Files to Google Drive**
Before running the app, make sure your **trained model and datasets** are stored in **Google Drive** under `My Drive/`. 

## 📁 File Structure (Google Drive + Google Colab)
Ensure your files are **uploaded to Google Drive** in the following structure:

📁 My Drive/ │── 📁 trained_resume_model/ # Trained model directory (stored in Drive) │ │── config.json │ │── tokenizer.json │ │── model.safetensors │── 📄 resumes.csv # Resume dataset │── 📄 job_descriptions.csv # Job descriptions dataset │── 📄 app.ipynb # Google Colab notebook (Gradio app)

---

### **2️⃣ Open & Run the Colab Notebook**
1. **Open Google Colab** → [Google Colab](https://colab.research.google.com/).
2. Upload **`app.ipynb`** to Colab.
3. **Mount Google Drive** when prompted.
4. Run all cells in the notebook.
5. A **Gradio web app** will launch with a public link where you can **paste a resume and get job matching results**.

---

## 📊 Model Training
### **🔹 How I Trained It**
- **Dataset**: Used a dataset of **tech resumes and job descriptions**.
- **Embeddings Model**: `all-MiniLM-L6-v2` for **resume-job similarity**.
- **LLM Fine-Tuning**: Fine-tuned `t5-small` to generate **resume feedback**.

---

## 📌 Future Improvements
🚀 **Expand to Other Job Sectors** (Right now, it’s focused on tech jobs).  
🚀 **Improve Resume Feedback** by fine-tuning a more powerful LLM.  
🚀 **Deploy on Hugging Face for Public Access** (Currently runs only on Google Colab).  

---

## 🤝 Contributing
If you'd like to contribute:
1. **Fork the repository**.
2. **Make your changes**.
3. **Submit a pull request**.

---

## 📜 Acknowledgments
- **Hugging Face Transformers** for NLP models.
- **Sentence Transformers** for embeddings.
- **Google Colab** for training
