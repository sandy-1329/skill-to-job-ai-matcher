# Skill-to-Job AI Matcher 💡

An AI-powered system that matches a candidate's resume to the most relevant job descriptions using **SBERT sentence embeddings** and **cosine similarity**. Inspired by real-world platforms like Personio, Delivery Hero, and SAP, this tool helps individuals identify the top jobs they are most qualified for.

---

## 🔎 How It Works

1. **User Uploads Resume (PDF)**
2. **User Uploads Job Descriptions (CSV)**
3. Text is extracted from the resume
4. Descriptions and resume are embedded via **`all-MiniLM-L6-v2`** from `sentence-transformers`
5. Cosine similarity is calculated
6. Jobs are sorted by similarity score
7. Top 5 jobs are printed as match results

---

## 🌐 Demo Output
```
Top 5 Matching Jobs for Your Resume:

 job_title                     company          location        match_score
--------------------------------------------------------------------------
Data Analyst                  Delivery Hero    Berlin, Germany   0.505557
Machine Learning Engineer     Siemens          Munich, Germany   0.501868
Data Scientist                Zalando          Berlin, Germany   0.495130
Business Intelligence Analyst SAP              Walldorf, Germany 0.483455
AI Product Manager            N26              Berlin, Germany   0.443797
```

---

## 📊 Technologies Used

- `sentence-transformers` (SBERT)
- `PyMuPDF` (PDF to text)
- `sklearn.metrics.pairwise.cosine_similarity`
- `pandas`, `numpy`
- Google Colab

---

## 📁 Files

- `Skill_to_Job_Matcher.ipynb` → Main code notebook
- `Cheva_Kavitha_Resume.pdf` → Sample real resume
- `job_descriptions.csv` → Sample job descriptions dataset
- `requirements.txt`
- `Skill_to_Job_AI_Matcher_Report_Venkata.pdf` → 16-page formal report

---

## 🗂️ Use Cases

- Tailor resume to specific job goals
- Job recommender system for HR tech
- Personalized job suggestions
- Interview preparation tool

---

## 🌟 Author

**Venkata Sandeep Kumar Reddy**  
Machine Learning Engineer | AI Project Portfolio Builder  
[GitHub](https://github.com/sandy-1329) | [LinkedIn](https://linkedin.com/in/yourprofile)

---

## ✨ Future Improvements

- UI using Streamlit or Flask
- Add explainability to match score
- Highlight skill gaps vs JD
- Resume tailoring suggestions

---

## 🔗 License

MIT License
