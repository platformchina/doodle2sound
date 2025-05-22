# Doodle to Sound

A simple web application that converts your doodles into sound. Draw on the canvas using different colors and brush sizes, then click "Turn Drawing into Sound" to hear your creation.

## How it Works

*   **Drawing:** Use your mouse or touch to draw on the canvas.
    *   Select different colors from the palette. Each color corresponds to a different sound waveform (timbre).
    *   Adjust the brush size using the slider.
*   **Sound Generation:**
    *   The application "scans" your drawing from left to right.
    *   The **horizontal position (X-axis)** of your drawing determines *when* a sound is played.
    *   The **vertical position (Y-axis)** of your drawing determines the *pitch* of the sound (higher on the canvas means higher pitch).
    *   The **color** of your drawing determines the *timbre* (waveform) of the sound:
        *   Red: Sine wave
        *   Green: Square wave
        *   Blue: Sawtooth wave
        *   Yellow: Triangle wave
        *   Black: Sine wave (default)
*   **Controls:**
    *   **Color Brushes:** Select a color for drawing.
    *   **Brush Size:** Adjust the thickness of your lines.
    *   **Turn Drawing into Sound:** Plays back the audio representation of your doodle.
    *   **Clear Doodle:** Erases the canvas.

## Files

*   `index.html`: The main HTML structure of the application.
*   `style.css`:  Styles for the application's appearance.
*   `script.js`:  Contains all the JavaScript logic for drawing, UI interactions, and sound generation using the Web Audio API.

## How to Run Locally

1.  Clone this repository or download the files.
2.  Open `index.html` in your web browser.

## Deployment (Vercel Example)

This project consists of static HTML, CSS, and JavaScript files, making it very easy to deploy on platforms like Vercel, Netlify, or GitHub Pages.

**To deploy on Vercel:**

1.  **Push your code to a GitHub repository.**
2.  **Sign up or log in to Vercel (vercel.com).**
3.  **Import your GitHub repository:**
    *   Click "New Project".
    *   Connect your GitHub account if you haven't already.
    *   Select the repository containing this project.
4.  **Configure Project (Optional but usually not needed for static sites):**
    *   Vercel should automatically detect it as a static site.
    *   Framework Preset: Usually "Other" or it might auto-detect.
    *   Build Command: Not needed for this static setup.
    *   Output Directory: Not needed (or specify `.` if it asks).
    *   Install Command: Not needed.
5.  **Click "Deploy".**

Vercel will build and deploy your site, providing you with a unique URL.

## Features & Potential Improvements

*   **Current:**
    *   Canvas drawing with multiple colors and brush sizes.
    *   Sound generation based on X (time), Y (pitch), and color (timbre).
    *   Clear canvas functionality.
    *   Basic responsive design.
*   **Future Ideas:**
    *   More sophisticated sound mapping (e.g., line thickness to volume).
    *   Different "instruments" beyond basic waveforms.
    *   Saving/loading doodles.
    *   Real-time sound generation as you draw.
    *   More advanced audio effects (reverb, delay).
    *   Visual feedback during playback (e.g., a scanning line).

Enjoy doodling and making sounds!