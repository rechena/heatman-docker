## Intro
This Dockerimage is to be run with the [Heatman](https://github.com/nagius/heatman) tool.

### How to run: 
#### Simple start
*  docker run --name heatman -d -p9292:9292 rechena/heatman

#### Start with local mount of config.yml file
* docker run -p 9292:9292 -v "$PWD"/config:/usr/src/app/config --name heatman rechena/heatman

### Access
http://__\<container ip\>__:9292

#### Notes:
In order for this to work you need to have the .sh or .py scripts to control the devices. 