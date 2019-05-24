# Rails

The goal of this dockerfile is to provide a minimal environment to develop your own rails applications on top of.

To use please create your own Dockerfile and use ```FROM mdrewt/rails:latest```. Then copy your rails app into the working directory, CD into that app, bundle install, and use ```CMD [ "bundle", "exec", "rails", "server", "-b", "0.0.0.0", "-p", "3000" ]``` to start the server. port 3000 has already been exposed.

### Release 1.0
Linux Distro: Debian

JS Runtime: NodeJS
- NodeJS version: 12.3.1
- NPM version: 6.9.0

Rails version: 5.2.3

Ruby version: 2.6.3
