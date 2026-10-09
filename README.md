# AI-Powered CV Analyzer

An intelligent recruitment system that leverages Artificial Intelligence to objectively analyze resumes and evaluate candidates against specific job descriptions.

## 🚀 Features

- **PDF Text Extraction**: Automatically extracts content from candidate resumes in PDF format.
- **AI-Driven Evaluation**: Uses GPT-4o-mini to analyze experience, skills, and educational background.
- **Objective Scoring**: Calculates a "Fit Percentage" based on weighted criteria:
    - Relevant Experience (40%)
    - Technical Skills (35%)
    - Education & Certifications (15%)
    - Professional Consistency (10%)
- **Detailed Feedback**: Provides a structured breakdown of:
    - Key Technical Skills
    - Main Strengths
    - Areas for Improvement
    - Final Hiring Recommendation

## 🛠️ Tech Stack

- **Frontend**: [Streamlit](https://streamlit.io/)
- **LLM Framework**: [LangChain](https://www.langchain.com/)
- **AI Model**: OpenAI `gpt-4o-mini`
- **Data Validation**: [Pydantic](https://docs.pydantic.dev/)
- **PDF Processing**: `PyPDF2`

## 📦 Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd cv_analyzer
   ```

2. **Create a virtual environment**:
   ```powershell
   python -m venv venv
   ```

3. **Activate the environment**:
   - Windows: `.\venv\Scripts\Activate.ps1`
   - macOS/Linux: `source venv/bin/activate`

4. **Install dependencies**:
   ```bash
   pip install streamlit pydantic langchain-openai PyPDF2
   ```

## ⚙️ Configuration

The system requires an OpenAI API Key. You can set it as an environment variable:

**Windows (PowerShell):**
```powershell
$env:OPENAI_API_KEY="your-api-key-here"
```

**macOS/Linux:**
```bash
export OPENAI_API_KEY="your-api-key-here"
```

## 🚀 Running the Application

To launch the user interface, run:

```bash
streamlit run app.py
```

The application will be available at `http://localhost:8501`.

## 📖 How to Use

1. **Upload CV**: Drag and drop the candidate's resume in PDF format.
2. **Job Description**: Paste the detailed requirements, responsibilities, and skills for the position you are filling.
3. **Analyze**: Click on "Analyze Candidate" to generate the professional evaluation.
4. **Review**: Check the Fit Percentage, Profile Summary, and the Final Recommendation.
