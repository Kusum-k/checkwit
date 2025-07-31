# Build and Deploy a Full Stack MERN AI Image Generation App  MidJourney & DALL E Clone
![Image Generation App](https://i.ibb.co/p0f27C2/Thumbnail-9.png)

CheckWit is a full-stack AI-powered web app that generates high-quality images from natural language prompts. Built with the MERN stack and OpenAI’s DALL·E API, users can create, view, and share generated art through a sleek, responsive interface.

##  Tech Stack

The project is built using the **MERN stack**. The frontend is developed with **React (using Vite for fast bundling)** and styled using **Tailwind CSS** for a clean, responsive UI. The backend is powered by **Node.js** and **Express.js**, handling API requests and server-side logic. **MongoDB Atlas** is used as the cloud database to store generated images and user posts. For AI image generation, the app integrates **OpenAI’s DALL·E API**. The application is hosted using **Vercel** (for the frontend) and **Render** (for the backend).


##  How It Works

1. User enters a **text prompt**  
2. Frontend sends the prompt to backend via REST API  
3. Backend uses **OpenAI API** to generate a base64 image  
4. The image is displayed instantly and can be shared to the community gallery  
5. All shared posts are saved in **MongoDB** and shown on the homepage
   
## Project Structure

The project is organized into two main directories: `client` and `server`. The `client` folder contains the frontend code, built using React (with Vite) and styled using Tailwind CSS. The `server` folder holds the backend logic built with Node.js and Express, including API routes and integration with OpenAI and MongoDB. The root directory also includes the `README.md` file for project documentation.


##  Local Setup Instructions

### 1. Clone the Project
git clone https://github.com/Kusum-k/checkwit.git
cd checkwit

### 2. Setup Backend
cd server
npm install

Create a `.env` file:
OPENAI_API_KEY=your-openai-api-key
MONGODB_URL=your-mongodb-atlas-url

Start the server:
npm start

### 3. Setup Frontend
cd ../client
npm install

Create a `.env` file:

VITE_SERVER_URL=http://localhost:5000


Run the frontend:
npm run dev

##  Usage Instructions

Once both the frontend and backend are running locally:

1. Open your browser and go to: [http://localhost:5173](http://localhost:5173)
2. Enter a creative prompt in the input field 
3. Click **Generate** to create an AI-generated image using OpenAI's DALL·E model
4. Optionally, click **Share with Community** to publish your image to the public gallery
5. Browse all shared images on the homepage

 Enjoy your AI art creation experience!



