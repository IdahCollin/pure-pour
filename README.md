<p align="center"><img src="frontend/src/assets/favicon-martini.png" alt="Logo" width="10%"></p><br>

"Pure Pour" generates mocktails by integrating with the OpenAI API. Recipe generation is based on user prompts of ingredients. <br><br>

## Technologies used

<div style="display: flex; justify-content: space-between; gap: 10px;">

<div style="width: 30%;">

**Frontend**

- React (HTML, CSS, JavaScript)
- Vite
- Zustand
- React Router
- React Icons

</div>

<div style="width: 30%;">

**Backend**

- Node.js
- Express
- MongoDB
- Mongoose
- OpenAI
- Nodemon

</div>

<div style="width: 30%;">

**Other**

- GitHub
- Figma
- VScode
- Squoosh
- Affinity Designer<br><br><br>
</div>
</div>

## Database Operations

- **RecipeModel:** Represents the data structure for recipes, including user input, search words, title, description, ingredients, instructions, and creation timestamp.
- **MongoDBOperations:** Implements CRUD operations for managing recipes in the MongoDB database.
<br><br>

## AI integration

**OpenAI:** The backend integrates with the OpenAI API to generate text-based recipes based on user prompts.

**Endpoint:** Provides an /openai/generateText endpoint to handle AI-driven recipe generation.
<br><br>

## API Endpoints

### External APIs

**OpenAI API:**

- **Description:** Utilized to generate text-based recipes based on user prompts.
- **Endpoint:** `POST /openai/generateText`
- **Usage:** This API is integrated into the backend to dynamically create recipes using the OpenAI GPT-3 model.

### Internal APIs

**MongoDB API:**

- **Description:** The backend acts as an API to interact with the MongoDB database.
- **Endpoints:**
  - `GET /`: Lists all available API endpoints for reference.
  - `GET /recipes`: Retrieves all stored recipes.
  - `GET /recipes/search/:query`: Searches for recipes based on a specified query.
 <br><br>

## How to Run the Project

### Backend

1. **Clone the Repository:**

```
git clone hobby-drinks
```

2. **Navigate to the Backend Directory**

```
cd backend
```

3. **Install Dependencies**

```
npm install
```

4. **Set Environment Variables**
   Create a .env file in the backend directory and add necessary environment variables, including PORT, MongoDB connection details, and OpenAI API key.

Example .env:

```
PORT=3001
MONGO_URL=[your-mongodb-url]
OPENAI_API_KEY=[your-openai-api-key]
```

5. **Start the Backend Server**

```
npm start
```

### Frontend

1. **Navigate to the Frontend Directory**

```
cd frontend
```

2. **Install Dependencies**

```
npm install
```

3. **Set Environment Variables**
   Create a .env file in the frontend directory and add an environment variables for the backend localhost.

Example .env:

```
VITE_BACKEND_API=[backend-localhost]
```

4. **Start the Frontend Development Server**

```
npm run dev
```
<br>

## Challenges

It was a challenge connecting to the OpenAI API. Many of the explanatory videos and similar repos on GitHub already were outdated as the openAI technology develops very fast. But reading the documentation on OpenAIs website very thouroughly, in combination with studying similar projects helped.

Continuing to explore the subject of prompt engineering and learning how to structure texts in a way so they are intepreted and understood by AI models as intended. 
<br><br>

## Project Process

Input info here. This is a hobby project inspired by a project built by Emmy Dieden and me.

Moving forward: 
The project is prepared for further development, such as using authentication for building a login function. There is a prepared endpoint for searching for recipes, which only needs to be implemented in the frontend. To extend the project further, next step would be to build an endpoint for saving recipes to the database, and also fine-tune the model for even better responses. 

Google Lighthouse and cross-browser testing show satisfactory results.
<br><br>

## View it live

**Frontend:** <br>

**Backend:** <br><br>

## Let's connect!

**Idah Collin:**<br>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/idah-collin)<br>

[![GitHub](https://img.shields.io/badge/GitHub-black?style=flat-square&logo=github)](https://github.com/IdahCollin)<br>

[Portfolio](https://idah-collin-portfolio.netlify.app/)<br>

