# CodeRefinery recipe book

We use this repository to teach Git and also to collect
some nice recipes.

This exercise is created from https://github.com/coderefinery/recipe-book-template.
If you wish to improve the exercise itself, please direct your pull requests
towards the template repository. I had to leave the fork network in order to be 
able to publish this repository as a GitHub Pages website:

- [enryh.github.io/recipe-book/](https://enryh.github.io/recipe-book/)


## Categories

- [salads](salads)
- [soups](soups)
- [pasta](pasta)
- [mains](mains)
- [sides](sides)
- [desserts](desserts)


## Build website

```bash
pip install -r requirements.txt
# check recipes for errors
python check_recipes.py 
```

Then build the website using:

```bash
sphinx-build -n -W --keep-going -b html ./ ./_build/
open _build/index.html
```

In the CodeSpace, right-click on `_build/index.html` and select 'Show Preview'. This
is done using Live Preview, see their
[docs](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server#features).

For more information on the usage of this template, see:
  - [enryH/notes_template](https://github.com/enryH/notes_template)
