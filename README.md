# Text-Editor

### Features

- File Management: 
  - Retrieve a list of files from the server.
  - Load and display content of selected files.
  - Save changes to the existing files.
  - Save content as a new file with a different name, ensuring no duplicate file names.
  
- Text Editing:
  - Simple and intuitive text editor with an easy-to-use interface.
  - Real-time editing with options to save or save as a new file.

- User Interface:
  - Minimalistic and clean design with sky-blue background for a pleasing visual experience.
  - Yellow buttons for actions to ensure clarity and visibility.
  - Centralized form layout to focus user attention on text editing tasks.

### Installation and Run Instructions

1. Clone the Repository
2. Set Up the Server:
   - Ensure you have a web server (like IIS or any ASP.NET compatible server) installed.
   - Copy the project files to the server's root directory.
3. Run the Application:
   - Open your web browser.
   - Navigate to the server URL where you hosted the application (e.g., `http://localhost/A06-Text-Editor`).
4. Usage:
   - Select a file from the dropdown to load its content into the text editor.
   - Edit the content as needed.
   - Click `Save` to save changes to the current file or `Save As` to save the content as a new file.


### Interesting Parts during the Build Process

- Integration of jQuery and ASP.NET:
  - Utilizing jQuery for AJAX requests made the interaction between the client-side and server-side seamless.
  - Learning how to serialize and deserialize data efficiently using JSON for smooth communication between the front-end and back-end.

- Dynamic UI Updates:
  - Implementing real-time updates to the file list and editor content without page refresh was an exciting challenge.
  - Ensuring a responsive and user-friendly interface that adapts to user interactions dynamically.


### Difficulties Faced and Solutions
- File Name Validation:
  - Challenge: Implementing validation to prevent saving files with duplicate names.
  - Solution: Added a simple check in the `saveAsContent` function to verify if the new file name already exists before proceeding with the save operation. This was implemented using jQuery to search the file list dropdown for existing names.

- Error Handling:
  - Challenge: Providing meaningful feedback to users when errors occurred (e.g., file saving issues).
  - Solution: Implemented detailed error handling in both JavaScript and C# code. Used `alert` for user-friendly error messages and console logging for developer insights during debugging.


### Screenshots:
<img src="https://github.com/shubhhh19/Text-Editor/assets/126296317/d01cea6a-2660-49cc-990c-5f4ef4fd0d35" width="700" height="400">
<img src="https://github.com/shubhhh19/Text-Editor/assets/126296317/67cc5133-71d2-44d6-8166-53dc21145446" width="700" height="400">
