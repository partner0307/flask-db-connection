# Flask Project with Different Database Connections

This repository contains a Flask project that demonstrates how to connect to different types of databases. It includes examples for MySQL, PostgreSQL, and MongoDB.

## Installation

To run this project locally, follow these steps:

1. Clone the repository to your local machine using the following command:

   ```
   git clone https://github.com/your-username/flask-database-connections.git
   ```

2. Navigate to the project directory:

   ```
   cd flask-database-connections
   ```

3. Create a virtual environment to isolate the project's dependencies:

   ```
   python -m venv env
   ```

4. Activate the virtual environment:

   - On macOS and Linux:
     ```
     source env/bin/activate
     ```

   - On Windows:
     ```
     .\env\Scripts\activate
     ```

5. Install the project dependencies:

   ```
   pip install -r requirements.txt
   ```

6. Create a `.env` file in the project directory with the following contents:

   ```
   FLASK_APP=app
   FLASK_ENV=development
   DATABASE_URL=mysql+pymysql://username:password@localhost/database_name
   MONGO_URI=mongodb://localhost:27017/database_name
   ```

   Replace `username`, `password`, and `database_name` with your own values.

7. Run the Flask development server:

   ```
   flask run
   ```

8. Open your web browser and visit `http://localhost:5000` to access the application.

## Usage

This Flask application demonstrates how to connect to different types of databases using SQLAlchemy. Here are the available routes:

- `/mysql`: Displays data from a MySQL database.
- `/mongo`: Displays data from a MongoDB database.

Each route connects to a different type of database and displays data from it.

Feel free to explore the project's code and modify it according to your needs.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

If you have any questions or suggestions, feel free to contact us at [email@example.com](mailto:email@example.com).
