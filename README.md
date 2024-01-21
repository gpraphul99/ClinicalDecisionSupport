# NER FOR EHR WITH NLP
This project detects entities for EHR from natural text input.

## How it works
![working](public/ner-for-ehr.png)

# 1. User Input:

The user interacts with the application by providing health-related information of the patient in natural language.

# 2. Frontend Interaction:

The frontend sends the user's input to a Next.js API route. This API route is responsible for handling the incoming data and facilitating communication with the GPT-3 model.

# 3. NLP Processing:

This project uses LLaMa and GPT-3.5 as NLP layer. The user can choose between them. The model processes the user's natural language input to identify and extract relevant entities, such as name, date of birth, address, allergies, medical history, medications, exercise routine, and diet.

# 4. Entity Extraction:

NLP model extracts structured information from the user's input based on the specified entities. It identifies patterns and relationships in the text to understand the context and extract relevant details.

# 5. Structured JSON Formation:

The extracted information is then used to construct a structured JSON response. This JSON includes key-value pairs representing different entities such as Full Name, Date of Birth, Age, Gender, Address, Allergies, Medical History, Medications, Exercise Routine, and Diet. The structure of the JSON aligns with the desired format for an electronic health record.

# 6. API Response to Frontend:

The Next.js API route sends the structured JSON response back to the frontend.

# 7. Display on Frontend:

The frontend receives the JSON response and displays the extracted health information. However, this state can be alternatively linked to EHR system to integrate NLPs into EHR. 

By leveraging LLM as the NLP layer, the application gains the ability to understand and extract meaningful information from unstructured natural language input, providing a powerful and flexible solution for processing health-related data in electronic health record systems.

## Running Locally

1. Create an account at [OpenAI](https://beta.openai.com/account/api-keys) and add your API key under `OPENAI_API_KEY` in your `.env`
2. Create an account at [Together.ai](https://www.together.ai/) and add your API key under `TOGETHER_API_KEY`
3. Installing dependencies with `pnpm i`
4. Run the application with `pnpm dev` and it will be available at `http://localhost:3000`.
# ClinicalDecisionSupport
# ClinicalDecisionSupport
# ClinicalDecisionSupport
