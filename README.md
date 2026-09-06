# clovishigh2001.github.io

A simple static site for the Clovis High School Class of 2001, hosted with GitHub Pages. It exists to surface links and information for classmates (Facebook group, class events, etc.) and isn't affiliated with Clovis High School.

## Tech

Plain HTML styled with [Tailwind CSS](https://tailwindcss.com/) and [daisyUI](https://daisyui.com/). There's no JavaScript framework — `index.html` is served as-is by GitHub Pages, and `main.css` is a compiled build artifact checked into the repo.

## Local development

```sh
npm install
npm run watch:css   # rebuilds main.css as you edit tailwind.css
```

Open `index.html` directly in a browser to preview changes. Before committing, run a final build so `main.css` reflects your changes:

```sh
npm run build:css
```

## Submitting a change

1. Fork this repository and clone your fork locally (or create a branch directly if you have write access).
2. Create a branch for your change: `git checkout -b my-change`.
3. Make your edits to `index.html` / `tailwind.css`, then run `npm run build:css` so `main.css` is up to date.
4. Commit your changes and push the branch to your fork: `git push origin my-change`.
5. Open a pull request against the `main` branch of `clovishigh2001/clovishigh2001.github.io` and describe what you changed.

Once merged to `main`, GitHub Pages will automatically publish the update.
