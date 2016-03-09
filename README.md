## Installation

### homebrew

```
brew update && brew install hugo
git clone git@github.com:callbacknight/blog.git
```

### without homebrew (masochists)

Install [golang](https://golang.org/dl/) and configure your [GOPATH](https://github.com/golang/go/wiki/GOPATH)

```
go get -v github.com/spf13/hugo
git clone git@github.com:callbacknight/blog.git
```

## Usage

Content exists in ./content/posts/

### Add content

To add a new entry

```
hugo new posts/entry.md
```

content is in markdown by default

### Run local server

Hugo is pretty cool; you can make edits to the content and the page will dynamically refresh without needing an extension like autoreload.

```
hugo server -t lanyon
```

### Deploy to github pages

Once you have the site in a state that you like simply deploy using the deploy.sh script. This will build the site and push it to git@github.com:callbacknight/callbacknight.github.io.git on the master branch.

```
./deploy.sh "optional commit message"
```

 This is my first attempt at using [Hugo](https://gohugo.io/) and this particular theme, so please feel free to suggest alternative themes and make edits as you please.

 I chose Hugo over Jekyll or the static site generator I've been using up till now, [Nikola](https://getnikola.com/) because of how easy it is to get it installed and the speed with which it builds and serves sites.
