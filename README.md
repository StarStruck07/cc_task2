# AI agent for assisting through engineering admissions in India

This agent adequately answers user’s query regarding various engineering entrance exams, such as exam dates, registration deadlines, results etc

Moreover, it inquires the user about its exam scores, interests, branch preferences, location preferences to assess user’s profile and recommends it 3 engineering colleges in India

I have used llama3.1 llm, chroma db vector store, hugging face embeddings, and langchain as a framework to integrate these together. 

I have embedded top 100 engineering colleges as per NIRF data, with their rank and city as a csv file. 

The input entered by user is searched in web through tavily search API. The results of the search, also with the retrieved information from the vector database is fed into the prompt of llm

Although it would be a hassle, cutoffs and recommendations could be much more accurate by embedding an excel sheet/csv file of the cutoffs of all the branches of all colleges in the database

Instead of the above, I tried using ReAct agent, but that took too long to compute even simple queries, hence had to scratch that. 
