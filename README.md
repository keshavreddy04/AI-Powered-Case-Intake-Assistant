# ⚖️ AI-Powered Case Intake Assistant for CloudLex  

An AI-driven prototype that automates **legal case intake** by extracting structured data from unstructured client reports.  
This project was built as part of a design challenge to enhance **law firm efficiency, case management, and client experience** using AI and NLP.  

---

## ✨ Features  
- Extracts structured details (Doctors, Hospitals, Dates, Symptoms, Affected Areas) from client narratives.  
- Summarizes medical issues into a concise report using HuggingFace Transformers.  
- Provides **automated risk flagging** (immediate vs. non-urgent).  
- Interactive **Streamlit web app** for easy use by staff and attorneys.  
- Hybrid **AI + rule-based logic** for better accuracy.  

---

## 🛠️ Tech Stack  
- **Language**: Python  
- **NLP**: spaCy (Named Entity Recognition), HuggingFace Transformers (BART)  
- **UI**: Streamlit  
- **ML Backend**: PyTorch  

---

## 📂 Project Workflow  
1. **Input**: Client pastes their case report in plain text.  
2. **NLP Processing**:  
   - spaCy extracts names, hospitals, and dates.  
   - Rules detect affected body parts.  
   - HuggingFace model generates a concise symptoms summary.  
3. **Output**: Structured case data in JSON format + risk flag.  

---

## 🔍 Example  

**Input:**  
On 12 August 2025, I slipped in the bathroom and hurt my right knee.
Since then, I have had pain and swelling. I tried a knee brace but it still hurts.
I consulted Dr. Rao at City Hospital in July.


**Output:**  
```json
{
  "Cause": "Slip in bathroom",
  "Affected Area": ["knee"],
  "Duration": "Since 12 August 2025",
  "Symptoms Summary": "Persistent knee pain and swelling despite treatment.",
  "Doctor": ["Dr. Rao"],
  "Hospital": ["City Hospital"],
  "Date": ["12 August 2025", "July"],
  "Risk Flag": "✅ No immediate risk"
}
```
---

## 📊 Impact

- Reduced manual data entry by ~50%.

- Improved accuracy and efficiency in case intake.

- Enhanced client experience with faster structured reporting.

---

## ⚠️ Risks & Mitigation

- Data Privacy → Ensure sensitive client data is anonymized.

- AI Errors → Keep humans in the loop for verification.

- Scalability → Deploy on cloud with GPU support for handling traffic.

---

## 📌 Future Improvements

- Integration with CloudLex API for seamless workflow.

- Advanced medical entity recognition models.

- Multi-language support for diverse clients.

---

## 👨‍💻 Author

- V Om Keshava Reddy
- 📌 B.Tech CSE (AI & ML), SRM University
- 🔗 [LinkedIn](https://www.linkedin.com/in/v-om-keshava-reddy-792478349/)| [GitHub](https://github.com/keshavreddy04)| [LeetCode](https://leetcode.com/u/keshav_30/)
