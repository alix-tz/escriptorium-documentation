<img src="./docs/img/logo_esriptorium_tutorial.png" width=500 align="center" alt="eScriptorium Tutorial">

This GitHub repository stores the source code for the [eScriptorium tutorial](https://escriptorium-tutorial.readthedocs.io). It is a collective initiative, open to anyone and designed to be modified by anyone.

The eScriptorium Tutorial website is powered by MkDocs and hosted on readthedocs. All the source files of the pages are written in Markdown, which is a light markup language facilitating future editions.

For more information on Markdown's syntax, see the [cheat-sheet](https://github.com/alix-tz/escriptorium-tutorial/wiki/Markdown-in-Mkdocs).

## Contribute

Anyone can contribute to this project by:

- listing errors in [a dedicated issue](https://github.com/alix-tz/escriptorium-tutorial/issues/new), preferably offering solutions;
- editing the files (see below) and opening pull requests, preferably justifying the necessity of the edition;
- picking up tasks from the issues board, in particular [those tagged with "help wanted"](https://github.com/alix-tz/escriptorium-tutorial/labels/help%20wanted).

Editions can be minor (you spot a missing s, a broken link, etc) or major (a piece of information is out-dated, you want to add a whole new page, etc). Any reasonable modification is welcome, as long as it helps keep this documentation up-to-date with the core eScriptorium application.

## Edit the files and run a local test server

The following steps will allow you to locally test the success of the website's build before pushing your modifications to the project.

1. Clone this repository and move to the corresponding directory

``` sh
git clone git@github.com:alix-tz/escriptorium-tutorial.git
cd escriptorium-tutorial/
```

2. Create your own local branch

``` sh
git checkout -b my-new-branch
```

3. Create a **Python 3.8** virtual environment and install mkdocs from requirements

(with conda)

``` sh
conda -n create venv python=3.8
pip install -r requirements.txt
```

4. Start the dev server

``` sh
mkdocs serve
```

Open up [`http://127.0.0.1:8000/`](http://127.0.0.1:8000/) in your browser to see the default home page.

Note that the local server will automatically reload the content when you save a document.

For more information on how to install and use mkdocs, see [the official documentation](https://www.mkdocs.org/getting-started/).
