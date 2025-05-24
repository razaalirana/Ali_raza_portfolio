# 🚀 Building a Portfolio using mkdocs

We will use mkdocs to build a portfolio website. This is a simple and easy way to create a static website using markdown files. We will use the following steps to create the portfolio:

📖 Link to the mkdocs documentation is [here](https://www.mkdocs.org/getting-started/).

## 1️⃣ Install mkdocs using pip

```bash
conda create -n mkdocs python=3.12 -y
conda activate mkdocs
pip install mkdocs mkdocs-material mkdocstrings[python] mkdocs-jupyter mkdocs-git-revision-date-localized-plugin pymdown-extensions
```

## 2️⃣ Create a new mkdocs project

```bash
mkdocs new my-portfolio
cd my-portfolio
```

## 🗂️ Project Structure

Your project should look like this:

```
my-portfolio/
├── mkdocs.yml
├── docs/
│   ├── index.md
│   ├── resume.md
│   ├── certifications.md
│   ├── contact.md
│   ├── education.md
│   ├── experience.md
│   ├── projects.md
│   ├── publications.md
│   ├── references.md
│   ├── skills.md
│   ├── image/
│   │   └── profile.jpg
│   └── ...
└── ...
```

## 3️⃣ Run the mkdocs server

```bash
mkdocs serve
```

> 💡 You can also specify the port using the `-a` option. For example, to run the server on port 8501, use the following command:

```bash
mkdocs serve -a 127.0.0.1:8501
```

## 4️⃣ Build the mkdocs project

```bash
mkdocs build
```

## 5️⃣ Deploying Your Portfolio

You can deploy your static site to GitHub Pages or any static hosting provider. For GitHub Pages:

```bash
git init
git remote add origin <your-repo-url>
git add .
git commit -m "Initial commit"
git push -u origin main
mkdocs gh-deploy
```

## 6️⃣ Customization

- 🖌️ Update `mkdocs.yml` to change site name, logo, navigation, and theme options.
- 🖼️ Add your profile image to `docs/image/profile.jpg` and update the logo path in `mkdocs.yml`.
- 📝 Edit markdown files in `docs/` to update your content (resume, certifications, contact, etc).

## 🔗 Useful Links

- [MkDocs Material Theme](https://squidfunk.github.io/mkdocs-material/)
- [MkDocs Plugins](https://github.com/mkdocs/catalog)

---

**📚 Portfolio Sections:**

- 🏠 Home (index.md)
- 📄 Resume (resume.md)
- 🏅 Certifications (certifications.md)
- 📬 Contact (contact.md)
- 🎓 Education (education.md)
- 💼 Experience (experience.md)
- 🗃️ Projects (projects.md)
- 📝 Publications (publications.md)
- 📝 References (references.md)
- 🧰 Skills (skills.md)

---

❓ For any issues, refer to the official MkDocs documentation or the Material for MkDocs theme docs.
