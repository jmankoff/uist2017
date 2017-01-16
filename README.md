This is the repo for the [ACM UIST 2017 website](https://uist.acm.org/uist2017/). Feel free to send pull requests for any corrections!

## Editing

To setup the build tools:

- First, install Node and npm if you don't already have it
- `cd` to the website folder and run `npm install`

After that, run `gulp watch` before you make any edits, and it will automatically generate any files needed.

If this seems like too much hassle don't worry, just make a pull request with your edits and I will run gulp on them myself.

## Editing the HTML

Only edit the `*.html` files in the `templates/` folder, or `*.tpl.html` files. **Any other `*.html` files are generated by the build process and your edits will be lost next time gulp runs!**

## How to make a correction via the Github website

Navigate to the `*.tpl.html` file you need to edit via the Github file manager above. Click on the file to open it, then click the pencil icon on the top right ("Fork this project and edit this file"). Once you make your changes, scroll to the bottom, write a short description of the changes you made and click "Propose file change".

## How to add a new page

Create a folder with the name of the path you want for your page (e.g. for `https://uist.acm.org/uist2017/cfp` the folder name is `cfp`). Inside it, put an `index.tpl.html` page and copy the head and foot @@includes from any of the other pages. Once you save (and assuming you've followed the instructions in the first section and are running `gulp watch`), an `index.html` file will be created in the same location as the `index.tpl.html` file.

## Editing the CSS

We use SCSS to preprocess CSS. Please only edit *.scss files, NOT the *.css files because they are generated and your edits will be lost next time gulp runs.
