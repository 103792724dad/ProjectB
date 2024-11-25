Certainly! Here is a cleaned-up version of your deployment instructions for a GitHub README file:

---

# ProjectB

## Apartment Manager

### Backend Deployment

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/giang6996/COS40006---Backend.git
    ```

2. **Setup Environment Variables**:
    - Create a `.env` or `appsettings.json` file with required configurations (e.g., database connection strings).

3. **Initialize the Database**:
    - Run migrations to set up the database:
    ```sh
    dotnet ef migrations add InitialMigration
    dotnet ef database update
    ```

4. **Run the Backend**:
    - Build and start the server:
    ```sh
    dotnet build
    dotnet run
    ```

### Frontend Deployment

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/giang6996/COS40006---Fe.git
    ```

2. **Install Dependencies**:
    - Navigate to the frontend directory and run:
    ```sh
    npm install
    ```

3. **Configure Environment Variables**:
    - Update the `REACT_APP_BACKEND_URL` in the `.env` file to point to the backend API URL.

4. **Run the Frontend**:
    - Start the development server:
    ```sh
    npm start
    ```

### AI Model Deployment

1. **Clone the Repository of the AI Model**:
    ```sh
    git clone https://github.com/giang6996/COS40006---AI-model.git
    ```

2. **Navigate to the AI Model project directory**:
    ```sh
    cd COS40006---AI-model
    ```

3. **Install dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

4. **Running the Fall Detector**:
    ```sh
    python fall_detector.py --video ./examples/fall.mp4 --num_cams 1 --save_output
    ```

5. **Clone the Repository of the AI Server**:
    ```sh
    git clone https://github.com/giang6996/COS40006---AI-server.git
    ```

6. **Navigate to the AI Server project directory**:
    ```sh
    cd COS40006---AI-server
    ```

7. **Adjust the `VIDEO_DIRECTORY`**:
    - Change it to the current directory location of the `saved_falls` in the `COS40006---AI-model` project.
    - For example, if the AI-model and AI-server are next to each other:
    ```python
    VIDEO_DIRECTORY = "../COS40006---AI-model/saved_falls"
    ```

8. **Running the Flask Application**:
    ```sh
    python app.py
    ```

---

You can copy and paste this into your GitHub repository's README file for clear and concise deployment instructions.
