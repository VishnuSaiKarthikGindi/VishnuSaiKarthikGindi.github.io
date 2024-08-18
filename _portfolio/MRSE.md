---
title: "Medical Record Search Engine using LLM and KG"
excerpt: "An AI-powered search assistant for healthcare clinics that leverages large language models (LLMs) and knowledge graphs (KGs) to improve patient data retrieval and insights, This innovative approach addresses the challenges posed by traditional chat assistants, such as limited data connectivity and the inability to handle complex queries effectively.
<br/><img src='/images/MRSE2.png'>"
collection: portfolio
---

The data used in this project includes comprehensive patient records, encompassing patient demographics, medical history, medications, lab results, and visit details. The data is typically stored in various text formats. 

1. **Data Ingestion and Processing**: 
   - The data was ingested from different text files, which were then processed to create structured `Document` objects.
   - These documents were subsequently used to populate a Neo4j graph database. The data was transformed into nodes and relationships to create a rich and interconnected knowledge graph that reflects the complexity of patient information.

2. **Model Development**:
   - **Entity and Relationship Extraction**: Using custom designed prompts, the system extracted entities such as patients, conditions, and treatments, as well as their relationships, from the textual data. These were stored in the graph database.
   - **Retrieval-Augmented Generation (RAG)**: The system uses the Langchain framework, combines the strengths of LLMs for understanding natural language queries with the structured retrieval capabilities of the KG. Cypher queries are generated to retrieve relevant data from the graph, which is then used by the LLM to generate contextually accurate responses to user queries.

The knowledge graph enables the system to connect related pieces of information that would typically be isolated in vector bases, providing a more holistic view of patient data. The chat assistant achieved a **15% improvement in query precision** compared to vector database, and reduced the average time to retrieve complex patient information by **25%**, making it a valuable tool in time-sensitive clinical settings.

This project showcases the potential of integrating advanced AI models with knowledge graphs to revolutionize data retrieval in healthcare. For more details, you can view the project code on [GitHub](https://github.com/VishnuSaiKarthikGindi/LLMs_with_KnowledgeGraphs).
