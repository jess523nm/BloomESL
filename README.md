# Bloom ESL Student Lesson Hub

A pastel retro GitHub Pages site for students to access the Bloom ESL pre-test and Lessons 1–50.

## What is already wired up

- Pre-test: https://forms.gle/NV2UBcLm7mUisoq88
- Lesson 1 → `assets/bloom-guidebook-1-lessons-1-5.pdf#page=3`
- Lesson 2 → `assets/bloom-guidebook-1-lessons-1-5.pdf#page=8`
- Lesson 3 → `assets/bloom-guidebook-1-lessons-1-5.pdf#page=11`
- Lesson 4 → `assets/bloom-guidebook-1-lessons-1-5.pdf#page=16`
- Lesson 5 → `assets/bloom-guidebook-1-lessons-1-5.pdf#page=21`
- Lessons 6–50 are visible as "Coming soon" until their PDFs are added.

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`, this `README.md`, and the entire `assets` folder.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose the `main` branch and `/ (root)`, then save.
6. GitHub will give you a public Pages URL after deployment finishes.

## Add future lessons

Open `index.html` and find this section near the bottom:

```js
const lessonLinks = {
  1: { file: "assets/bloom-guidebook-1-lessons-1-5.pdf", page: 3, title: "Introductions" },
  2: { file: "assets/bloom-guidebook-1-lessons-1-5.pdf", page: 8, title: "The Problem" },
  3: { file: "assets/bloom-guidebook-1-lessons-1-5.pdf", page: 11, title: "Food" },
  4: { file: "assets/bloom-guidebook-1-lessons-1-5.pdf", page: 16, title: "Origins" },
  5: { file: "assets/bloom-guidebook-1-lessons-1-5.pdf", page: 21, title: "Actions" }
};
```

Add future lessons using the same format. Example:

```js
6: { file: "assets/bloom-guidebook-2-lessons-6-10.pdf", page: 3, title: "Your Lesson 6 Title" },
```

The page number is the **physical PDF page number**, not the printed page number inside the workbook.

## iPad/Safari note

Most desktop PDF viewers respect `#page=...` links. Some iPad/Safari configurations may open the correct PDF but ignore the page jump. The site therefore displays the target PDF page on each active lesson button as a fallback.


## Current lesson files

Lessons 1–15 are live. Lessons 16–50 remain marked Coming soon until their guidebooks are added.
