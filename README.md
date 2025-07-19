# DemoAgent
# Modern AI Widget Webpage

A sleek, modern webpage with a centered GIF, heading, paragraph, and a call-to-action button that triggers the Omnidimension AI widget on click. Built with Tailwind CSS for styling and vanilla JavaScript for dynamic widget loading, the page features smooth animations and hover effects for an enhanced UI/UX.

## Features
- **Centered GIF**: Displays a visually appealing GIF at the top of the page.
- **Heading and Paragraph**: Clean, readable text to introduce the AI widget.
- **Call-to-Action Button**: A stylish button with hover effects (glow and scale) that loads the Omnidimension AI widget when clicked.
- **Animations**: Fade-in-up animations for all elements with staggered delays for a smooth entrance.
- **Responsive Design**: Fully responsive layout, optimized for mobile, tablet, and desktop screens.
- **Dynamic Widget Loading**: The Omnidimension widget script loads only when the button is clicked, improving page performance.

## Demo
[https://sudarshanbadli.github.io/DemoAgent/]

## Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge, etc.).
- Internet connection to load the Tailwind CSS CDN and the Omnidimension widget script.
- A valid Omnidimension `secret_key` for the widget.

## Installation
1. **Clone or Download the Repository**:
   ```bash
   git clone github.com/Sudarshanbadli/DemoAgent/
   ```
   Alternatively, download the `index.html` file directly.

2. **Open the Page**:
   - Open `index.html` in a web browser to view the page locally.
   - No additional dependencies are required since Tailwind CSS is included via CDN.

3. **Host the Page (Optional)**:
   - Deploy the `index.html` file to a web server or hosting platform (e.g., Netlify, Vercel, GitHub Pages) for public access.
   - Example for Netlify:
     1. Drag and drop the project folder into Netlify's dashboard.
     2. Deploy the site and get a live URL.

## Usage
1. Open the webpage in a browser.
2. The page displays a centered GIF, a heading, a paragraph, and a "Start AI Chat" button.
3. Click the button to load the Omnidimension AI widget.
4. The button text changes to "AI Chat Loading..." while the widget loads and updates to "Chat Now" once loaded.

## File Structure
```
├── index.html       # Main webpage file
├── README.md        # This file
```

## Customization
To tailor the webpage to your needs, modify the following in `index.html`:

- **GIF**:
  - Replace the GIF URL in the `<img>` tag:
    ```html
    <img src="https://media.giphy.com/media/3o7bu3XilJ5BOiSGic/giphy.gif" alt="AI Animation" ...>
    ```
    - Use a GIF that aligns with your branding (recommended size: 256x256 pixels).

- **Text Content**:
  - Update the heading and paragraph:
    ```html
    <h1>Connect with Our AI Agent</h1>
    <p>Experience seamless interaction with our advanced AI...</p>
    ```
    - Replace with your brand name or specific messaging.

- **Colors**:
  - Modify Tailwind CSS classes for the background (`bg-gray-900`), button (`bg-blue-600`, `hover:bg-blue-700`), or text (`text-gray-300`).
  - Example: Change the button color to green:
    ```html
    <button class="btn-glow bg-green-600 ... hover:bg-green-700 ...">
    ```

- **Button Behavior**:
  - Adjust the button text or states in the JavaScript:
    ```javascript
    triggerButton.textContent = 'Chat Now';
    ```
  - Add toggling logic if the Omnidimension widget supports opening/closing.

- **Widget Configuration**:
  - Ensure the Omnidimension `secret_key` is valid:
    ```javascript
    script.src = 'https://backend.omnidim.io/web_widget.js?secret_key=e238eafd81e935ba1657525abff017da';
    ```
  - If the widget requires a specific container ID or initialization function, update the JavaScript accordingly.

- **Animations**:
  - Modify the `fadeInUp` animation in the `<style>` section for different effects or durations.
  - Adjust animation delays (e.g., `style="animation-delay: 0.2s;"`) for timing.

## Dependencies
- **Tailwind CSS**: Included via CDN (`https://cdn.tailwindcss.com`).
- **Omnidimension Widget**: Loaded dynamically from `https://backend.omnidim.io/web_widget.js`.
- No local dependencies or build tools are required.

## Notes
- **Widget Loading**: The Omnidimension widget loads only when the button is clicked to optimize page performance. Verify the `secret_key` is correct to avoid loading issues.
- **Production Optimization**:
  - For production, consider installing Tailwind CSS locally and building a minified CSS file to reduce load times.
  - Host the GIF on a CDN for faster loading.
- **Troubleshooting**:
  - If the widget doesn’t load, check the browser console for errors related to the Omnidimension script.
  - Ensure an active internet connection for CDN and widget script loading.

## Contributing
Feel free to fork this repository, make improvements, and submit pull requests. Suggestions for UI enhancements, additional animations, or widget integration improvements are welcome!

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For questions or support, contact [sudarshanbadli7@gmail.com] or open an issue in the repository.
