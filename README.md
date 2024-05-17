# Medical Image Generation: Using Fine-Tuned CLIP Model with Stable Diffusion

## Project Overview

Script2Skin is a deep learning project designed to generate synthetic images of skin rashes based on textual descriptions. The project aims to provide educational and diagnostic tools by creating high-fidelity images that vary by rash type, skin color, and affected area.

The motivation behind SkinRashGenerator is to assist medical professionals, educators, and students by providing a tool that can generate realistic images of skin rashes. This can be particularly useful in scenarios where visual examples are needed for training or diagnostic purposes but real-life examples are unavailable or difficult to obtain.

Using advanced AI techniques such as CLIP (Contrastive Language-Image Pre-training) and latent diffusion models, our system can interpret textual descriptions and produce corresponding images. This allows for a high degree of customization, enabling users to specify the type of rash, the skin color, and the location on the body.

For example, a command might be: "Generate a few images of a eczema type of rash at the back of the neck area on fair skin." The system will process this input and generate images that match the given description, providing valuable visual aids for various applications.

## Objective

To develop a generative model capable of producing detailed images of common skin rashes, customizable by type, skin tone, and body area, for use in educational and diagnostic settings.

## Key Features

<b> Text-to-Image Generation:</b> Create images from textual descriptions specifying rash type, skin color, and affected area.<br>
<b>Customizable Parameters:</b> Generate images based on various factors including rash type (e.g., eczema, ringworm), skin color (e.g., fair, brown), and affected body area (e.g., chest, neck).

## Technologies Used
- Python
- CLIP (Contrastive Language-Image Pre-training)
- Latent Diffusion Model

## Example Commands
Use the following example commands to generate images:

"Generate a eczema rash on fair skin at the neck area."
"Show acne on brown skin on the hand."

## Project Approach
<b>Initial Approach</b><br>
We began by training the OpenAI CLIP model with our dataset using a straightforward method. The model performed well in predicting image captions. However, integrating this trained CLIP model with the stable diffusion model led to compatibility issues and multiple errors.

<img width="682" alt="Screen Shot 2024-04-24 at 1 04 43 AM" src="https://github.com/jhalak1509/Medical_Image_Generation/assets/114832299/c3391370-9c21-45a3-8440-62c658a3be8d">


<b>Revised Approach</b><br>
To overcome the initial challenges, we utilized a script from Hugging Face to fine-tune the CLIP model, which we then integrated with stable diffusion. This improved approach resolved compatibility issues but did not produce optimal image quality due to hardware limitations, preventing extensive training.

## Challenges and Future Enhancements
<b>Challenges</b><br>
- Compatibility Issues: Initial difficulties in integrating the fine-tuned CLIP model with the stable diffusion model.
- Hardware Limitations: Limited computational resources impacted our ability to fully train and optimize the model.

<b>Future Enhancements</b><br>
- Infrastructure: Acquire better hardware to address resource constraints.
- Optimization: Improve model efficiency and performance.
- Dataset Expansion: Enhance the dataset for improved accuracy and versatility.


