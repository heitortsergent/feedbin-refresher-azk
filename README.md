# feedbin-refresher-azk

This is a repository containing both [Feedbin](https://github.com/feedbin/feedbin) and the [Refresher](https://github.com/feedbin/refresher) service.

Feedbin is an awesome open-source RSS reader, but it's not exactly easy to set it up in a local environment. You're gonna need to install Homebrew, rbenv, Ruby, Bundler, Postgres, Redis, Pow, Elasticsearch and Memcached.

This is a way to easily set up all of the above, plus the feed refreshing service "Refresher" with azk. :)

## Running the project

### Install azk

If you are using a Mac and already have Virtualbox installed, or are using Linux with Docker installed, just run:

```sh
$ curl -Ls http://azk.io/install.sh | bash
```

You can find more detailed instalation instructions [here](http://docs.azk.io/en/installation/index.html).

### Running the project

```sh
# We are using git submodules
$ git clone --recursive https://github.com/heitortsergent/feedbin-refresher-azk.git

# Start the azk agent
$ azk agent start

# Start the project
$ azk start
```

After that you can access http://feedbin.dev.azk.io/. :)
