# Victor Omondi's Blog

A personal data science blog built with [Quarto](https://quarto.org/), featuring posts on data analysis, data wrangling, statistical thinking, machine learning, and more.

🌐 **Live site:** [https://victoromondi1997.quarto.pub/blog/](https://victoromondi1997.quarto.pub/blog/)

---

## Table of Contents

- [About](#about)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Running Locally](#running-locally)
- [Adding a New Post](#adding-a-new-post)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

---

## About

This repository contains the source code for Victor Omondi's personal blog. Posts are written as Jupyter notebooks (`.ipynb`) or Quarto markdown (`.qmd`) files and rendered into a static website using Quarto.

---

## Prerequisites

Make sure you have the following installed before setting up the project:

- [Quarto](https://quarto.org/docs/get-started/) (v1.0 or later)
- [Python](https://www.python.org/downloads/) (v3.8 or later) — for Python-based notebooks
- [R](https://www.r-project.org/) — for R-based notebooks (optional)
- [Git](https://git-scm.com/)

---

## Getting Started

1. **Clone the repository:**

   ```bash
   git clone https://github.com/VictorOmondiCDS/blog.git
   cd blog
   ```

2. **Install Python dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Verify Quarto installation:**

   ```bash
   quarto check
   ```

---

## Running Locally

To preview the blog locally with live reload:

```bash
quarto preview
```

This will start a local development server (usually at `http://localhost:4848`) and open the blog in your browser.

To build the site without previewing:

```bash
quarto render
```

The rendered output is placed in the `docs/` directory.

---

## Adding a New Post

1. Create a new folder inside `posts/` named with the format `YYYY-MM-DD-your-post-title/` and add your content file (`.qmd` for Quarto markdown or `.ipynb` for Jupyter notebooks):

   ```
   posts/
   └── 2024-01-15-my-new-post/
       └── index.qmd      # or index.ipynb for a Jupyter notebook
   ```

2. Add a YAML front matter block at the top of your `.qmd` or `.ipynb` file. For example:

   ```yaml
   ---
   title: "My New Post"
   author: "Victor Omondi"
   date: "2024-01-15"
   categories: [python, data-analysis]
   image: "image.png"
   ---
   ```

3. Write your content below the front matter.

4. Preview your changes with `quarto preview` before committing.

---

## Project Structure

```
blog/
├── posts/              # Blog post source files (.qmd and .ipynb)
├── docs/               # Rendered static site output (auto-generated)
├── images/             # Shared images and media
├── _notebooks/         # Legacy notebooks (migrated to posts/)
├── _quarto.yml         # Quarto project configuration
├── index.qmd           # Blog home page
├── about.qmd           # About page
├── styles.css          # Custom CSS styles
├── requirements.txt    # Python dependencies
└── README.md           # This file
```

---

## Contributing

Contributions, suggestions, and bug reports are welcome! To contribute:

1. Fork the repository.
2. Create a new branch for your changes:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. Make your changes and commit them:

   ```bash
   git commit -m "feat: describe your change"
   ```

4. Push your branch and open a Pull Request.

Please follow the [Code of Conduct](CODE_OF_CONDUCT.md) in all interactions.

---

## License

This project is licensed under the terms of the [LICENSE](LICENSE) file included in this repository.
