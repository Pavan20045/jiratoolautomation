# Jira MoM Issue Creator

Automatically convert your meeting transcripts into actionable Jira issues using AI and Jira REST APIs. Just upload a `.txt` transcript and this tool will handle the rest — MoM generation, issue extraction, assignment, and Jira task creation.

---

## Features

- Upload `.txt` meeting transcripts
- Generate Minutes of Meeting (MoM) using Moonshot AI
- Extract actionable issues with assigned team members
- Auto-create tasks in Jira via REST API
- Prevent duplicate issues based on summary
- Clean and user-friendly web interface (HTML + JS)

---

## Built With

- Python – Flask for backend
- Moonshot API – For natural language MoM generation
- Jira REST API – For automated task creation
- Regex – For extracting issues and assignees
- HTML + JavaScript – Simple frontend form

---

## Prerequisites

### 1. Jira API Access

- Create a Jira account and generate an API token:  
  https://id.atlassian.com/manage-profile/security/api-tokens

### 2. Moonshot API Key

- A static demo key is already included in the code for testing.

---

## Sample Transcript Format

Place your meeting transcript in `.txt` format using a clear speaker format and time stamps.  

## Folder Structure

.
├── app.py # Flask app handling form, processing, and Jira integration
├── sample_transcript.txt # Sample .txt file to test the app
├── requirements.txt # Python dependencies
└── README.md # This documentation

## How to Run

1. Clone the Repository

git clone https://github.com/Pavan20045/jiratoolautomation
cd jiratoolautomation

2. Install Dependencies

pip install -r requirements.txt

3. Run the App using this command:

  python app.py

4. Access the Interface

Open your browser and navigate to:  
http://127.0.0.1:PORT

5. Submit Form

Fill in:
- Jira Email
- Jira API Token
- Jira Instance URL
- Jira Project Name
- Upload `.txt` transcript file

Click Submit to automatically generate and post Jira issues.

---

## Notes

- The system skips duplicate issues by checking if an issue with the same summary already exists.
- Make sure that the assignee names in the transcript match the user names in your Jira instance.

---

## License

This project is for demo and educational use. For production use, secure all API keys and consider authentication and rate-limiting.
