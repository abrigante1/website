# Website Build Instructions

- Ruby
- Jekyll (gem install bundler jekyll)
- bundle exec jekyll serve 
    - this runs the local server and compiles out the MD to HTML
    - Exports to the `_site` directory

# Updating Live Website

- Switch to the gh-pages branch
- Upon switching, everything will update *with the execption* of `_site`
- Delete everything in directory execept `_site`
- Copy contents from `_site` up to the root directory
- Commit changes