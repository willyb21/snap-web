# Snap Web

Snap Web is a web application for [Snapchat](http://www.snapchat.com/) that uses [Gibson Security's full disclosure of the private Snapchat API](http://gibsonsec.org/snapchat/fulldisclosure/).

## Requirements

* Ruby 2.0.0 - [RailsInstaller](http://railsinstaller.org/)
* Bundler - `gem install bundler`

The best way to manage dependencies for any web application is with a virtual machine. I went ahead and set up a [Ruby development box](https://github.com/mhenry/ruby-devbox) just for this project. To get started, type the following commands on the host machine:

    git clone https://github.com/mhenry/ruby-devbox.git
    cd ruby-devbox
    git submodule init
    git submodule update
    vagrant up
    vagrant ssh

## Running Snap Web

The following commands will download the code, install the gem dependencies, and run the web server.

    git clone https://github.com/mhenry/snap-web.git
    cd snap-web
    bundle install
    ruby app.rb
