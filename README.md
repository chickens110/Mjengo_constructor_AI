# Mjengo_constructor_AI
Building Design Agent
Project Goal
The goal of this project is to create an interactive agent that allows users to describe their desired building design through various input methods (text, voice, or drawing) and then generates a visual representation (drawing) of that building. The agent should also support iterative refinement based on user feedback.

Implemented Features
1. Handle User Input (Text)

A function get_user_building_description is implemented to handle text input from the user using the input() function.
Placeholders for voice and drawing input are included to indicate future development areas.
2. Process User Input (Text)

The analyze_building_description function processes text input.
It uses basic keyword matching and regular expressions to extract key building characteristics such as type, number of floors, style, materials, and features.
The extracted characteristics are stored in a dictionary.
An outline for handling drawing input analysis is included as a placeholder.
3. Generate Building Drawing

The create_building_drawing function utilizes the PIL (Pillow) library to generate a simple drawing of a building based on the analyzed characteristics.
It can represent basic building structure, floors, windows, and some specific features like balconies and large windows.
The drawing is returned as a PIL Image object.
4. Display Drawing

The generated PIL Image object is displayed within the notebook using IPython.display.display.
5. Iterate and Refine

A basic iterative refinement loop is implemented.
The get_user_feedback function prompts the user for feedback.
The update_characteristics_from_feedback function attempts to update the building characteristics based on simple text feedback.
The drawing is regenerated and displayed after each refinement step.
How to Use
Run the notebook cells sequentially.
When prompted, enter your building description as text.
The agent will generate and display a drawing based on your description.
You will then be asked if you want to refine the drawing. Enter "yes" or "no".
If you enter "yes", provide your feedback as text (e.g., "add a floor", "change material to brick").
The agent will attempt to update the drawing based on your feedback and display the refined version.
Continue providing feedback or enter "no" to stop the refinement process.
Future Enhancements
Voice Input: Implement speech-to-text functionality to process voice descriptions.
Drawing Input: Integrate image processing and computer vision techniques to analyze building drawings.
Advanced NLP: Enhance the natural language processing capabilities to understand more complex and nuanced building descriptions and feedback.
More Sophisticated Drawing Generation: Improve the drawing generation to create more detailed, realistic, and varied building representations. Explore using more advanced graphics libraries or even generative models for image creation.
Error Handling: Add more robust error handling for invalid inputs and unexpected feedback.
User Interface: Develop a more user-friendly interface for interacting with the agent, potentially outside of the notebook environment.
