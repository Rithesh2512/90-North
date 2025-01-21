
# Project Title
## Real-Time Chat Application

## Description
The Real-Time Chat Application is a web-based platform that allows users to communicate with each other in real-time. Built using Django for the backend and HTML/CSS/JavaScript for the frontend, this application utilizes Django Channels to facilitate WebSocket connections, enabling instant message delivery. The application is designed to be responsive, ensuring a seamless user experience across various devices, including desktops and mobile phones. Additionally, it integrates an AWS Lambda function to perform simple arithmetic operations, showcasing the power of serverless computing.

## Installation Instructions

### Prerequisites
Before you begin, ensure you have the following installed on your machine:
- **Python 3.x**: The programming language used for the backend.
- **pip**: The package installer for Python.
- **Git**: For cloning the repository.

### Clone the Repository
1. Open your terminal or command prompt.
2. Clone the repository using the following command:
   ```bash
   git clone https://github.com/yourusername/real-time-chat-app.git
   cd real-time-chat-app
   ```

### Set Up the Backend
1. **Create a virtual environment**:
   ```bash
   python -m venv venv
   ```
   - Activate the virtual environment:
     - On Windows:
       ```bash
       venv\Scripts\activate
       ```
     - On macOS/Linux:
       ```bash
       source venv/bin/activate
       ```

2. **Install the required dependencies**:
   ```bash
   pip install django channels
   ```

3. **Run database migrations**:
   ```bash
   python manage.py migrate
   ```

4. **Start the development server**:
   ```bash
   python manage.py runserver
   ```

### Set Up the Frontend
- The frontend files are located in the `frontend` directory. Open `index.html` in your web browser to view the application.

## Usage Instructions
1. Once the development server is running, navigate to `http://127.0.0.1:8000` in your web browser.
2. You will see the chat interface where you can enter your name and start chatting.
3. Open multiple browser tabs or windows to simulate different users chatting in real-time.
4. To use the AWS Lambda function, you can implement a feature in the frontend that allows users to input two numbers and receive the sum by invoking the Lambda function.

## Features
- **Real-time Chat**: Users can send and receive messages instantly without refreshing the page, thanks to WebSocket support via Django Channels.
- **Responsive Design**: The application is designed to adapt to various screen sizes, providing an optimal user experience on both desktop and mobile devices.
- **User -Friendly Interface**: The chat interface is simple and intuitive, allowing users to easily navigate and participate in conversations.
- **AWS Lambda Integration**: The application includes a serverless function that can perform arithmetic operations, demonstrating the ability to extend functionality using cloud services.
- **Scalability**: Built with Django, the application can be easily scaled to accommodate more users and features in the future.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Special thanks to the Django and AWS communities for their extensive documentation and support.
- Acknowledgment to [Your Mentor/Instructor Name] for guidance throughout the development of this project.
```














   # Project Title
   ## Responsive Chat Application

   ## Description
   The Responsive Chat Application is a web-based platform that allows users to engage in real-time conversations. Built using Django for the backend and HTML/CSS/JavaScript for the frontend, this application leverages Django Channels to provide a seamless chat experience. The application is designed to be responsive, ensuring that it works well on both desktop and mobile devices. Additionally, it integrates an AWS Lambda function to perform simple arithmetic operations, showcasing the versatility of serverless computing.

   ## Installation Instructions

   ### Prerequisites
   Before you begin, ensure you have the following installed on your machine:
   - Python 3.x
   - pip (Python package installer)
   - Git (for cloning the repository)

   ### Clone the Repository
   1. Open your terminal or command prompt.
   2. Clone the repository using the following command:
      ```bash
      git clone https://github.com/yourusername/responsive-chat-app.git
      cd responsive-chat-app
      ```

   ### Set Up the Backend
   1. **Create a virtual environment**:
      ```bash
      python -m venv venv
      ```
      - Activate the virtual environment:
        - On Windows:
          ```bash
          venv\Scripts\activate
          ```
        - On macOS/Linux:
          ```bash
          source venv/bin/activate
          ```

   2. **Install the required dependencies**:
      ```bash
      pip install django channels
      ```

   3. **Run database migrations**:
      ```bash
      python manage.py migrate
      ```

   4. **Start the development server**:
      ```bash
      python manage.py runserver
      ```

   ### Set Up the Frontend
   - The frontend files are located in the `frontend` directory. Open `index.html` in your web browser to view the application.

   ## Usage Instructions
   1. Once the development server is running, navigate to `http://127.0.0.1:8000` in your web browser.
   2. You will see the chat interface where you can enter your name and start chatting.
   3. Open multiple browser tabs or windows to simulate different users chatting in real-time.
   4. To use the AWS Lambda function, you can implement a feature in the frontend that allows users to input two numbers and receive the sum by invoking the Lambda function.

   ## Features
   - **Real-time Chat**: Users can send and receive messages instantly without refreshing the page, thanks to WebSocket support via Django Channels.
   - **Responsive Design**: The application is designed to adapt to various screen sizes, providing an optimal user experience on both desktop and mobile devices.
   - **User -Friendly Interface**: The chat interface is simple and intuitive, allowing users to easily navigate and participate in conversations.
   - **AWS Lambda Integration**: The application includes a serverless function that can perform arithmetic operations, demonstrating the ability to extend functionality using cloud services.
   - **Scalability**: Built with Django, the application can be easily scaled to accommodate more users and features in the future.

   ## License
   This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

   ## Acknowledgments
   - Special thanks to the Django and AWS communities for their extensive documentation and support.
   - Acknowledgment to [Your Mentor/Instructor Name] for guidance throughout the development of this project.
   ```















# Project Title
## AWS Lambda Functions for Basic Operations

## Description
This project contains two AWS Lambda functions designed to demonstrate basic serverless computing capabilities using AWS. The first function adds two numbers and returns the result, while the second function uploads a document or PDF file to an Amazon S3 bucket. These functions showcase the simplicity and power of AWS Lambda for handling common tasks in a serverless architecture. The project is ideal for learning how to create and deploy AWS Lambda functions and interact with AWS services like S3.

## Installation Instructions

### Prerequisites
Before you begin, ensure you have the following:
- An **AWS account**: You will need access to AWS services.
- **AWS CLI**: Optional, but useful for managing AWS resources from the command line.
- Basic knowledge of AWS Lambda and S3.

### Setting Up the AWS Lambda Functions
1. **Log in to the AWS Management Console**.
2. **Navigate to the Lambda service**.
3. **Create a new Lambda function** for each of the following:
   - **Add Two Numbers Function**:
     - Choose the runtime as **Python 3.x**.
     - Copy and paste the code from the "Add Two Numbers" section below.
   - **Upload Document to S3 Function**:
     - Choose the runtime as **Python 3.x**.
     - Copy and paste the code from the "Upload Document to S3" section below.

### Permissions
- For the **Upload Document to S3 Function**, ensure that the Lambda execution role has permissions to write to the specified S3 bucket. You can attach the `AmazonS3FullAccess` policy or create a custom policy with the necessary permissions.

## Usage Instructions

### Add Two Numbers Function
1. **Set up a test event** in the AWS Lambda console with the following JSON structure:
   ```json
   {
       "num1": 5,
       "num2": 10
   }
   ```
2. **Run the test** to see the output, which will return the sum of the two numbers.

### Upload Document to S3 Function
1. **Set up a test event** in the AWS Lambda console with the following JSON structure:
   ```json
   {
       "bucket_name": "your-s3-bucket-name",
       "file_name": "example.pdf",
       "file_content": "base64-encoded-content-here"
   }
   ```
   - Replace `"your-s3-bucket-name"` with the name of your S3 bucket.
   - Replace `"base64-encoded-content-here"` with the actual base64-encoded content of the PDF or document you want to upload.
2. **Run the test** to see the output, which will confirm the successful upload of the file.

## Features
- **Add Two Numbers Function**: A simple function that takes two numbers as input and returns their sum.
- **Upload Document to S3 Function**: A function that uploads a document or PDF file to an S3 bucket, demonstrating file handling in a serverless environment.
- **Serverless Architecture**: Both functions are designed to run in a serverless environment, showcasing the benefits of AWS Lambda.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Special thanks to the AWS community for their extensive documentation and support.
- Acknowledgment to [Your Mentor/Instructor Name] for guidance throughout the development of this project.


