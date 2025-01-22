<img src="./readme/title1.svg"/>

<br><br>

<!-- project philosophy -->
<img src="./readme/title2.svg"/>

> EchoWave is a web app for songwriting assistant that helps users craft mood-based, genre-adaptive lyrics while ensuring originality and legal compliance.
>
> The aim to revolutionize the songwriting process by providing a creative, AI-driven platform for lyricists and musicians.

### User Stories

#### User
- As a user, I want to select a mood and genre, so I can generate lyrics that match the vibe of my song.
- As a user, I want to analyze the originality of my lyrics, so I can ensure they are unique and stand out.
- As a user, I want AI-suggested rewrites, so I can improve my lyrics while maintaining their essence.

#### Song Producer
- As a song producer, I want to select two lyrics and provide them to the AI, so it can rewrite them into a new, cohesive song.
- As a song producer, I want to manage my Channel, where I can showcase my created songs, and receive feedback.
- As a song producer, I want to view insights and analytics about the performance of my songs, so I can understand how they are received by the audience.

#### Admin
- As an admin, I want to monitor and moderate content, so I can ensure all submitted lyrics and songs adhere to community guidelines.
- As an admin, I want to handle user support requests and complaints, so I can provide timely and effective solutions.
- As an admin, I want to handle user support requests and complaints, so I can provide timely and effective solutions.

<br><br>
<!-- Tech stack -->
<img src="./readme/title3.svg"/>

###  Echo Wave is built using the following technologies:

- ["ReactJS"](https://react.dev/) - is used for the frontend, providing a dynamic and interactive user interface.For backend services.
- ["Node.js"](https://nodejs.org/en) - and ["Express"](https://expressjs.com/) - are used for the backend, providing scalable, and efficient server-side environment.
- The website's data is stored in ["MongoDB"](https://www.mongodb.com/) -, a NoSQL database that allows for flexible storage and fast retrieval of user-generated content and AI-generated lyrics.
- For AI-powered features, [OpenAI](https://openai.com/) - Integrated to suggest original lyrics for the user.
- ["JWT"](https://jwt.io/) - is used for authentication to provide secure access to protected resources.
- The app uses the font ["Work Sans"](https://fonts.google.com/specimen/Work+Sans) as its main font, and the design of the app adheres to the material design guidelines.
- Machine learning models are trained using ["TensorFlow"](https://www.tensorflow.org/?authuser=1) - and ["scikit-learn"](https://scikit-learn.org/) -, with data processing and training handled separately, while the models are hosted on a Flask server and served through ["FastAPI"](https://fastapi.tiangolo.com/) -.

<br><br>
<!-- UI UX -->
<img src="./readme/title4.svg"/>


> Echo Wave is designed using wireframes and mockups, iterating on the design until the ideal layout was reached for easy navigation and a friendly user experience.

- Project Figma design [figma](https://www.figma.com/design/adR5j8ACHfDyoOaPNZjPis/EchoWave?node-id=14-59&p=f&t=sv7wiOeqeg40YBqp-0)


### Mockups
| Home screen | Profile Screen |
| ---| ---|
| ![Landing](./readme/demo/HomePage.png) | ![fsdaf](./readme/demo/UserPage.png) |

<br><br>

<!-- Database Design -->
<img src="./readme/title5.svg"/>

###  Architecting Data Excellence: Innovative Database Design Strategies:

| Users Model | Lyircs Model | Originality Model|
| ---| ---| ---|
| ![Landing](./readme/demo/UsersModel.png) | ![fsdaf](./readme/demo/LyricsModel.png) | ![fsdaf](./readme/demo/OriginalityModel.png) |


<br><br>


<!-- Implementation -->
<img src="./readme/title6.svg"/>


### User Screens (Web)
| Home | Register |
| ---| ---| 
| ![Landing](./readme/demo/implementation/HomePage.png) | ![fsdaf](./readme/demo/implementation/signUp.png)
| Mood Feature  | Originality Feature |
| ---| ---| 
| ![Landing](./readme/demo/implementation/moodGif.gif) | ![fsdaf](./readme/demo/implementation/originalityGif.gif)

### Song Producer Screens (Web)
| Song Producer Feature  | Song Producer Profile screen |
| ---| ---| 
| ![Landing](./readme/demo/implementation/songProducerGif.gif) | ![fsdaf](./readme/demo/implementation/channels.PNG)
| Song Producer Profile screen
| ---| ---| 
| ![Landing](./readme/demo/implementation/profilePage.PNG)

<br><br>


<!-- Prompt Engineering -->
<img src="./readme/title7.svg"/>

###  EchoWave:

- This project leverages AI to enhance the songwriting process by generating alternative lyrics based on user submissions, offering creative variations to match their desired mood or theme. Additionally, AI is used to merge two sets of lyrics, producing a song that combines elements from both inputs. These AI-driven features provide users with a powerful tool for exploring creativity and originality in music creation. By integrating AI, the project ensures a unique, personalized, and innovative songwriting experience.
| ---
| ![Landing](./readme/demo/prompt.png) 

<br><br>

<!-- AWS Deployment -->
<img src="./readme/title8.svg"/>

###  From Ideas to Innovation: AWS in AI Development

- This project utilizes AWS services to deploy AI and Machine learning models, ensuring high availability, scalability, and performance.
- API endpoints were tested using [Postman](https://www.postman.com/).
- Backend URL: 35.181.154.194:8000

| Create User | Get User |
| ---| ---| 
| ![Landing](./readme/demo/createUser.PNG) | ![fsdaf](./readme/demo/getUser.PNG)
| Lyrics Mood Generation  | Lyrics Originality Check |
| ---| ---| 
| ![Landing](./readme/demo/moodGenerate.PNG) | ![fsdaf](./readme/demo/similarityModel.PNG)

<br><br>

<!-- How to run -->
<img src="./readme/title10.svg"/>

> To set up EchoWave locally, follow these steps:

### Prerequisites

1. Ensure that Node.js and npm are installed on your system.

* npm
  ```sh
  npm install npm@latest -g
  ```

2.  Ensure that you login inside Atlas and create a new project and after naming the project, create a new cluster then setup your connection inside the backend.

3.  Ensure Git is installed for cloning the repository.

### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._
### EchoWave-backend

1. Clone the repo
   git clone https://github.com/OmarMallouk/Echo-Wave.git
2. Install NPM packages
   ```sh
   npm install
   ```
3.  Configure Environment Variables Create a .env file in the root directory and provide the necessary values as follows:

   ```js
   MONGO_URI=mongodb+srv://username:dbpassowrd@cluster0.co4dp.mongodb.net/dbName_db?retryWrites=true&w=majority
   make sure to change the above usernam, password, database name according to your mongo db data 
   OPENAI_API_KEY=API_KEY
   ```

5. After completing the Setup navigate to the EchoWave-server and type the following:
   ```sh
  npm run serve 
  or
  npm run start
  ```
a successfull compile should give you the following message:
  ``sh
   Server running on port 8080 (depending on your port it may vary)
   Connected to MongoDB Atlas

6. Now you should also access the python server directory: src/modules/pythonModules:
   ```sh
   python multiServer.py
   ```
a successfull run should give you the following message:
   ``sh
   * Serving Flask app 'multiServer'
 * Debug mode: on
 * Running on http://127.0.0.1:5000
 * Debugger is active!
 * Debugger PIN: 178-440-388
   ``

### EchoWave-frontend:

1. assuming you have cloned the github repo navigate to the echoWave-app and type the following:
   ``sh
   npm install
   ``

2. After installing the necessary dependencies run the following command to initialize the website:
   ``sh
   npm run dev
   ``
a successfull run should give you the following message:
  VITE v6.0.7  ready in 1111 ms

  ➜  Local:   http://localhost:5173/
  ➜  Network: use --host to expose
  ➜  press h + enter to show help

🌼   daisyUI 4.12.23
├─ ✔︎ 2 themes added            https://daisyui.com/docs/themes
╰─ ★ Star daisyUI on GitHub     https://github.com/saadeghi/daisyui


🌼   daisyUI 4.12.23
├─ ✔︎ 2 themes added            https://daisyui.com/docs/themes
╰─ ❤︎ Support daisyUI project:  https://opencollective.com/daisyui

if not then make sure that you have installed all the dependencies mentioned in the package.json

