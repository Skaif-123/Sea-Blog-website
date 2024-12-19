![oceano blogs](https://github.com/user-attachments/assets/9796e5fc-c3ad-4b76-a1d4-d4cf87847e04)
# Responsive Blog Website using Grid

## Overview
This project is a responsive blog website created using HTML and CSS Grid. The website features a header and multiple blog cards showcasing various types of ships. Each card contains an image, title, description, author information, and an "Apply" button.

## Features
- **Responsive Design:** The website layout adapts to different screen sizes using CSS Grid.
- **Interactive Elements:** Hover effects are implemented on images, titles, and buttons for a better user experience.
- **Lazy Loading Images:** Images are optimized with the `loading="lazy"` attribute for faster page loading.
- **Semantic HTML:** Proper use of semantic elements like `<header>`, `<main>`, and `<div>` for improved accessibility.

## File Structure
```
project-folder/
|-- index.html
|-- style.css

    |-- Tanker.jpg
    |-- gas carrier.jpg
    |-- navy.jpeg
    |-- bulk carrier.jpg
    |-- container.jpeg
    |-- general cargo.jpeg
    |-- dredger.jpeg
    |-- PCC.jpeg
    |-- ship_icon.png
```

## How to Run the Project
1. Clone or download the project files.
2. Ensure all image files are present in the `images` folder.
3. Open `index.html` in any modern web browser.

## Usage
- The homepage displays a header section with the blog title and description.
- Each blog card includes:
  - A clickable image that links to relevant Wikipedia pages.
  - A title, description, and author details.
  - An "Apply" button styled with hover effects.

## Responsiveness
- The website adjusts its layout based on the screen size.
- The `grid-template-columns` property in the `.main_container` ensures that cards are displayed in a grid format, dynamically adjusting for available space.

## CSS Highlights
- **Grid Layout:** 
  ```css
  .main_container {
      display: grid;
      gap: 1.5rem;
      grid-template-columns: repeat(auto-fit, minmax(250px, 350px));
      justify-content: center;
      align-items: center;
  }
  ```
- **Hover Effects:**
  ```css
  .card_container:hover .card_image {
      transform: scale(1.1);
      transition-duration: 200ms;
  }

  .card_tag_container:hover {
      background-color: rgb(223, 102, 108);
      color: rgb(230, 230, 109);
      font-weight: bold;
      transition: ease;
  }
  ```

## Dependencies
- No external libraries or frameworks are used. The project relies solely on HTML and CSS.

## Future Enhancements
- Add JavaScript for more interactivity (e.g., filtering blog cards, dark mode toggle).
- Improve accessibility by adding ARIA labels and alt attributes for all images.
- Enhance styling with animations and transitions.

## Author
**Kaif Bhombal**

Feel free to contribute or suggest improvements!

