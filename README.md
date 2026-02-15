# Ashish Pakki - Portfolio Website

A modern, dynamic portfolio website showcasing my work as a Backend Engineer specializing in scalable data systems and production-grade ETL pipelines.

![Portfolio Preview](![portfolio 1](https://github.com/user-attachments/assets/23e70159-8600-4587-8511-3ce022e95f5b)
)

## 🚀 Features

- **Dynamic Animated Background** - Interactive particle system with floating orbs
- **Smooth Animations** - Fade-in effects and hover interactions throughout
- **Responsive Design** - Fully optimized for mobile, tablet, and desktop
- **Sections:**
  - Hero with professional photo and key metrics
  - About Me with personal story, education, family, and friends
  - Experience timeline
  - Featured projects
  - Technical skills organized by category
  - Contact information

## 🛠️ Tech Stack

- **React 18** - Modern React with hooks
- **Vite** - Fast build tool and dev server
- **Tailwind CSS** - Utility-first CSS framework
- **Lucide React** - Beautiful icon library

## 📦 Installation

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ashish-portfolio.git
   cd ashish-portfolio
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173`

## 🏗️ Build for Production

```bash
npm run build
# or
yarn build
```

The optimized production files will be in the `dist` folder.

## 🌐 Deployment

### Deploy to GitHub Pages

1. **Install gh-pages**
   ```bash
   npm install --save-dev gh-pages
   ```

2. **Add to package.json scripts**
   ```json
   "scripts": {
     "predeploy": "npm run build",
     "deploy": "gh-pages -d dist"
   }
   ```

3. **Deploy**
   ```bash
   npm run deploy
   ```

### Deploy to Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel`
3. Follow the prompts

### Deploy to Netlify

1. Build the project: `npm run build`
2. Drag and drop the `dist` folder to [Netlify](https://app.netlify.com/drop)

## 📁 Project Structure

```
ashish-portfolio/
├── public/
│   └── ashish-photo.jpeg      # Profile photo
├── src/
│   ├── App.jsx                # Main portfolio component
│   ├── index.css              # Global styles with Tailwind
│   └── main.jsx               # React entry point
├── index.html                 # HTML template
├── package.json               # Dependencies and scripts
├── vite.config.js             # Vite configuration
├── tailwind.config.js         # Tailwind configuration
└── README.md                  # This file
```

## 🎨 Customization

### Update Personal Information

Edit `src/App.jsx` and update:
- Personal details in the hero section
- Experience data in the `experiences` array
- Projects in the `projects` array
- Skills in the `skills` object
- About me content
- Contact links

### Change Colors

Modify the color scheme by updating the gradient colors in `src/App.jsx`:
- `emerald-400` / `emerald-500` - Primary accent color
- `cyan-400` / `cyan-500` - Secondary accent color

### Replace Photo

Replace `public/ashish-photo.jpeg` with your own photo (recommended size: 400x500px)

## 📱 Responsive Design

The portfolio is fully responsive with breakpoints:
- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px

## 🔧 Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build locally

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contact

- **Email:** princeofpakki@gmail.com
- **LinkedIn:** [linkedin.com/in/ashish-pakki-29a2b8259](https://www.linkedin.com/in/ashish-pakki-29a2b8259)

---

**Designed & Built by Ashish Pakki © 2025**
