# langchain
Resources:
- https://www.pinecone.io/learn/langchain-prompt-templates/

|[**langchain tutorial to follow**](https://github.com/gkamradt/langchain-tutorials.git)|

What is LangChain?
LangChain is a framework built to help you build LLM-powered applications more easily by providing you with the following:

- a generic interface to a variety of different foundation models (see Models),
- a framework to help you manage your prompts (see Prompts), and
- a central interface to long-term memory (see Memory), external data (see Indexes), other LLMs (see Chains), and other agents for tasks an LLM is not able to handle (e.g., calculations or search) (see Agents).
- It is an open-source project (GitHub repository) created by Harrison Chase.

Because LangChain has a lot of different functionalities, it may be challenging to understand what it does at first. That’s why we will go over the (currently) six key modules of LangChain in this article to give you a better understanding of its capabilities.

<h2>Prerequisites<h2>
To follow along in this tutorial, you will need to have the langchain Python package installed and all relevant API keys ready to use.

  ![11](https://github.com/andysingal/langchain/blob/main/Images/Screenshot%202023-06-16%20at%2012.58.31%20PM.png)  

What can you do with LangChain?
The package provides a generic interface to many foundation models, enables prompt management, and acts as a central interface to other components like prompt templates, other LLMs, external data, and other tools via agents.

At the time of writing, LangChain (version 0.0.147) covers six modules:

- Models: Choosing from different LLMs and embedding models
- Prompts: Managing LLM inputs
- Chains: Combining LLMs with other components
- Indexes: Accessing external data
- Memory: Remembering previous conversations
- Agents: Accessing other tools
- The code examples in the following sections are copied and modified from the LangChain documentation.

Models: Choosing from different LLMs and embedding models
Currently, many different LLMs are emerging. LangChain offers integrations to a wide range of models and a streamlined interface to all of them.

LangChain differentiates between three types of models that differ in their inputs and outputs:

LLMs take a string as an input (prompt) and output a string (completion).
  
  
  
