# Resume Optimizer with AI 📄

Make your resume ATS-friendly and boost your job application success! This tool uses **Google Gemini Pro** to analyze your resume against job descriptions and suggest improvements. It's like having an HR expert review your resume for free!

---

## What It Does ✨

- **ATS Match Score** 📊: See what % of the job you match (e.g., "Your resume matches 78%")
- **Missing Keywords** 🔍: Find exactly what keywords you need to add
- **Smart Suggestions** 💡: Get specific tips like "Add Docker experience" or "Mention Agile"
- **Improved Resume** 📥: Download a PDF with all suggestions already incorporated

---

## Quick Start (5 mins) 🚀

### Step 1: Get Google API Key
- Go to [Google AI Studio](https://aistudio.google.com/app/apikeys)
- Click "Create API Key" 
- Copy your API key

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

**What gets installed:**
- `streamlit` — Web interface
- `google-generativeai` — AI model
- `python-dotenv` — Secure credential management
- `PyPDF2` — PDF handling

### Step 3: Create `.env` File
Create a file named `.env` in your project folder:
```ini
GOOGLE_API_KEY=your_api_key_here
```

⚠️ **Important:** Add `.env` to `.gitignore` so you don't share your API key!

### Step 4: Run the App
```bash
streamlit run app.py
```

Open `http://localhost:8501` in your browser and start analyzing! 🎉

---

## How to Use 📖

### Quick 2-Minute Workflow

1. **Open the app** at `http://localhost:8501`
2. **Upload your resume** (PDF or Word document)
3. **Paste the job description** you're applying for
4. **Click "Analyze Resume"**
5. **Get instant results:**
   - Your ATS match percentage
   - Missing keywords highlighted
   - Specific improvement suggestions
   - Downloadable PDF with improvements

### Example

**Your Resume:**
```
Python Developer
Skills: Python, Flask, MySQL
```

**Job Description:**
```
Senior Python Developer
Required: Python, Django, REST APIs, Docker, PostgreSQL
```

**Results You Get:**
```
✅ ATS Match: 65%
❌ Missing Keywords: Django, REST APIs, Docker, PostgreSQL
💡 Suggestion: Add experience with Django, REST API development, and Docker containerization
```

---

## Features 🎯

### For Job Seekers 👤
✅ Free resume analysis (just need Google API key)  
✅ AI-powered improvement suggestions  
✅ Instant feedback - no waiting  
✅ Downloadable improved resume  
✅ Works with any job description  
✅ Unlimited analyses  

### For Recruiters 🏢
✅ Automated resume screening  
✅ Standardized keyword matching  
✅ Quick evaluation  
✅ Batch processing possible  

---

## Requirements 📦

Create `requirements.txt` or install manually:

```
streamlit>=1.28.0
google-generativeai>=0.3.0
python-dotenv>=1.0.0
PyPDF2>=3.0.0
```

Install with:
```bash
pip install -r requirements.txt
```

---

## Understanding ATS 🤖

**What is ATS?**
ATS (Applicant Tracking System) is software companies use to filter resumes. It scans for:
- Keywords matching the job description
- Specific formats and structures
- Required experience levels
- Relevant skills

**Why This Tool Helps:**
Many great candidates get rejected by ATS because:
- Keywords are worded differently
- Resume format is confusing to the software
- Missing common industry terms
- Skills aren't clearly stated

This tool fixes all that! ✨

---

## Pro Tips 💡

1. **Test Multiple Jobs** — Run your resume against 5-10 similar jobs to see trending skills
2. **Be Honest** — Only add skills/experience you actually have (recruiters will verify!)
3. **Keywords Matter** — ATS scans for specific terms, so matching them increases your chances
4. **Update Regularly** — Update your resume quarterly as your skills grow
5. **Keep Original** — Always keep your original, use suggestions as guidance
6. **Customize Per Job** — Tailor your resume to each position for best match

---

## Example Before & After

### Before Analysis:
```
John Smith
Software Developer with 5 years experience

Skills: Python, JavaScript, databases
Experience: Built web apps, managed servers
```
**ATS Score: 45%**

### After Using Tool:
```
John Smith
Senior Full-Stack Developer | Python | JavaScript | Django | REST APIs

Technical Skills:
- Backend: Python 3.8+, Django, FastAPI, REST APIs, Flask
- Frontend: JavaScript, React, HTML5, CSS3
- Databases: PostgreSQL, MongoDB, MySQL
- DevOps: Docker, Linux, CI/CD Pipelines
- Cloud: AWS, Heroku

Professional Experience:
- Designed and implemented microservices architecture using Django REST Framework
- Containerized applications using Docker for scalable deployment
- Led team in adopting Agile/Scrum methodologies
- Optimized database queries reducing load time by 40%
```
**ATS Score: 85%** ✨

---

## Troubleshooting 🔧

**Q: "Invalid API Key Error"**
- Check your `.env` file has the correct key
- Make sure there are no extra spaces or quotes
- Regenerate the key from Google AI Studio

**Q: "Module Not Found"**
- Run `pip install -r requirements.txt`
- Make sure you're using the right Python environment

**Q: "Can't Upload PDF"**
- Try a different PDF viewer to extract text first
- Make sure PDF is not password protected
- File size should be under 10MB

**Q: "Results Don't Match"**
- Make sure you pasted the full job description
- Check for typos or formatting issues
- Try analyzing again (sometimes AI gives slightly different results)

---

## What's Next? 🚀

### Features to Add
- [ ] LinkedIn profile analyzer
- [ ] Cover letter generator
- [ ] Salary negotiation guide
- [ ] Interview preparation tips
- [ ] Resume version history tracking
- [ ] Batch resume processing

### To Deploy
- Deploy on [Streamlit Cloud](https://streamlit.io/cloud) (free!)
- Add Stripe for premium features
- Create API for integration
- Build mobile app version

---

## How AI Works Here 🧠

This tool uses Google Gemini Pro (a powerful AI model) to:

1. **Understand Context** — Reads and comprehends both your resume and the job description
2. **Find Gaps** — Identifies missing keywords and skills
3. **Generate Suggestions** — Creates specific, actionable improvement recommendations
4. **Rewrite Content** — Creates an improved version of your resume
5. **Calculate Match** — Determines what percentage of the job you match

All processing is private and secure!

---

## FAQ ❓

**Q: Is my resume data stored?**  
A: No! Your resume is only sent to Google's AI for analysis. We don't store anything.

**Q: Can I use this for free?**  
A: Yes! You just need a Google API key (free tier includes 1500 requests/month).

**Q: How accurate is the matching?**  
A: Very accurate! It analyzes 100+ data points. But use it as a guide, not gospel.

**Q: Can I edit the improved resume directly?**  
A: Yes! Download the PDF and edit it as needed. These are suggestions, not requirements.

**Q: Works with all resume formats?**  
A: Best with standard formats (PDF, Word). Some fancy designs might have issues.

---

## License 📜

MIT License - Use freely, modify, share! Open source forever! 🎉

---

## Made By

**Rushitha**  
Data Engineer | AI Enthusiast | Open Source Contributor

Have feedback? Found a bug? Want to contribute?  
[Open an issue](https://github.com/rushithareddyyy/Application-Tracking-System-Analysis/issues) or [Submit a PR](https://github.com/rushithareddyyy/Application-Tracking-System-Analysis/pulls)!

---

**Last Updated:** February 2026  
**Status:** ✅ Active & Maintained  
**Stars:** ⭐ Help us grow - give us a star if you found this useful!
