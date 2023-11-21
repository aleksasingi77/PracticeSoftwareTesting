# PracticeSoftwareTesting

This README file will guide you to run the API tests in the command line with Newman.
----------------------------------------------------------------------------------------
# Prerequisites

1. **Intall NODE.js and npm:**
   Make sure you have Node.js and npm (Node Package Manager) installed on your machine.
   You can download and install them from the official website: https://nodejs.org/en.

2. **Install Newman:**
   Once Node.js and npm are installed, you can install Newman globally using the following
   command in your terminal or command prompt: npm install -g newman
   
----------------------------------------------------------------------------------------

# Running Tests with Newman:

1. **Clone the repository:**
   Clone the repository containing your Postman collection. If you don't have a Git
   repository, you can use the collection file directly.
   git clone https://github.com/your-username/your-repo.git
   
2. **Navigate to the Repository:**
   Change to the directory where your Postman collection is located.
   cd your-repo

3. **Export Environment Variables (If Needed):**
   If your collection relies on environment variables, export them using a file
   (e.g., environment.json).
   newman run Practice Software Testing.postman_collection.json --environment environment.json

4. **Run Newman:**
   Execute the following command to run your Postman collection using Newman.
   newman run Practice Software Testing.postman_collection.json

5. **Export Results:**
   newman run Practice Software Testing.postman_collection.json --reporters cli,junit --reporter-junit-export results.xml

# Notes:
  Ensure that the necessary dependencies are installed and the Postman collection is up-to-date.
  Review and update the command parameters based on your specific requirements.
