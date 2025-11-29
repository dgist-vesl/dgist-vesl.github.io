# dgist-vesl.github.io
VeSL - DGIST Verified Systems Lab

Instruction [(link)](https://docs.github.com/ko/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)
- Create a repository with the name xxx.github.io and clone it
- mkdir docs; cd docs (Since I prefer this way)
- jekyll new --skip-bundle .
- Open `Gemfile`
  + Comment out `gem "jekyll"`
  + Add `gem "github-pages", "~> GITHUB_PAGES_VERSION", group: :jekyll_plugins` where `GITHUB_PAGES_VERSION` is the latest supported version of the `github-pages` gem (check [here](https://pages.github.com/versions.json), e.g., `232`)
  + Save and close Gemfile
- run `bundle install`
- Open `.gitignore` and Add `Gemfile.lock`
- Test locally by `bundle exec jekyll serve` and open [localhost](localhost:4000)