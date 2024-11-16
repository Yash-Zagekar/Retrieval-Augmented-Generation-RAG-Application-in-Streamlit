
```markdown
# Chat with documents : Receive Immediate Insights from documents


Chat with documents is an advanced Streamlit application designed to extract and analyze text from various document formats, utilizing the powerful capabilities of Google's Generative AI, specifically the Gemini-PRO model. This tool employs a Retrieval-Augmented Generation (RAG) framework to provide highly accurate, context-sensitive responses to user queries, drawing on the content within the uploaded documents. By processing the text of these documents, the application is able to deliver detailed and relevant information, ensuring that users receive precise answers tailored to the specific content they upload. This system enhances the user experience by facilitating efficient and intelligent document-based interactions.
## Features

- **Instant Analysis**: Extracts and processes text from uploaded documents to deliver immediate, valuable insights.
- **Contextual AI Responses**: Leverages Google's Gemini-PRO Generative AI model for delivering accurate and context-aware answers.

## 🌟Lets get started

### Prerequisites

- Google API Key : You need a Google API key to interact with Google's Generative AI models. To obtain your key, visit [Google API Key Setup](https://makersuite.google.com/app/apikey).
- Streamlit : This application is developed using Streamlit. Make sure Streamlit is installed in your environment to run the application.

```bash
- Installation
- To install the necessary dependencies, run:

- bash
- pip install -r requirements.txt
- How to Use
- Launch the Application: Start the Streamlit app by executing the following command:

- bash
- streamlit run <path_to_script.py>
- Replace <path_to_script.py> with the path to the script file.

- Input Your Google API Key: When prompted, securely enter your Google API key. This key allows the application to access Google's Generative AI models.

- Upload Documents: Upload one or more documents. The application will analyze their contents to provide responses based on the text.

- Ask Questions: After processing the documents, you can ask any question related to their content, and the application will generate an appropriate response.

### Technical Overview
- Document Processing: Uses PyPDF2 for extracting text from uploaded documents.
- Text Segmentation: The RecursiveCharacterTextSplitter from LangChain is used to break the extracted text into manageable segments.
- Vector Store: Implements FAISS to create a searchable vector store from the text chunks.
- Answer Generation: Uses ChatGoogleGenerativeAI from LangChain to generate responses to user queries, leveraging the context from the uploaded documents.

### App link - https://retrieval-augmented-generation-rag-application.streamlit.app/


