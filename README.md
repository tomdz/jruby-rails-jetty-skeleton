This is a skeleton project showing how to combine these things:

* Rails 3.2.3
* JRuby 1.6.7
* Jetty 8.1.3

plus these development/build tools:

* Warbler 1.3.5 for assembling the rails webapp
* Maven 3 for maintaining additional java dependencies that the Rails app might need, and for assembling the final artifact (tar.gz containing jetty and the web app)

### How to use

You'll need [jruby](http://jruby.org/), installed e.g. via [rvm](https://rvm.io/) or [rbenv](https://github.com/sstephenson/rbenv).
 You also need [bundler](http://gembundler.com/) which can be installed via gem:

    gem install bundler

Finally, you'll need maven which comes pre-installed on MacOS X or can be downloaded/installed from
[here](https://maven.apache.org/download.html).

Then, clone this repo and run the build:

    mvn -Pmake-dist install

This will run bundler (to fetch relevant gems) and warbler (to build the war file), and then maven will build the `tar.gz` archive and put it into the `target` folder.