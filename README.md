# Portfolio site setup

## 1. Create the repo
On GitHub, create a new repository named exactly:

```
yourusername.github.io
```

Replace `yourusername` with your actual GitHub username (e.g. `Levine123.github.io`). This exact name is what makes GitHub automatically host it as your main site instead of a project subpage.

## 2. Add the files
Add `index.html` **and** the `images` folder (with all five .jpg files inside it) to the root of that repo, keeping the same folder structure:

```
yourusername.github.io/
├── index.html
├── resume.pdf   (add this yourself, see step 3)
└── images/
    ├── hart.jpg
    ├── lunabotics.jpg
    ├── cooling.jpg
    ├── dino.jpg
    └── seascope.jpg
```

You can do this two ways:

- **Drag and drop:** open the repo on github.com, click "Add file" > "Upload files," and drop everything in at once (GitHub preserves the `images/` folder structure automatically).
- **Git:**
  ```
  git clone https://github.com/yourusername/yourusername.github.io.git
  cd yourusername.github.io
  cp /path/to/index.html .
  cp -r /path/to/images .
  git add .
  git commit -m "add portfolio site"
  git push
  ```

## 3. Add your resume
Upload your resume PDF into the same root folder and name it exactly `resume.pdf`. The "Download resume" button in the site already links to that filename, so it'll work automatically once it's there.

## 4. Turn on Pages
Go to the repo's **Settings > Pages**. Since the repo is named `yourusername.github.io`, it's usually already set to deploy from the `main` branch, root folder. If not, set that manually and save.

## 5. View it
Your site goes live at:

```
https://yourusername.github.io
```

It can take a minute or two after your first push. After that, any future push updates the live site automatically.
