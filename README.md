This is the source code of the [SPAAM Community](https://spaam-community.github.io/).

The website is powered by [GitHub Pages](https://pages.github.com/) + [Jekyll](https://jekyllrb.com/), and the theme is customized based on [Hydeout](https://github.com/fongandrew/hydeout).

## Development Instructions

To develop this website, you should following the [GitHub Pages documentation](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll).
Many components also adopted from the [sedaDNA](https://sedadna.github.io) society.

## Quick Start - Fast

Standard - edit via github, and wait for website to re-render to test:

> ⚠️ Not ideal as all changes are visible to the world before you have checked it works!

- On this repository press <kbd>.</kdb> on your keyboard
- Open the files you want to edit on the left-hand bar
- Press <kbd>ctrl</kbd>+<kbd>s</kbd> on each file to save your edits
- Go to the source control tab (on the left, should have a blue badge with a number indicating the number of files changed)
- Select all the files you want to publish to the website by pressing the `+` next to each file under the `Change` section
  - Pressing the `+` should then move the files to the `Stage` section
- Once you've selected all the files to publish, type in a brief description in the `commit message` box
- Press the `☑` button to publish!
- Shut the tab to close the workspace

## Quick Start - Best

Using GitPod and with real-time rendering of website before pushing

> 💡 Development and testing without pushing, and all without having to install anything on your laptop

- Press the gitpod button on the repository (assuming extension installed)
- Make a change
- ~~Run `bundle exec jekyll serve`, open link~~ Edit: this will be run in the background now for you on GitPod startup!!
- Press 'open preview' on prompt (or press Ports: 4000 in bottom right, then split pane icon in sidebar)
    - If you accidently close the preview or 'simple browser' tab, click ports, copy and the URL displayed, open the command pallette (e.g. `ctrl`/`cmd` + `shift` + `p`), type `simple browser` and then paste in the URL to the URL bar.

## Quick start - Hardcore

Advanced - run local server on our laptop to see changes in real time

- Install Ruby, gems, and Bundle (see above).
- Clone this repository
- Modify the files in your editor of choice (VSCode is a good option)
- Run `bundle exec jekyll serve` to check locally (with `127.0.0.1:<IP>` link on your browser)
  - Refresh page on browser after each change
  - Fundamental changes e.g. to `_config.yml` _may_ require restarting of the local server (`ctrl+c` and restart)
- Commit and push

Adding content:

- To update main home page/entry page, modify `index.html`
- To add new posts (e.g. news, events, career, meetings) to a news-like page, add your new post to `posts/`, and add the coresponding `categories:` tag.
- To allow display posts with a date in the future, put `future: true` in `_config.yml` (already set here by defualt)
- To modify the general information about these pages, update the corresponding `.md` file under `category.md`
- To update normal `page` files (e.g. about, board, membership), update the corresponding `.md` file at the root of this repository
- Add files/photos under `assets/` however please keep this 'tidy' in sub-folders and informative file names

Notes on news posts:

- Add these to `posts/`
- File name should be `<yyyy>-<mm>-<dd>-<category>-<title-of-post>.md`
- For Blog/News/Publication posts etc, the _Title_ of the post in the markdown header of the `.md` file should start with the post 'category' respectively

Notes on photos:

- If you see very pixelly images, despite being large/high resolution, scale them down to prevent (bad) web compression
- Profile pictures are ideally at a 200px width. If running on linux, install `imagemagick` and run: `mogrify -resize 200x <file>.png`

Tips and tricks for theming the website website:

- Import new fonts in `includes/font-includes.html`
- To change which fonts are actually displayed, update `$root-font-family` in `_sass/hydeout/_layout.scss`
- To change sidebar background colour, update `$sidebar-bg-color` in `_sass/hydeout/_layout.scss`
- To change sidebar font colour, update `$sidebar-fg-color` in `_sass/hydeout/_layout.scss`
- To change order of sidebar pages update `includes/sidebar.html`
- To add custom CSS classes (e.g. the membership/contact buttons), modify `assets/css/main.scss`
