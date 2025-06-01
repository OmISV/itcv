## How to Make Changes and Serve Locally (Jekyll + GitHub Pages)

1. **Install Prerequisites (First Time Only)**
   - **Ruby**: Make sure Ruby is installed (version 2.5+)
   - On Windows
     - Use [RubyInstaller](https://rubyinstaller.org/)
     - Download the latest Ruby+Devkit version (2.5 or newer recommended)
     - Run the installer and follow the prompts.
   - On Mac
     - [Mac OS installer instructions for Jekyll](https://jekyllrb.com/docs/installation/macos/)
     - Directly skip to **[3.](#make-your-code-changes)**
   - **Bundler**: Install bundler if not present:
     ```sh
     gem install bundler
     ```
   - **Jekyll**: You don’t need to install `jekyll` globally; GitHub Pages uses a Gemfile.

2. **Install Project Dependencies**
   - In your project root directory:
     ```sh
     bundle install
     ```
     This will install the correct Jekyll and plugin versions as specified in your `Gemfile`.

3. <span id="make-your-code-changes">**Make Your Code Changes**</span>
   - Edit files as needed (`_posts/`, `_layouts/`, `_includes/`, assets, etc).

4. **Serve the Site Locally**
   - In the project root, run:
     ```sh
     bundle exec jekyll serve
     ```
   - Or, if your project uses the GitHub Pages Gem (common for gh-pages):
     ```sh
     bundle exec jekyll serve --livereload
     ```
   - Visit [http://localhost:4000](http://localhost:4000) in your browser to view and test changes.

5. **Iterate**
   - Make further edits as needed. Jekyll will auto-reload changes (if using `--livereload`).

6. **Commit and Push**
   - When satisfied:
     ```sh
     git add .
     git commit -m "Describe your change"
     git push
     ```

7. **Check GitHub Pages Deployment**
   - Visit your live site’s URL after GitHub Pages rebuilds your site (usually within a minute).

---

### **Common Issues**
- If you get dependency errors, delete `Gemfile.lock` and run `bundle install` again.
- For permission issues, try using `sudo` or set up Ruby via a version manager (`rbenv` or `rvm`).

---

**1-liner to install & serve**
```sh
bundle install && bundle exec jekyll serve
```

---

Agency Jekyll theme
====================

Agency theme based on [Agency bootstrap theme ](https://startbootstrap.com/template-overviews/agency/)

# How to use

### Portfolio 

Portfolio projects are in `/_posts`
Images are in `/img/portfolio`

### About

Images are in `/img/about/`

### Team

Team members and info are in `_config.yml`
Images are in `/img/team/`


# Demo

View this jekyll theme in action [here](https://y7kim.github.io/agency-jekyll-theme)

