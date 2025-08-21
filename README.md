# Personal Website

This is a simple website which acts as my landing page to showcase my resume and portfolio. This repo is a fork of [gradfolio template](https://github.com/jitinnair1/gradfolio)

# Local Development

The easy way is to use Bundler to set up and run Jekyll locally. For this, you will need Ruby and Bundler installed for your platform.

After cloning the repo or downloading the source files, open a terminal inside the source folder and run:

`bundle install` to install Jekyll and required plugins

```bundle exec jekyll serve --incremental --trace``` 

to make it available on a local server (typically `http://localhost:4000/`)

The --incremental flag ensures that any changes you make are reflected in your browser in real-time and the --trace option might be useful for debugging if things break while you are changing the source files.


# Running locally with Docker

To test locally with docker, run the following in your terminal after installing docker into your system:

1. `docker image build -t webpage -f Dockerfile .`
2. `docker run --rm --name webpage -v "$PWD":/home/app -p 4000:4000 webpage`