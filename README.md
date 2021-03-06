### Prerequisites

You're going to need:

 - **[Node JS](https://nodejs.org/en/)**

_Yes, that's it!_

### Getting Set Up

 1. Clone this repository to your hard drive with `$ git clone https://github.com/mpociot/whiteboard.git`
 2. `$ cd whiteboard`
 3. Install the dependencies: `$ npm install`
 4. Start the test server: `$ npm start`

Now go ahead and visit <http://localhost:4000> and you will be presented with a beautiful example API documentation as a starting point.

Go ahead and modify the markdown file at `source/index.md` to suit your needs.

### Publishing your API documentation

The easiest way to publish your API documentation is using this command within your `whiteboard` directory:

`$ npm run-script generate`

This will generate a `public` folder which you can upload anywhere you want.

> **Windows users:** You need to install the global `hexo-cli` package using `npm install -g hexo-cli`. To publish your API documentation under windows use `hexo generate`.

If you want other (more automated) deployment options like **git**, **heroku**, **rsync** or **ftp** - please take a look at the [Hexo deployment documentation](https://hexo.io/docs/deployment.html).

`$ npm install -g hexo-cli` then edit config.yml file, then do a git commit, then `hexo generate -d` or `$ hexo deploy` just deploy .deploy_git directory.

### Slate compatibility
Since both Whiteboard and Slate use regular markdown files to render the API documentation, your existing Slate API documentation should work just fine. If you encounter any issues, please [submit an issue](https://github.com/mpociot/whiteboard/issues).

### In depth documentation
For further documentation, read the [Slate Wiki](https://github.com/tripit/slate/wiki) or the [hexo documentation](https://hexo.io/docs/).
