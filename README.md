# career-multi-agent-system
# **Multi-Agent AI Career Assistance System**

This repository contains the implementation of a multi-agent AI system designed to support job-seeking individuals by automating resume understanding, job role identification, job search retrieval, resume tailoring to a job description, and interview preparation. The tool aims to reduce manual effort in career preparation and provide a structured decision-support workflow powered by AI.

---

## **Overview**

The objective of the system is to streamline the career readiness process by transforming a single resume input into a complete preparation package.
The system is built using modular agents that operate independently but communicate in a pipeline fashion for task execution.

The solution improves efficiency in job search, personal branding, and interview preparation.

---

## **Core Modules / Agents**

| Agent Module               | Functionality                                                                                              |
| -------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **Resume Analyzer**        | Extracts text from PDF resumes using NLP and identifies applicant skills and experience                    |
| **Job Finder Agent**       | Retrieves relevant job postings based on skills and predicted job role                                     |
| **Resume Tailoring Agent** | Automatically restructures and rewrites resume aligned with selected job description for ATS compatibility |
| **Interview Coach Agent**  | Generates interview questions, behavioral prompts, and suggested answers                                   |
| **Project Mentor Agent**   | Suggests project ideas aligned with job requirements to strengthen profile                                 |

---

## **End-to-End Workflow**

1. Resume uploaded
2. NLP extraction and processing
3. Role prediction and skill inference
4. Job retrieval using external job APIs/search queries
5. Resume tailoring according to JD keywords
6. Interview preparation and project suggestions generated
7. Final output delivered as career assistance package

---

## **System Architecture**

Diagram available in artifacts folder:

```
/artifacts/system_architecture.png
```

Layers:

* Input Layer: Resume document
* Processing Layer: Text extraction + role prediction
* Decision Layer: Job match + resume tailoring
* Output Layer: Final recommendations and resources

---

## **Data Flow**

Visualization stored in:

```
/artifacts/dataflow_diagram.png
```

Flow logic:

* Input → Processing → Agent Collaboration → Output
* Sequential multi-agent communication design ensures extensibility

---

## **Implementation Summary**

* Modular architecture allowing each agent to run standalone
* NLP pipelines extract experience, skills, and summary text
* Agent-chaining approach used for execution flow
* Resume tailoring powered through job-description keyword alignment
* Interview preparation uses prompt-based generation mechanism
* Designed to scale: new agents can be added (Email, Learning Path, ATS Scoring etc.)

---

## **Key Goals of The Tool**

* Reduce repetitive manual effort in job search
* Improve resume-job alignment to increase interview calls
* Provide guided interview preparation
* Offer project ideas that increase employability
* Serve as a multi-agent base for future deployment as a career assistant platform

---

## **Future Enhancements**

* Web interface for real-time interaction
* Continuous job scraping feed
* Multi-language resume support
* Personalized learning paths using skill-gap analysis
* ATS score evaluation and optimization insights

---

## **How to Use (Simple Execution Instructions)**

1. Upload resume to input folder or pass to script
2. Run agent modules located in `/src/`
3. Retrieve output generated under `/results/` or console print
4. Flow can be executed agent-by-agent or chained end-to-end

---
