# Website Build Instructions

- Ruby
- Jekyll (gem install bundler jekyll)
- bundle exec jekyll serve 
    - this runs the local server and compiles out the MD to HTML
    - Exports to the `_site` directory

# Updating Live Website

- Copy and paste the `_site` folder to the parent directory of the repo
- Switch to the gh-pages branch
- Copy contents from `_site` to the repo directory, replacing all files.
    - After copying up from `_site`, delete `_site`!
- Commit changes
