# Track2p

Track2p documentation.

For the repo of the algorithm and gui visit: https://github.com/juremaj/track2p



## For developers

### Setup (already done)

follow instructions for jupyter book setup:
https://jupyterbook.org/en/stable/start/overview.html

even better follow cookiecutter jupyter book github readme instructions: https://github.com/executablebooks/cookiecutter-jupyter-book

this will come with a template book and also it will include the automated github workflow/action to publish the html build on github pages every time that a push is made.

Important things with this:
- the `build` folder generated by `jupyter-book build Track2p/` (for example) has to be in the root of the documentation github directory
- the `.github/workflows/` directory also needs to be in the root (this is what automatically builds the website on each push)

### Making a new build

1) modify the files or contents in `track2p.github.io/Track2p`
	1) If adding new file or changing structure modify `_toc.yml`
	2) for other setting `_config.yml`
2) from `track2p.github.io` run `jupyter-book build Track2p/`
	1) you can access this by opening locally `track2p.github.io/Track2p/_build/html/index.html`
3) to publish new version:
	1) move `_build` to root of `track2p.github.io` (this could be changed maybe, check here: https://jupyterbook.org/en/stable/publish/gh-pages.html)
	2) and then add, commit, push
	3) wait for action to finish correctly (first orange circle, once finished becomes green tick)
	4) check that changes are online
