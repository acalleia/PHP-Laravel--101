# PHP-Laravel-101

[PHP Docs](http://php.net/manual/en/)
[Laravel Docs](https://laravel.com/docs/5.5)

Introduction to PHP and Laravel.

PHP, very much like node.js or ruby is a back-end language. It is especially suited for web development.

Laravel is a front-end framework for PHP. 

Writing PHP and Laravel feels very similar to writing Ruby and Rails respectively. 

An example of this can be seen here when we make controllers for websits:


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

namespace App\Http\Controllers;

use App\Farm;
use Illuminate\Http\Request;

class FarmController extends Controller
{
  public function index()
  {
    $farms = Farm::all();
    return view('farms.index', ['farms' => $farms]);
  }

  

}
```