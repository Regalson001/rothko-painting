# 🎨 Rothko Painting — CSS Art & Visual Design

A minimalist abstract painting recreated with **HTML5 and CSS3**, inspired by the expressive colour fields and geometric compositions associated with Mark Rothko's artwork.

This project demonstrates how fundamental CSS techniques—including the box model, spacing, shadows, border radius, transforms, and blur filters—can be combined to create an artistic composition entirely in the browser, without images, JavaScript, or external graphics libraries.

## 📌 Overview

**Rothko Painting** is a CSS art project that transforms simple HTML elements into an abstract painting displayed inside a traditional black frame.

The composition features a deep burgundy canvas with three rectangular colour fields in warm orange and red tones. Subtle rotations, blurred edges, rounded corners, and layered shadows give the shapes a softer, painterly appearance.

The project focuses on understanding how CSS controls not only the structure and layout of a webpage but also its visual character.

## ✨ Features

- **Pure HTML & CSS** — Created without JavaScript, image assets, or external libraries.
- **Classic framed presentation** — A thick black border and inner padding create the appearance of a physical picture frame.
- **Abstract colour composition** — Three layered rectangular shapes form the central artwork.
- **CSS blur effects** — The `filter: blur()` property softens the shapes and blends their edges.
- **Layered shadows** — The `box-shadow` property adds depth and a subtle glow around the colour fields.
- **Organic shapes** — Different `border-radius` values soften the geometric forms.
- **Slight rotations** — The `transform: rotate()` property introduces subtle irregularity.
- **Precise spacing and alignment** — Margins, padding, widths, and heights control the composition.
- **Clean HTML structure** — Separate elements represent the frame, canvas, and individual colour fields.

## 🖼️ Artwork Structure

The composition is built from four main layers:

| Element | Purpose |
|---|---|
| `.frame` | Creates the outer black frame and surrounding space. |
| `.canvas` | Defines the painting's background, dimensions, and overall blur effect. |
| `.one` | Creates the upper orange colour field. |
| `.two` | Creates the middle dark-red colour field. |
| `.three` | Creates the lower red colour field with irregular rounded corners. |

Each colour field is an ordinary HTML `<div>` styled with CSS. Together, these elements form the complete artwork.

## 🛠️ Technologies Used

| Technology | Application |
|---|---|
| HTML5 | Structures the frame, canvas, and colour fields. |
| CSS3 | Controls layout, colours, shapes, and visual effects. |
| CSS Box Model | Manages element dimensions, borders, padding, and margins. |
| CSS Transforms | Applies subtle rotations to the artwork's shapes. |
| CSS Filters | Creates soft edges using blur effects. |
| CSS Box Shadows | Adds depth and a painterly glow. |
| CSS Border Radius | Produces rounded and irregular corners. |

## 📚 CSS Concepts Practised

### 1. The CSS Box Model

The `.frame` combines a thick border, internal padding, a defined width, and automatic horizontal margins.

```css
.frame {
  border: 50px solid black;
  width: 500px;
  padding: 50px;
  margin: 20px auto;
}
```

This demonstrates how borders, padding, and margins influence the total space an element occupies.

### 2. Background Colours

Different colour values establish contrast between the canvas and the individual colour fields.

```css
.canvas {
  background-color: #4d0f00;
}

.one {
  background-color: #efb762;
}

.two {
  background-color: #8f0401;
}

.three {
  background-color: #b20403;
}
```

### 3. Blur Filters

The `filter: blur()` property softens edges and creates a less rigid appearance.

```css
.canvas {
  filter: blur(2px);
}
```

Individual shapes also use blur filters to introduce additional softness.

### 4. Box Shadows

The `box-shadow` property adds subtle shadows around the colour fields, helping the shapes blend into the canvas.

```css
.one {
  box-shadow: 0 0 3px 3px #efb762;
}
```

### 5. Border Radius

Different corner radii create variation in the shapes instead of leaving every rectangle perfectly square.

```css
.three {
  border-radius: 30px 25px 60px 12px;
}
```

### 6. CSS Transforms

Small rotations introduce subtle imperfections that make the composition feel more organic.

```css
.two {
  transform: rotate(0.4deg);
}
```

### 7. Layout and Alignment

Fixed dimensions establish the canvas and colour fields, while automatic horizontal margins centre the composition's elements.

```css
.one {
  width: 425px;
  margin: 20px auto;
}
```

## 📁 Project Structure

```text
Rothko-Painting/
├── index.html
├── styles.css
└── README.md
```

- **`index.html`** — Contains the semantic document foundation and the HTML elements that form the artwork.
- **`styles.css`** — Contains the styles for the frame, canvas, colours, spacing, and visual effects.
- **`README.md`** — Documents the project, technologies, and implementation.

## 🚀 Getting Started

Follow these steps to run the project locally.

### Prerequisites

You need:

- A modern web browser.
- A code editor, such as Visual Studio Code.
- Git installed on your computer if you want to clone the repository.

### 1. Clone the Repository

Replace the example repository URL below with your actual GitHub repository URL.

```bash
git clone https://github.com/Regalson001/Rothko-Painting.git
```

### 2. Open the Project Folder

```bash
cd Rothko-Painting
```

### 3. Open the Project

Open `index.html` directly in your browser, or open the project folder in Visual Studio Code and use the Live Server extension if you have it installed.

The artwork will render in the browser using the styles defined in `styles.css`.

## 🌐 Live Demo

**Explore the live project:** Add your published GitHub Pages URL here after deploying the project.

For a repository named `Rothko-Painting`, the expected GitHub Pages URL is:

`https://regalson001.github.io/Rothko-Painting/`

This URL will work once GitHub Pages has been enabled and the project has been successfully published.

## 📱 Responsive Design

The current implementation uses fixed pixel dimensions for the frame and canvas. It is primarily designed around a fixed-size composition.

Although the artwork can render in modern browsers, the current layout is **not fully responsive on narrow screens** and may cause horizontal overflow on mobile devices.

Potential improvements include:

- Using `max-width` to constrain the canvas to the available screen width.
- Applying responsive dimensions to the frame and canvas.
- Adjusting frame borders and padding for smaller screens.
- Testing the composition at different viewport widths.

These improvements would preserve the artwork's appearance while making it more adaptable to different devices.

## ♿ Accessibility Considerations

The project uses a straightforward HTML structure and does not rely on JavaScript or interactive controls.

Possible improvements include:

- Adding a descriptive `<meta name="viewport">` tag for mobile browsers.
- Providing a meaningful page description.
- Considering an accessible description of the artwork if it is presented as part of a larger gallery or portfolio.
- Testing the page with browser zoom and different viewport sizes.

Because the artwork is created entirely from styled `<div>` elements, consider adding a suitable textual description if the painting itself communicates important information.

## 🎯 Learning Objectives

This project was created to practise and reinforce:

- Understanding the relationship between HTML structure and CSS presentation.
- Applying the CSS box model to control dimensions and spacing.
- Positioning and aligning elements with margins.
- Working with background colours and colour contrast.
- Using blur filters and box shadows to create visual depth.
- Applying border radii to modify geometric shapes.
- Using transforms to rotate elements.
- Separating HTML structure from CSS styling.
- Understanding the difference between fixed-size layouts and responsive designs.

## 🔮 Future Improvements

Possible enhancements for future iterations include:

- [ ] Make the artwork responsive across desktop, tablet, and mobile screens.
- [ ] Add a viewport meta tag and page description.
- [ ] Refine the colour palette and shadow effects.
- [ ] Experiment with gradients and layered blur effects.
- [ ] Add a subtle background around the framed artwork.
- [ ] Improve the overall presentation for a front-end portfolio.
- [ ] Publish the project using GitHub Pages.

## 👨‍💻 Author

**Stephen Oyugi**

Front-End Developer in Training | HTML5 & CSS3

Passionate about building clean, responsive, and accessible web experiences while developing practical skills in semantic HTML, modern CSS, and user-focused design.

- **GitHub:** [@Regalson001](https://github.com/Regalson001)
- **Repository:** [Rothko Painting](https://github.com/Regalson001/Rothko-Painting)

## 📄 License

This project is available for educational and portfolio purposes.

If you would like to distribute or reuse the project under a specific open-source license, consider adding a `LICENSE` file to the repository. For example, the MIT License is a common choice for open-source projects.

---

<p align="center">
  Built with HTML5 and CSS3.
  <br>
  <strong>Exploring the creative possibilities of CSS, one shape at a time.</strong>
</p>
