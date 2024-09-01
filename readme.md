# To-Do List Application 📝

This is a simple and user-friendly To-Do List application that helps users manage their day-to-day tasks efficiently. The app allows users to perform all the CRUD applications such as create, read, update, and delete tasks, with all data stored in a database to ensure persistence even after refreshing the page.

## 📜 Features
- **Add Tasks**: Users can easily add tasks to their to-do list.
- **Modify Tasks**: Users can edit existing tasks.
- **Mark as Completed**: Tasks can be marked as completed.
- **Delete Tasks**: Users can delete tasks from the list.
- **Persistent Storage**: All tasks are saved in a database, so they persist even after the page is refreshed.

## 🛠️ Technologies Used
- **Node.js**: A JavaScript runtime environment that allows you to run JavaScript on the server-side. In this project, Node.js is used to handle server operations and manage routing.

- **Express**: A minimal and flexible Node.js web application framework that provides a robust set of features for building web applications. Express is used in this project to manage server routes and handle HTTP requests and responses.

- **EJS (Embedded JavaScript)**: A templating engine that allows you to generate HTML markup with plain JavaScript. EJS is used here to render dynamic content on the web pages based on the data stored in the PostgreSQL database.

- **PostgreSQL**: A powerful, open-source object-relational database system. In this project, PostgreSQL is used to store and manage the tasks, ensuring that the data is persistent and can be retrieved or modified as needed.

- **CSS**: Cascading Style Sheets are used to style the HTML elements on the webpage. In this project, CSS is used to design the layout and appearance of the to-do list, making it visually appealing and user-friendly.

## 🚀 Getting Started

### Prerequisites
Before running the project, make sure you have the following set up:

1. **Create a Table in PostgreSQL**:
   - Use pgAdmin or the psql command line to create a table named `items` in your PostgreSQL database. You can run the following SQL command:
     ```sql
     CREATE TABLE items (
         id SERIAL PRIMARY KEY,
         title TEXT NOT NULL
     );
     ```

2. **Update Database Configuration**:
   - In the `index.js` file, update the database connection settings (host, user, password, database name, and port) according to your local PostgreSQL setup.

### Installation
To run this project locally, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yash-johari/to-do-list-with-postgres.git
    cd to-do-list-with-postgres
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Set up the PostgreSQL database**:
   - Ensure the `items` table is created as per the prerequisites.
   - Update the database connection settings in `index.js` according to your PostgreSQL setup.

4. **Run the application**:
    ```bash
    nodemon index.js
    ```
   - The application will be available at `http://localhost:3000`.

## 📝 Usage
1. Open your browser and go to `http://localhost:3000`.
2. Add tasks by typing into the input field and pressing "Add".
3. Modify or delete tasks as needed. Changes are saved in real-time in the PostgreSQL database.
4. Refresh the page to see that tasks persist, thanks to the database integration.

## Dependencies
- **Express**: Web framework for Node.js.
- **EJS**: Templating engine.
- **pg**: PostgreSQL client for Node.js.

## 🤝 Contributing
Feel free to fork this project, submit issues, and send pull requests. Contributions are always welcome!

## 📧 Contact
Feel free to reach out to me via [LinkedIn](https://www.linkedin.com/in/yash-johari-6575b41b9/) or [Email](mailto:yashjohari2508@gmail.com) for any questions or suggestions.