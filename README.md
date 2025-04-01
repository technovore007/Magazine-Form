# Magazine Subscription Form

A modern, responsive multi-step form for magazine subscriptions with dark mode support.

## 🚀 Features

- **Multi-step form** with progress tracking
- **Responsive design** for all device sizes
- **Dark/Light mode** with user preference persistence
- **Form validation** with error messages
- **Order summary** on submission
- **Clean modern UI** with smooth transitions

## 📋 Form Sections

1. **Personal Information**
   - First name
   - Last name

2. **Address Information**
   - Street address
   - City
   - State
   - Zip code

3. **Subscription Details**
   - Magazine selection
   - Subscription length (1 or 2 years)
   - Additional comments

## 🎨 UI Components

- Progress bar with step indicators
- Theme toggle switch with emoji indicators (☀️/🌙)
- Validation error messages
- Responsive form layout
- Success message with order summary

## 💻 Technologies Used

- HTML5
- CSS3 (with CSS variables for theming)
- Vanilla JavaScript
- Local Storage API for theme preference

## 📱 Responsive Design

The form is fully responsive and adapts to different screen sizes:
- Desktop: Full two-column layout
- Mobile: Single column layout with optimized spacing

## 🌓 Dark Mode Implementation

The site implements a dark/light theme toggle that:
- Uses CSS variables for seamless transitions
- Persists user preference in local storage
- Adjusts colors, shadows, and backgrounds automatically

## 📁 Project Structure

```
magazine-subscription/
├── index.html         # Main HTML structure
├── styles.css         # Styling with CSS variables
├── script.js          # Form validation and functionality
└── preview.png        # Project preview image
```

## 🖥️ Setup and Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/username/magazine-subscription.git
   ```

2. Open `index.html` in your browser or use a local development server.

## 🧩 Code Features

### CSS Variables for Theming

```css
:root {
  --primary-color: #4a6cf7;
  --secondary-color: #6c757d;
  /* Other variables */
}

[data-theme="dark"] {
  --primary-color: #6d8cff;
  --secondary-color: #adb5bd;
  /* Dark theme variables */
}
```

### Multi-Step Form Navigation

```javascript
function showSection(index) {
  sections.forEach((section, i) => {
    if (i === index) {
      section.style.display = 'block';
    } else {
      section.style.display = 'none';
    }
  });
  
  currentSection = index;
  updateProgress();
}
```

### Form Validation

```javascript
function validateSection(sectionIndex) {
  let isValid = true;
  
  // Validation logic for each section
  // ...
  
  return isValid;
}
```

## 📝 Future Enhancements

- Email verification step
- Payment processing integration
- Magazine cover previews
- Subscription pricing details
- Animation transitions between form steps

## 📄 License

This project is available for educational purposes. Feel free to use it as a learning resource.

## 🙏 Acknowledgements

- Created for educational purposes
- Inspired by modern web design principles
- Built with accessibility in mind
