# Auto Responder Email

An intelligent email automation workflow designed to categorize incoming emails and generate appropriate responses using AI.

## 🚀 Features

- **Smart Categorization**: Uses AI to classify emails into categories like "Ready to Send Data," "More Info Needed," "Not Interested," or "Pending."
- **Vector Store Integration**: Retrieval-Augmented Generation (RAG) using Supabase to find relevant answers from a knowledge base.
- **AI Response Drafting**: Automatically categorizes and drafts professional, HTML-formatted email responses.
- **Human-in-the-Loop**: Options to review drafts before sending (if configured).

## 🛠️ How It Works

1. **Trigger**: Monitors a Gmail inbox for new unread messages.
2. **Analysis**:
   - Cleans HTML content.
   - Categorizes the email intent.
3. **Response Strategy**:
   - **Data Found**: If a relevant answer exists in the Supabase vector store, it's used to craft a reply.
   - **General Inquiry**: If no specific data is found, a polite acknowledgement and company introduction is generated.
4. **Drafting**: separate AI agents handle drafting based on the categorization (e.g., asking for clarification vs. providing pricing).

## ⚙️ Setup

1. **Import Workflow**: Load `Auto Responder email.json` into n8n.
2. **Credentials Needed**:
   - **Gmail**: For reading and sending emails.
   - **OpenAI**: For the LLM agents.
   - **Supabase**: For the vector store knowledge base.
