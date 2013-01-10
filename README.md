## subl 

The subl repo contains a chef-solo based installer for Sublime Text 2. This is for sharing my own personal module and keybinding preferences between OSX and ubuntu desktops.

## Installation 
The installer will bootstrap chef-solo if necessary and the run 'chef-solo -c solo.rb -j install.json' from the kitchen directory
```
> sudo ./install.rb
```
## Push
In the event that you add new packages or keybindings the push recipe will tar up the current state of sublime on either platform and push it to github
```
> # from the kitchen directory
> chef 'chef-solo -c solo.rb -j push.json'
```

## Authors

* Sean Kelly sean.alexander.kelly@gmail.com

## License

Licensed under the Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
