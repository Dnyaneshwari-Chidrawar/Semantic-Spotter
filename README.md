# Semantic-Spotter
Llama-Index is used to store and retrieve the user query

## Context
- OpenAI LLM model's limitation is it does not have domain specific knowledge. This limitation can be resolved by the Llama-Index or Langchain.
- I have taken the myntra fashion dataset and stored using llama-index.
- when the user query comes, llama-index retrieve the document and it market the retrieved product.

## Business Objective:
- Create a generative search engine capable of searching a plethora of product descriptions to find and recommend appropriate choices against user query.

## Design: 
- Loading the data set.
- Understanding and cleaning the data
- Feed the formatted data to Llama-Index
- Create the Llama-Index query engine
- Retrieve the document and present it to the user in well structured format.

## Implementation: 
- In this project, I have used Llama_index library to build the Myntra fashion Search AI.
- Used Chat.Completion.Create API from OpenAI to generate the marketing response message of the retrieved product.
- Used matplotlib library to show the image of the final product as per user query
- Used requests library to extract the image from the given URL.

## Challenges:
- SimpleDirectoryReader does not read csv file. I have read the csv file using pandas library.
- Llama_index does not take dataframe as input. I had to convert the dataframe into list of documents of the text.
- Llama_index LLM output is not as per the expectation. I had to take the help from OpenAI LLM models to generate the required output.
- Yes, we can customize the LLM prompt of Llama-Index, but it is little complicated to implement.


## Lessons learnt: 
- Llama-Index storing and retrieval is faster than chromadb or other vector stores. 
- Implementation is simple in using Llama_index module
- But the flexibility and accuracy is lesser than chromadb.
- It is difficult to give customized prompt to llama-index LLMs. Where as in chromadb, we can give customized document, metadata, and prompt.
