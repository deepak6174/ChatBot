# Chatbot Recommender Systems

## 1. Introduction
I developed a chatbot capable of recommending restaurants and movies based on user preferences and past interactions. The chatbot utilizes two distinct recommender systems connected by an intent classifier. The classifier determines whether the user query pertains to restaurant recommendations or movie suggestions. 

The restaurant recommender system identifies the type of cuisine and location preferences of the user, offering recommendations sorted by restaurant ratings. Similarly, the movie recommender system recommends new movies based on the genre similarity with movies the user has previously watched, filtering out lower-rated options.

## 2. Background
The concept for this project was inspired by lectures on Human-AI Interaction, focusing on similarity-based recommender systems. TF-IDF was used to assign weights to words in documents, enabling cosine similarity calculation to find the closest matches. 

Ambiguity in user queries is managed through clarification questions, ensuring accurate intent classification. Disambiguation and clarification intents are implemented in the restaurant chatbot, facilitating context retention and handling ambiguous situations effectively.

## 3. Proposed Systems
### 3.1. Intent Hierarchy
The intent hierarchy diagram illustrates the arrangement of different intents within the chatbot. Intents guide the flow of conversations, ensuring seamless interactions between the user and the chatbot.

### 3.2. Restaurant Chatbot
The restaurant chatbot utilizes a dataset containing restaurant names, ratings, cuisine tags, and locations. Cosine similarity is calculated between the user query and restaurant tags + city name to provide relevant recommendations.

### 3.3. Movie Chatbot
The movie chatbot relies on a dataset containing movie names, ratings, and genres. It identifies the movie mentioned in the user query and recommends similar movies based on genre similarity.

## 4. Evaluation
Evaluation involves testing the restaurant and movie recommendation chatbots and intent classification. Manual testing ensures the accuracy and effectiveness of each component. Accuracy evaluation of the movie chatbot is based on the expected recommendation column in the dataset.

## 5. Discussion
### 5.1. Evaluation Inference
Testing revealed instances of incorrect recommendations due to tags present in restaurant names and movie sequels. Intent classification performs reasonably well, with occasional misclassifications.

### 5.2. Potential Impact
The chatbot offers users a convenient way to explore restaurants and movies based on their preferences, benefiting the entertainment and hospitality industries. It addresses the challenge of identifying good movies and restaurants among a vast selection.

### 5.3. Bias
Bias in the recommendations may stem from the dataset, reflecting the preferences of specific cities or regions.

## 6. Conclusion
The chatbot leverages TF-IDF and cosine similarity to provide tailored recommendations for restaurants and movies. While it effectively addresses user needs, improvements can be made to handle tag biases in restaurant and movie names.

Overall, the chatbot offers a practical solution for both users seeking recommendations and businesses aiming to attract customers.

---

**Start your conversation with the chatbot:**

User: Hi  
ChatBot: Hello  
User: Find me a vegan restaurant with a rating 5  
ChatBot: Tell me the city you want the restaurant to be in  
User: London  
ChatBot: Found 191 restaurants.  
1. R & H Cafe Gallery  
2. Liman Restaurant  
3. Holy Smoke  
4. The Clink Restaurant  
5. Bar 61 Restaurant  
ChatBot: Do you want to see all?  
User: no  

---
## 7. Youtube Code Walk

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/VZEVI8fNkyg/0.jpg)](https://www.youtube.com/watch?v=VZEVI8fNkyg)

[Report.pdf](https://github.com/deepak6174/ChatBot/files/15032433/Assignment.1.Report.pdf)


