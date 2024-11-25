# ProjectB
Apartment Manager
Backend Deployment
1.	Clone the Repository:
○	Run: git clone https://github.com/giang6996/COS40006---Backend.git.
2.	Setup Environment Variables:
○	Create a .env or appsettings.json file with required configurations (e.g., database connection strings).
3.	Initialize the Database:
○	Run migrations to set up the database:
■	dotnet ef migrations add InitialMigration.
■	dotnet ef database update.
4.	Run the Backend:
○	Build and start the server:
■	dotnet build.
■	dotnet run.
Frontend Deployment
1.	Clone the Repository:
○	Run: git clone https://github.com/giang6996/COS40006---Fe.git.
2.	Install Dependencies:
○	Navigate to the frontend directory and run: npm install.
3.	Configure Environment Variables:
○	Update the REACT_APP_BACKEND_URL in the .env file to point to the backend API URL.
4.	Run the Frontend:
○	Start the development server:
■	npm start.
AI Model Deployment
1.	Clone the Repository of the AI Model:
○	Run: git clone https://github.com/giang6996/COS40006---AI-model.git
2.	Navigate to the AI Model project directory
○	Run: cd COS40006---AI-model
3.	Install dependencies:
○	Run: pip install -r requirements.txt
4.	Running the Fall Detector:
○	Run: python fall_detector.py --video ./examples/fall.mp4 --num_cams 1 --save_output
5.	Clone the Repository of the AI Server:
○	Run: git clone https://github.com/giang6996/COS40006---AI-server.git
6.	Navigate to the AI Server project directory:
○	Run: cd COS40006---AI-server
7.	Adjust the “VIDEO_DIRECTORY”:
○	Change it to the current directory location of the saved_falls in the COS40006---AI-model project, for example, if the AI-model and Al-server are next to each other:
■	VIDEO_DIRECTORY = "../COS40006---AI-model/saved_falls"
8.	Running the Flask Application:
○	Run: python app.py
