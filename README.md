# billowin

Another cloud thing.

## Introductory Rant

I keep saying I want to build a solution to my hatred for what Heroku has become. So this is an another attempt to turn my dream into reality. This app will be a web app that acts as the control plane for my dream. It will send requests to a scheduler to actually schedule jobs. It will store configuration and user authentication. Users will give us a git repo containing a 12 factor app, and we'll spin it up on the scheduler.

After this piece is built, we will also talk to a router which will send requests to the right place. It will also tell the monitoring service to start monitoring things.

Rant continued: https://writing.natwelch.com/post/570

## Config

I think people want a build config. Might as well just have them be explicit.

```
language:
  name: ruby
  version: 2.3.0

apt:
 - some-package
```
