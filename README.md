
# **Blogger** 

### **Description**

This is a full-stack blog application built with Node.js, MongoDB, Mongoose, EJS for layouts, JSON Web Tokens (JWT) for authentication, and Cookie Parser for session management. Users can browse existing blog posts, while registered admins can create, edit, and delete posts.

## **Technologies**

-   Backend: Node.js, Express.js
-   Database: MongoDB
-   Object Modeling: Mongoose
-   Templating Engine: EJS
-   Authentication: JWT
-   Session Management: Cookie Parser

### **Installation**

1.  **Clone the repository:**
    

    
2. **Configuration**

**Important:** Before running the application, you need to create a file named `.env` in the root directory of your project. The `.env` file should contain the following key-value pairs:

-   `MONGO_URI`: Your MongoDB connection URI.
-   `JWT_SECRET`: A strong, secret password used for signing JWT tokens.

**Example `.env` file:**

- ```MONGO_URI=YOUR_MONGODB_CONNECTION_STRING>```

- ```JWT_SECRET=your_password```

    
    
3.  **Install dependencies:**
    
 ```npm install ```

    
    This will install all the necessary packages from the `package.json` file.
    

### **Development**

1.  Start the development server:
    

    
    ```npm run dev```
    

    ## **Usage**

-   **Browsing Articles:** Anyone can visit the application and freely read existing blog posts.

-   **Admin Functionality:**

    1.  **Registration:** Admins need to register first using the provided registration endpoint (details will be specified in the `routes` directory).
    2.  **Authentication:** Once registered, admins can log in using the login endpoint (details will be specified in the `routes` directory). This will generate a JWT token that is stored in a cookie.
    3.  **Creating Posts:** Authorized admins can create new blog posts through the designated endpoint (details will be specified in the `routes` directory).
    4.  **Editing Posts:** Authorized admins can edit existing posts using the appropriate endpoint (details will be specified in the `routes` directory).
    5.  **Deleting Posts:** Authorized admins can delete posts using the designated endpoint (details will be specified in the `routes` directory).