# Quick-start

<!-- New subsection -->

## Use of this template

Using this template is very simple.
Just clone the repository or create a new one from this template and add the desired presentations in the `presentations` folder.

Pushing a new commit to the `main` branch will trigger a GitHub Action that will update the GitHub Page of the repository.

<!-- New subsection -->

### Building locally

To build the presentations locally, you can run the `build.sh` script.

It will go through all the subfolders in `presentations` and add an html index file based on the template found in the `vendor` folder.
It will also create one at the root of the project, to be used as the homepage of the repository.

Just serve the root folder with any web server (like [http-server](https://www.npmjs.com/package/http-server) or [LiveServer](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)) and navigate to the desired presentation.

<!-- New subsection -->

### File structure

```shell
├── .github/workflows # GitHub Actions workflows. Updates the github page
├── presentations
│   ├── My-first-presentation
│   │   └── README.md
│   └── My-second-presentation
│       └── README.md
├── vendor # Custom CSS and JS files
│   └── index.html # Template html file used for the presentations
├── build.sh # Script to build the presentations locally
└── README.md # Homepage of the repository
```
