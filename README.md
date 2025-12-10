# 3-Column Preview Card (Vanilla Web)

A clean, responsive 3-Column Preview Card component built using vanilla HTML and CSS.

![3-Column Preview Card](./images/active-states.jpg)

## Key Features & Benefits

- **Clean and Simple:** Built using only vanilla HTML and CSS for a lightweight, dependency-free component.
- **Responsive Design:** Mobile-first approach with optimized layouts for both mobile and desktop viewports.
- **Smooth Interactions:** GPU-accelerated hover animations with opacity and transform effects for a polished feel.
- **Accessible:** Semantic HTML structure with proper ARIA and keyboard-navigable links.
- **Easy to Integrate:** Drop the `index.html`, `style.css`, and the `images/` folder into any project—no build step required.
- **Customizable:** Simple class structure lets you change copy, images, and styles quickly.

## Prerequisites & Dependencies

- A web browser (Chrome, Firefox, Safari, Edge) to view the component.
- A text editor or IDE to edit `index.html` and `style.css` (e.g., VS Code).
- (Optional) A local server for consistent asset loading (VS Code Live Server).

## Installation & Setup Instructions

1. **Clone or download the repository** (or copy the project folder locally):

```bash
git clone https://github.com/syntaxSangoma/three-column-preview-card-vanilla-08
```

```bash
cd three-column-preview-card-vanilla-08
```

2. **Open the project** in your editor and open `index.html` in the browser:

- Double-click `index.html` or open it from your editor.
- Or serve the folder using a simple local server (recommended for consistent image loading)

## Usage Examples

The component is a vehicle category showcase template. To customize, edit `index.html`:

- Replace the category icons at `./images/icon-sedans.svg`, `./images/icon-suvs.svg`, and `./images/icon-luxury.svg` with your own icons.
- Update the category titles in the `.three-column-card__title` sections (currently "Sedans", "suvs", "luxury").
- Change the category descriptions in the `.three-column-card__description` markup.
- Update the button text in the `.three-column-card__button` elements.

Example: to update the Sedans title and description, find the first section and replace the content:

```html
<section class="three-column-card__sub-card three-column-card__sub-card--sedans">
  <figure class="three-column-card__icon">
    <img src="./images/icon-sedans.svg" alt="icon-sedans" width="64" height="40">
    <figcaption class="offscreen">icon-sedans</figcaption>
  </figure>

  <h1 class="three-column-card__title">
    Sedans  <!-- Update this -->
  </h1>

  <p class="three-column-card__description">
    Choose a sedan for its affordability and excellent fuel economy. Ideal for cruising in the city or on
    your next road trip.  <!-- Update this -->
  </p>

  <a href="#" class="three-column-card__button three-column-card__button--sedans nowrap center">
    Learn More  <!-- Update this -->
  </a>
</section>
```

## Configuration Options

Most visual changes live in `style.css`. Typical customizations:

- **Colors & Palette:** Edit CSS custom properties (variables) at the top of `style.css` under `:root`:
  - `--SEDANS-BG`, `--SUVS-BG`, `--LUXURY-BG` for category background colors
  - `--BUTTON-BG` for button background color
  - `--TITLE-CLR` and `--DESCRIPTION-CLR` for text colors
  
- **Typography:** Change the `--FF1` and `--FF2` font imports or replace with different Google Fonts in the `@import` statement.

- **Card Size & Spacing:** Adjust `.three-column-card` width, padding, and inner element dimensions to fit your layout.

- **Animations & Hover Effects:** Modify transition durations and effects in the `@media (min-width: 992px)` section:
  - Change `0.5s` to adjust animation speed
  - Replace `ease` with `cubic-bezier(...)` for custom easing curves
  - Adjust the hover state properties (color, outline, background)

- **Responsive Breakpoints:** The mobile design applies by default; desktop styles activate at `992px` and above. Adjust this breakpoint to match your needs.

## Contributing Guidelines

Contributions are welcome. Suggested flow:

1. Fork the repository.
2. Create a feature branch (e.g., `feature/dark-mode`, `feature/new-category`).
3. Make changes with focused commits.
4. Push to your fork and open a pull request describing your changes.

## License

License not specified.

## Acknowledgments

- Google Fonts for the `Big Shoulders` and `Lexend Deca` font families used in this project.