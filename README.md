# ▲ Next.js Bootstrap ▲

> A quick scaffold to get a Next.js project started.

### Quick Start

```sh
# Download the repository
$ curl -LO https://github.com/stephenhowells/next-bootstrap/archive/master.zip

# Extract the starter files
$ unzip master.zip

# Name the project something useful
$ mv next-bootstrap-master some-useful-name

# Enter the project directory
$ cd some-useful-name

# Add the Yarn packages
$ yarn add next react react-dom

# Start the dev server
$ yarn run dev
```

### Automate the Steps

You can also create a shell function to automate the quick start and save even more time. Simply copy the function below and place it somewhere that it will get loaded by ZSH.

```sh
nextjs() {
    curl -LO https://github.com/stephenhowells/next-bootstrap/archive/master.zip
    unzip master.zip
    mv next-bootstrap-master "$*"
    cd "$*"
    git init
    yarn add next react react-dom
    yarn run dev
}
```

With this function all that is required to start a new project is `$ nextjs project-name`. You can see how I added this to my shell environment in my [dotfiles repository](https://github.com/stephenhowells/dotfiles/blob/master/functions/functions.zsh#L74).

### License

Licensed under the [MIT license](http://opensource.org/licenses/MIT)
