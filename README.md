## Build RAG Using Bedrock & SageMaker

### In this project, we successfully built a Retrieval-Augmented Generation (RAG) system using AWS Bedrock and SageMaker Notebooks. 
### The primary goal was to enhance decision-making by integrating large language models (LLMs) with retrieval mechanisms to generate more accurate, context-aware responses from unstructured data sources such as PDFs, databases, and documents.

### Key Technologies and Concepts Used

#### 1. Retrieval-Augmented Generation (RAG):

##### Traditional generative AI models rely only on their pre-trained knowledge, often lacking real-time or domain-specific accuracy. RAG overcomes this limitation by retrieving relevant information from external knowledge bases before generating responses. This significantly improves accuracy, contextual relevance, and reliability in AI-driven decision-making.

#### 2. AWS Bedrock:

##### AWS Bedrock provides access to state-of-the-art large language models like Amazon Titan and Claude 3 Sonnet. These models offer advanced natural language processing (NLP) capabilities for content generation, summarization, and business applications.

#### 3. LangChain:

##### LangChain serves as the backbone of the retrieval system, allowing us to seamlessly integrate LLMs with external data sources, process text efficiently, and facilitate retrieval-based query processing.

#### 4. LangSmith:

##### LangSmith was used for monitoring, debugging, and optimizing the workflow of our RAG system. It provides valuable insights into retrieval latency, response accuracy, and query execution performance.

#### 5. SageMaker Notebooks:

##### AWS SageMaker Notebooks were used for developing, testing, and deploying the RAG solution in a cloud-based, scalable environment. It provided an ideal workspace to run Python-based LangChain scripts, integrate Bedrock models, and test document retrieval functionalities.

### Implementation Steps

#### 1. Setting Up AWS Services:

##### - We created an AWS SageMaker Notebook instance.

##### - Enabled Claude 3 Sonnet and Amazon Titan in AWS Bedrock.

##### - Configured IAM roles with AmazonBedrockFullAccess policies.

#### 2. Installing Dependencies and Setting Up LangSmith:

##### - We installed essential Python libraries such as pypdf, langchain_community, and boto3.

##### - Created a LangSmith account and obtained an API key for monitoring.

#### 3. Document Retrieval Using LangChain:

##### - Loaded a PDF document using PyPDFLoader.

##### - Processed and split the document into smaller text chunks using RecursiveCharacterTextSplitter.

##### - Stored the vector embeddings in ChromaDB using Amazon Titan embeddings.

#### 4. Querying and Generating Contextual Responses:

##### - Created a retrieval chain using LangChain to fetch relevant document chunks based on user queries.

##### - Used Claude 3 Sonnet as the generative model to formulate accurate responses.

##### - The system successfully retrieved contextual data and generated well-structured answers.

#### 5. Running SQL Queries with LLMs:

##### - Integrated Chinook.db (SQLite database) into the RAG pipeline.

##### - Used Claude 3 Sonnet to generate SQL queries dynamically based on natural language input.

##### - The system retrieved structured data from the database, enhancing the precision of response

#### Final Outcome and Key Achievements

##### By the end of this project, we successfully built, tested, and deployed a RAG system that:
##### ✅ Retrieves relevant documents from PDFs and databases.
##### ✅ Generates accurate, context-aware responses using Claude 3 Sonnet.
##### ✅ Uses LangChain to handle NLP integration and document retrieval.
##### ✅ It leverages LangSmith for debugging and monitoring performance.
##### ✅ Processes structured and unstructured data effectively for business decision-making.
