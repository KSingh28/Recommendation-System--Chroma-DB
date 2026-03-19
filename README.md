# Recommendation-System--Chroma-DB
Create a food recommendation system- Utilize Chroma DB. The code is from IBM Lab
Part 1 Task 1: A. Install the Required Packages
pip install numpy==2.3.1
pip install scipy==1.16.0
pip install chromadb==1.0.12
pip install sentence-transformers==4.1.0
pip install ibm-watsonx-ai==1.3.24


Part 1 Task 1: B. Download the Food Dataset
wget https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/sN1PIR8qp1SJ6K7syv72qQ/FoodDataSet.json

Part 2 Task 1: A. Create the Shared Functions File

Part 2 Task 2: A. Create the Interactive Search File

Part 3 Task 1: A. Create the Advanced Search File
Run the advance search file in terminal:
python3.11 advanced_search.py

**Test different search options:
Option 1: Basic search with "chocolate dessert"
Option 2: Cuisine search for "sweet" in "American" cuisine
Option 3: Calorie search for "dessert" under 300 calories
Option 4: Combined Filters - Use multiple filters together
Option 5: Run the demonstration mode
Option 6: Show the help menu
Option 7: Quit – Exit the program
**

Part 4 Task 1: Building the RAG Chatbot System
Understanding RAG Architecture
Before implementing the code, let's understand what makes this a true RAG system:
Retrieval Phase: Search the vector database for relevant food items based on user query
Context Building: Extract and structure relevant information from search results
Augmented Generation: Pass both the user query and retrieved context to an LLM
Response Generation: The LLM generates a natural, contextual response using the retrieved information

#Run this in terminal
python3.11 enhanced_rag_chatbot.py


**
Test Different Query Types:

Natural Language Queries:

"I want something healthy and light for lunch"
"What Italian comfort food do you recommend?"
"I'm looking for protein-rich breakfast options under 300 calories"
Specific Preference Queries:

"Spicy Asian dishes for dinner"
"Sweet desserts for a special occasion"
"Low-calorie snacks for weight management"
Complex Context Queries:

"I'm feeling sick and want something soothing"
"Quick meal ideas for busy weeknight"
"Celebratory foods for a party"
Test the Comparison Feature:

Type compare when prompted
First query: "chocolate dessert"
Second query: "healthy breakfast"
Observe how the AI analyzes the differences
Observe the RAG Process:

Notice the "Searching vector database..." message (Retrieval)
See "Generating AI-powered response..." (Augmented Generation)
Compare the AI response with the detailed search results shown below**

Part 5: Testing and Comparing All Three Systems
Create a comparison demonstration script called system_comparison.py:
