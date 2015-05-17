# Goodrecipes

Group all subproject goodrecipes    
Module Project Training    
Beijing Jiao Tong University 2015    
Beijing, China    

## Summary

1. [Description](https://github.com/Manawasp/goodrecipes#description)
2. [Repository](https://github.com/Manawasp/goodrecipes#repository)
3. [Web - application](https://github.com/Manawasp/goodrecipes#web---application)
	1. [Framework / Libraries / Languages](https://github.com/Manawasp/goodrecipes#framework--libraries--languages)
	2. [Installation](https://github.com/Manawasp/goodrecipes#install-and-configure)
4. [API - application](https://github.com/Manawasp/goodrecipes#api---application)
	1. [Framework / Libraries / Languages](https://github.com/Manawasp/goodrecipes#framework--libraries--languages-1)
	2. [Installation](https://github.com/Manawasp/goodrecipes#install-and-configure-1)
5. [Authors](https://github.com/Manawasp/goodrecipes#authors)
	1. [Clovis Kyndt](https://github.com/Manawasp/goodrecipes#clovis-kyndt)

## Description

Goodrecipes is a project where you manipulate ingredients and recipes created during our curriculum at Beijing Jiao Tong University. It will have mobile application (android), web application and an API. There is different kind of user.
- Simple user can see recipes, add favorites, mark recipes, and use the powerfull search bar for recipes
- Cooker is able to create and manage its recipes
- Grosist is able to create and manage ingredients
- Admin is able to create and manage everything, and have access to 'sexy' user data

## Repository

I use submodule so you to retrieve all of this repository you should to follow these instructions.    

**Shorter way:**    
`git clone --recursive git@github.com:Manawasp/goodrecipes.git goodrecipes`

**Other way:**    

```
$ git clone git@github.com:Manawasp/goodrecipes.git goodrecipes`
$ cd goodrecips
$ git submodule init
$ git submodule update
```

Now you should to have a lot of files in `goodrecipes/webapp/`, `goodrecipes/api/`.

## Web - application

#### Framework / Libraries / Languages

- [Haml](http://haml.info/)
- [SCSS/SASS](http://sass-lang.com/)
- [CoffeeScript](http://coffeescript.org/)
- [Bower](http://bower.io/)
- [Boostrap](http://getbootstrap.com/) _need to be deleted_
- [AngularJS - 1.3.x](http://angularjs.org)
- [AngularJS Material Design](http://material.angularjs.org)
- [Rails - 4.1.4](http://rubyonrails.org/)

#### Install / Configure / Deploy

##### Install from scratch

**depandancies**    
`sudo apt-get install curl git-core build-essential zlib1g-dev libssl-dev libreadline6-dev gem libyaml-dev`

**Download RVM (Ruby Version Manager)**    
`curl -sSL https://get.rvm.io | bash`

*if you have some problem you should to follow [these instructions](https://rvm.io/rvm/install)*

Binaries are installed in `$HOME/.rvm`. You should to give rvm access via your term, (if you use bash)    
`echo '[[ -s "$HOME/.rvm/scripts/rvm" ]] && . "$HOME/.rvm/scripts/rvm" # Load RVM function' >> ~/.bashrc`

Now close your term or if you prefer smarter solution:    
`source ~/.bashrc`

Try this command to see if it works:    
`rvm info`

**Install Ruby**

We want to install the `2.1.1` version but you can specify any version you want.    
`rvm install 2.1.1`

Choose your default ruby version:    
`rvm --default 2.1.1`

All works ?    
`ruby -v`

**Rails installation**    
`gem install rails`

#### Configure

Now go inside of the webapp `goodrecipes/webapp/`, and run this command:    
`bundle install`

After you should to have `bower` installer if not be sure `npm` is installed:    
`npm install bower` / `sudo npm install bower -g` (access everywhere)

When `Bower` is installed follow this instruction to init the asset components:    
`rake bower:install`

_If bower ask you to choose some version, take the choice with the `1.3.x` angular version._

#### Deploy

_API should to run if you want to haven't issues._    
`rails s -p 3000`

**note**: Currently there is no production mode, api and website you should to run in the same IP, api need to run on the port 8080.

#### Developmentt

I use haml but rails compile haml only in `app/views` or my HAML template for Angular are in `webapp/app/assets/javascripts/templates/`.
To manage this I use `guard` & `guard-haml` so if you want to compile this file go in `webapp/' and just run:    
`guard start`    
When you will save your file, guard will compile it automatically and he will provide a notification if there is success or error.

## API - application

#### Framework / Libraries / Languages

- [Node.js](https://nodejs.org/)
- [Apiary (documentation)](http://docs.foodapicn.apiary.io/)
- [Mongodb](https://www.mongodb.org/)
- [Redis](http://redis.io/)
- [Express](http://expressjs.com/)
- [Mocha.js (Test Units)](http://mochajs.org/)
- [Expect/Should (Test Units)](http://chaijs.com/api/bdd/)
- [JWT](jwt.io)

### Installation and configure

_soon_

## Authors

### Clovis Kyndt

- Works: Web application, API, Conception.
- Contact: [Github](https://github.com/Manawasp), [Website](http://cloviskyndt.com)

## Source

- [installation Rails via RVM - recommended](http://doc.ubuntu-fr.org/rubyonrails)
