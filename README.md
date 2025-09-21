# Applicant Screening Workflow

This project is a small experiment to automate the first round of applicant screening using LangGraph and Groq LLM.

The workflow is as follows:

1. **Categorize Experience**  
   The model looks at the application text and decides whether the candidate is *Entry-level*, *Mid-level*, or *Senior-level*.

2. **Assess Skillset**  
   The model then checks if the candidate’s skills match a Python Developer role. It responds with either **"Match"** or **"No Match"**.

3. **Route the Application**  
   Based on the two results:
   - If the skills match → the candidate is shortlisted for an **HR interview**.  
   - If the candidate is senior but skills don’t match → the case is **escalated to a recruiter**.  
   - Otherwise → the application is **rejected**.


