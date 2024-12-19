# ExDel
EXDEL is a robust and user-friendly courier management system developed using Java Swing, designed to streamline and enhance courier service operations. This desktop application integrates an intuitive graphical user interface (GUI) with a powerful database backend, ensuring efficient data management and seamless functionality.

Here are the steps to install your Java Swing-based **EXDEL Courier Management System** project from GitHub, load it in NetBeans, set up the JDBC driver, and connect it to the database:

---

### Step 1: Clone or Download the Project from GitHub
1. **Clone the repository**:
   - Open a terminal or command prompt.
   - Run the following command to clone the repository:
     ```bash
     git clone https://github.com/your-repository-link/exdel-courier-management.git
     ```
   - Replace `your-repository-link` with the actual GitHub URL for your project.

2. **Download the ZIP file**:
   - Visit your GitHub repository in a browser.
   - Click on the **Code** button, then select **Download ZIP**.
   - Extract the downloaded ZIP file to a desired location.

---

### Step 2: Load the Project in NetBeans
1. **Open NetBeans**:
   - Launch NetBeans on your system.

2. **Open the Project**:
   - Go to `File` > `Open Project`.
   - Navigate to the directory where you cloned or extracted your project.
   - Select the project folder and click **Open**.

3. **Resolve Dependencies** (if applicable):
   - Ensure that all required libraries (e.g., JDBC driver) are available in the project’s `lib` folder or added to the project classpath.

---

### Step 3: Set Up the JDBC Driver
1. **Download the JDBC Driver**:
   - If you are using MySQL, download the MySQL Connector/J driver from [MySQL's official site](https://dev.mysql.com/downloads/connector/j/).

2. **Add the JDBC Driver to NetBeans**:
   - Right-click on your project in the **Projects** panel.
   - Go to `Properties` > `Libraries` > `Add JAR/Folder`.
   - Locate the downloaded JDBC driver JAR file (e.g., `mysql-connector-java-x.x.x.jar`) and add it to your project.

---

### Step 4: Connect to the Database
1. **Create the Database**:
   - Open your database management tool (e.g., phpMyAdmin, MySQL Workbench, or Command Line).
   - Create a new database for your project:
     ```sql
     CREATE DATABASE exdel_db;
     ```
   - Import the SQL schema or dump file for your project (if included in your repository).

2. **Configure Database Connection in Your Code**:
   - Open the database connection class or configuration file in your project.
   - Update the connection string with your database details:
     ```java
     String url = "jdbc:mysql://localhost:3306/exdel_db";
     String user = "your-username";
     String password = "your-password";
     Connection conn = DriverManager.getConnection(url, user, password);
     ```

3. **Test the Connection**:
   - Run the application from NetBeans to ensure the database connection is successful.

---

### Step 5: Running the Project
1. **Build and Run**:
   - In NetBeans, right-click the project and select **Run** or press `F6`.

2. **Verify Functionality**:
   - Check if the GUI loads correctly and all database operations (like retrieving or storing data) work as expected.
