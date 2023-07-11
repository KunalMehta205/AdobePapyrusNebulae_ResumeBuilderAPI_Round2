# AdobePapyrusNebulae_ResumeBuilderAPI_Round2
Resume Builder API is a tool that allows users to create professional resumes quickly and easily. The API uses pre-built templates and dynamically generates the resume content based on the user's input data.

This is a Resume Builder Application that takes input from the user through a Webpage or Curl request, processes it and generates a Resume in `.pdf` format using the Adobe Document Generation API.

# Installation and Setup
1. Clone the repository in your local machine
2. After cloning the repository, install all the dependencies using:
   ```
   npm install
   ```
3. Set up the environment variables using (for Windows):
   ```
   set PDF_SERVICES_CLIENT_ID=<YOUR CLIENT ID>
   set PDF_SERVICES_CLIENT_SECRET=<YOUR CLIENT SECRET>
   ```
# Executing the Project
## Method 1: Using Resume UI
Run the following command in your terminal
```
npm start
```
This will start a server at `localhost:8080/resume` , go to the server.

You will see three different formats of resume to choose from.
Select one of the format, fill your details in the form and click on Submit.

Wait for few seconds while your API keys are being verified by Adobe's servers and the PDF is being generated.

The final Resume will be present in the `output` directory.

## Method 2: Resume Builder API
`app.js` provides the primary API endpoint, which can handle requests using various methods such as HTTP GET requests and Curl requests.

Run the following command in your terminal
```
npm start
```
This will input a curl request in another terminal window, port set at localhost:8080/resume, and will directly output a `.pdf` file inside the output directory.

The final Resume will be present in the `output` directory.

# Project Structure
`templates` - contains .docx files of sample templates. <br><br>
`static` - contains images, .js and .css files for UI component of the project. <br><br>
`views` - contains .ejs files <br><br>
`src` - contains modularized code files <br><br>
`sampleoutput` - stores some sample generated resumes. <br><br>
`output` - stores all the generated resumes
