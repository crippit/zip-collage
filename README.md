Photo Collage Grid Builder

Try it out at [https://crippit.github.io/zip-collage/](https://crippit.github.io/zip-collage/)

An interactive, high-fidelity, and completely serverless client-side web application designed to turn bulk photo uploads into pixel-perfect, custom-designed collage grids. This application runs entirely in the browser, meaning your images never leave your device, ensuring maximum privacy and blazing-fast local processing.

🚀 Key Features

1. Dynamic Grid Layouts (Up to $25 \times 25$)

Highly Scalable: Customize your grid columns and rows dynamically from $5 \times 5$ up to $25 \times 25$.

Locked Proportions (1:1): Link columns and rows to force a perfectly symmetrical square-cell layout, or unlink them for free-form rectangular matrices.

Automatic Multi-Page Segmentation: Upload as many images as you want! The application automatically calculates and segments your photo library across multiple high-res canvas sheets, ensuring no photo gets left behind.

2. Multi-Format Aspect Ratio Outputs

Design layouts tailored directly for your target medium:

Square (1:1): Perfect for Instagram feeds ($1080 \times 1080 \text{ px}$).

Instagram Story (9:16): Tall, phone-optimized layout with centered, auto-scaled grids ($1080 \times 1920 \text{ px}$).

Widescreen (16:9): Optimized for desktop wallpapers, slide presentations, and landscape sharing ($1920 \times 1080 \text{ px}$).

3. Native HEIC/HEIF Browser Conversion

Seamless iPhone Uploads: No need to manually convert HEIC photos from your iOS device first.

On-The-Fly Processing: The app automatically detects HEIC files and converts them in the background to standard JPEGs in real-time, utilizing heic2any loaded dynamically via CDN.

4. Style & Visual Customization

Take control of every layout variable:

Grid Gap (Spacing): Adjust margins between photos from $0\text{px}$ up to $20\text{px}$.

Outer Borders/Margins: Toggle safe-zone margins ($4\%$). Disable them entirely to create seamless, edge-to-edge Full-Bleed designs.

Overall Image Blur: Apply adjustable blur filtering ($0\text{px}$ to $40\text{px}$) inside individual image borders—perfect for abstract artwork or structured design mockups.

Photo Corner Radius: Add elegant rounded corners to each grid image.

Crop vs. Fit (Aspect Strategies):

Crop & Fill (Cover): Fills the square cell completely by cropping edges.

Fit Whole Photo (Contain): Keeps your entire image visible, letterboxing empty space using your selected background color.

Custom Background Color: Pick any solid background hue using the built-in color picker or hex input.

5. Interactive Editing

Drag & Drop (Desktop): Drag any picture tile and drop it onto another cell to instantly swap their grid positions.

Tap-to-Swap (Mobile/Tablet): Click/tap an image cell, then click/tap another cell to effortlessly swap positions without drag-and-drop hardware constraints.

Quick Shuffle: Shuffle the sequence of your loaded photo set globally in one click to spark inspiration.

Selective Deletion: Hover over any populated cell and click the red delete cross ($\times$) to remove unwanted photos from the page slice.

🛠️ How to Run & Deploy

Since this tool is built as a single-page client-side utility using React, Tailwind CSS, and Babel via CDNs, there is zero local installation required.

Quick Start (Local Run)

Save the index.html file from this project to your local computer.

Double-click the file to open it in any web browser (Chrome, Safari, Edge, Firefox).

Start uploading photos!

Deploying to GitHub Pages (or Netlify / Vercel)

This app is fully optimized for free hosting on GitHub Pages:

Create a public repository on GitHub.

Upload index.html directly to the root of the repository.

Go to Settings > Pages in your GitHub repository.

Set the Source to deploy from the main or master branch.

Your custom collage builder will be live globally in less than a minute!

📁 Technical Architecture

Frontend Library: React 18 (loaded as UMD script for zero-install runtimes)

Compiler: Babel Standalone (transpiles JSX in the browser on the fly)

Styling: Tailwind CSS CDN (fluid, responsive slate-dark design tokens)

Icons: Optimized inline raw SVGs (highly performant and eliminates third-party script loading failures)

Image Conversion: heic2any (loads dynamically on-demand only when a HEIC file is detected)
