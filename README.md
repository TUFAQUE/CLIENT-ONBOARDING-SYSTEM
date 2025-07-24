# 🤖 AI-Powered Client Onboarding Workflow (n8n + GPT-4o)

A fully automated AI onboarding agent built with [n8n](https://n8n.io), OpenAI (GPT-4o), Google Drive, ClickUp, Slack, and Gmail. This workflow handles everything from proposal upload to task assignment — with no manual steps needed.

---

## 🚀 What It Does

1. **Client Submission Form**  
   - Collects name, email, company name, website, and scoping document via form.

2. **AI-Powered Task Breakdown**  
   - Uses OpenAI GPT-4o to analyze the uploaded PDF proposal.
   - Breaks it into 20–30 actionable subtasks with estimated due dates.

3. **ClickUp Project Automation**  
   - Creates folder and list in ClickUp.
   - Automatically adds all AI-generated tasks to the client project.

4. **Google Drive Folder Setup**  
   - Creates a dedicated Google Drive folder for shared documents.

5. **Slack Channel Creation**  
   - Auto-creates a Slack channel and posts a personalized welcome message.

6. **Personalized Welcome Email**  
   - Sends a Gmail welcome email to the client with:
     - Google Drive link
     - Onboarding call scheduler
     - Slack + ClickUp instructions

---

## 🎯 Why Use This?

Manual onboarding takes time, introduces inconsistencies, and distracts your team from strategic work.  
This agent helps you:

- Onboard clients in **under 2 minutes**
- Automate multi-tool setup (Drive, Slack, ClickUp)
- Deliver a premium onboarding experience at scale
- Eliminate human errors and task duplication

---

## 🔧 APIs & Services Used

| Service         | Purpose                                |
|----------------|----------------------------------------|
| OpenAI GPT-4o   | Break down proposals into tasks        |
| Google Drive API| Create shared client folder            |
| ClickUp API     | Create folders, lists, and tasks       |
| Slack API       | Create client communication channel    |
| Gmail API       | Send onboarding emails                 |
| n8n             | Workflow orchestration engine          |

---

## 🛠️ Setup Instructions

1. **Import the Workflow**  
   Download the `.json` and import it into your [n8n instance](https://docs.n8n.io/hosting/installation/).

2. **Connect All Credentials**  
   - Google Drive OAuth2  
   - ClickUp OAuth2  
   - Slack Bot Token (OAuth2)  
   - Gmail OAuth2  
   - OpenAI API Key

3. **Update IDs**  
   - Replace the parent folder ID in Google Drive node.  
   - Set your actual ClickUp space, team, and template IDs.  
   - Link your onboarding form and calendar link (e.g., OnceHub or Cal.com).

4. **Deploy and Share the Form**  
   - Embed or send the client onboarding form.
   - Sit back and let automation take over!

---

## 🧩 Input Form Fields

The agent expects these fields from the form:

- **Name**  
- **Email**  
- **Company Name**  
- **Website**  
- **Proposal / Scope Document** (PDF)

---

## 🧠 Sample Output Tasks (From GPT-4o)

> "Initial strategy alignment call and documentation setup expected within first 3 days."

| Task Title                  | Description                                                  | Due Date     |
|----------------------------|--------------------------------------------------------------|--------------|
| Book Strategy Call          | Coordinate & schedule a kickoff call with the client         | MM/DD/YYYY   |
| Create Strategy Notes Doc   | Prepare shared doc to collect meeting notes                  | MM/DD/YYYY   |
| Create Project Workspace    | Set up access to Slack, ClickUp, Google Drive                | MM/DD/YYYY   |

*...and up to 30 similar detailed tasks generated.*

---

## 👨‍💻 Developed By

**Tufaque Sayyed**  
AI/ML Engineer | Data Scientist 
🌐 [Portfolio](https://tufaquesayyed.vercel.app)  
🔗 [LinkedIn](https://www.linkedin.com/in/tufaque-sayyed-843596364/)

---

## 📄 License

MIT – Feel free to use, fork, and customize this agent for your business.  
If it helps, leave a ⭐ on the repo!



👨‍💻 Developed By
Tufaque Sayyed
AI & ML Engineer | Data Scientist | Ai Agent Builder 
🌐 Portfolio
🔗 LinkedIn
