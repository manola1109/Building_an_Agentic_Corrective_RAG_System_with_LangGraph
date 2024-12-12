# Building_an_Agentic_Corrective_RAG_System_with_LangGraph

Building an Agentic Corrective RAG System with LangGraph
This project will cover a full hands-on workflow and demonstration of how to build an Agentic Corrective RAG (CRAG) System with LangGraph

The idea would be to implement the workflow taking inspiration from the Corrective Retrieval Augmented Generation research paper.

The main challenge of RAG systems include:

Poor Retrieval can lead to issues in LLM response generation
Bad retrieval or lack of information in the vector database can also lead to out of context or hallucinated answers
The idea is to couple a RAG system with a few checks in place and perform web searches if there is a lack of relevant context documents to the given user query as follows:



We can build this as an agentic RAG system by having a specific functionality step as a node in the graph and use LangGraph to implement it. Key steps in the node will include prompts being sent to LLMs to perform specific tasks as seen in the detailed workflow below:

