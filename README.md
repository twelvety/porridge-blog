# My porridge blog

This repository is a [porridge](https://github.com/alexjj/porridge) blog: an
outliner for writing a daily blog. You write in the porridge editor; your posts
are kept here as plain files, and GitHub Actions publishes them as a website on
GitHub Pages. There's nothing to host or install.

## Set up (about five minutes)

1. **Turn on Pages.** In this repository, go to **Settings → Pages** and set
   **Source** to **GitHub Actions**.
2. **Make a token for the editor.** Create a
   [fine-grained personal access token](https://github.com/settings/personal-access-tokens/new):
   - **Repository access:** *Only select repositories* → this repository.
   - **Permissions:** **Contents** and **Actions**, both *Read and write*.

   Copy the token. You'll paste it into the editor once; it's kept only in
   that browser.
3. **Connect the editor.** Open the editor at
   **<https://alexjj.github.io/porridge/>**, choose **Connect GitHub**, and
   enter this repository (`your-name/your-repo`) and the token. It loads the
   example blog that's in this repository.
4. **Set up your blog.** In the editor, open **⋯ → Blog settings** and fill in
   the title, your name and your timezone. Leave the site address empty: the
   site is published at this repository's GitHub Pages address
   (`https://your-name.github.io/your-repo/`). Fill it in only if you use your
   own domain.
5. **Publish.** Press **Publish**. After a minute or so the status says
   *Published* and links to your site.

The example posts show what porridge can do. Read them, then edit or delete
them and start writing with **New entry**.

## Day to day

- **New entry** adds a post under today's date.
- **Save** keeps your changes here on GitHub without changing the site.
- **Publish** saves and rebuilds the site.
- On a phone, the same editor works in the browser, with a toolbar above the
  keyboard.

## What's in this repository

```
blog.opml          blog settings, plus one entry per year
blog/2026.opml     the year's posts (a new file is added each year)
pages/about.opml   an About page; add more pages from the editor
images/            photos added in the editor
.github/workflows/ builds and publishes the site
```

You never need to edit these by hand, but they're readable if you want to.
The format is described in
[porridge's format.md](https://github.com/alexjj/porridge/blob/main/docs/format.md).
