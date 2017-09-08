# PHP-Laravel-101

[PHP Docs](http://php.net/manual/en/)

[Laravel Docs](https://laravel.com/docs/5.5)

## Introduction to PHP and Laravel.

PHP, very much like node.js or ruby is a back-end language. It is especially suited for web development.

Laravel is a front-end framework for PHP. 

Writing PHP and Laravel feels very similar to writing Ruby and Rails respectively. 


An example of this can be seen here when we make controllers for websites:


### Rails
```
class ForumsController < ApplicationController

  def index
    @forums = Forum.all
  end

end
```

### Laravel
```
<?php

class FarmController extends Controller{
  public function index(){
    $farms = Farm::all();
    return view('farms.index', ['farms' => $farms]);
  }
}

?>
```


## Getting Started

First we needs to install some dependancies.
For the sake of this lecture we ask our users to download:

[Virtual Box](https://www.virtualbox.org/wiki/Downloads)

and

[Vagrant](https://www.vagrantup.com/downloads.html)

specifically. There are other ways of running and coding PHP and Laravel but they will change some of the ways we write our code. These other means can be explored in the official docs linked in earlier in the lecture.

Once these two are installed type the following in your terminal:

```
vagrant box add laravel/homestead
```

You will need to make a choice of what provider you want, enter 2 for virtualbox:

![provider](./assets/provider-choice.png)

There it will give you a choice of what 

Next type into your terminal:

```
cd ~

git clone https://github.com/laravel/homestead.git Homestead
```

To Initialize our homestead we need to type:

```
bash init.sh
```

Open the homestead directory in your preferred text editor of choice. 