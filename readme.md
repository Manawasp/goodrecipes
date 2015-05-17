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

#### Install and configure

**Install depandancies**

`sudo apt-get install curl git-core build-essential zlib1g-dev libssl-dev libreadline6-dev gem libyaml-dev`

**Download RVM (Ruby Version Manager)**

`curl -sSL https://get.rvm.io | bash`

*if you have some problem you should to follow [these instructions](https://rvm.io/rvm/install)*

Binaries are installed in `$HOME/.rvm`. You should to give rvm access via your term, (if you use bash)    `echo '[[ -s "$HOME/.rvm/scripts/rvm" ]] && . "$HOME/.rvm/scripts/rvm" # Load RVM function' >> ~/.bashrc`   and now close your term or if you prefer smarter solution:    `source ~/.bashrc`


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
