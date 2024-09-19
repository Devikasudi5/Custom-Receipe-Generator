# Custom-Receipe-Generator
Generates a receipe for a given set of ingredients and a fun-fact at the last.
# Project Overview:

The "Custom Recipe Generator" is a web application built with Flask and integrated with OpenAI's GPT-3.5-turbo model. The purpose of the application is to generate unique recipes based on user-provided ingredients.

# Key Components:

1.Backend Functionality:
a.Flask Web Framework: Used to create the web application and define routes.
b.OpenAI Integration: Utilizes OpenAI's GPT-3.5-turbo model to generate recipe tutorials.
The model is fed a list of available ingredients and produces a recipe along with a fun fact.
c.API Key Management: The OpenAI API key is securely managed using environment variables.

2.Front-End Features:
a.HTML Form: Allows users to input a list of ingredients.
b.Bootstrap: Used for styling the web page, making it visually appealing and responsive.
c.JavaScript Functions:
         c.1.generateTutorial: Fetches the generated recipe from the server and displays it.
         c.2.copyToClipboard: Copies the recipe text to the clipboard for easy sharing.
d.Routes and Functions:
      / (Home Route): Displays the HTML form for user input and handles form submissions. Upon submission, it triggers the generation of a recipe.
      /generate (Recipe Generation Route): Processes the user input, calls the generate_tutorial function, and returns the generated recipe.
      
3.Deployment:
The application is designed to run on 0.0.0.0 and port 8080, making it accessible from any IP address on port 8080.

How It Works:

User Input: Users enter a list of ingredients into the form.
Recipe Generation: When the form is submitted, the generateTutorial function sends the ingredient list to the backend.
OpenAI API: The backend uses OpenAI’s GPT-3.5-turbo model to create a recipe based on the provided ingredients.
Output Display: The generated recipe is displayed on the web page, and users can copy it to their clipboard using a button.
