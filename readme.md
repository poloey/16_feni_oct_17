# [:house: Feni Batch Home Page](http://poloey.github.io/feni)
# Class 16 
# Home work
~Learn~ Practice php from [w3schools](https://www.w3schools.com/php/php_intro.asp) till topic [Super Globals](https://www.w3schools.com/php/php_superglobals.asp)

# Php Introduction    
Our browser only know `html`, `css`, `js`. So whenever I write something in php, those `php` code should converted into `html`. So that browser can render our page. So in order write php, you need `php` and a server in your pc. There are 2 popular server for php development `apache` & `ngnix`. In php version 7 we can create a mini server. Although in production we won't use php mini server. We will use apache or ngnix.      
So we will use a package called xampp. Which actually a package of php & apache. Its easy to use and no need any configuration. We will just install xampp. And keep php project inside `htdocs` folder. In our browser  we will access those file by `localhost/YourFolder`.    
Only 2 things you have to remember
* You will keep your php file in `xampp > htdocs > tanim` folder
* In browser you can access tanim by `http://localhost/tanim` address.

# programming 101 with php (total 7 things have to consider)
In [class 10](https://github.com/poloey/10_feni_oct_2) we have learned programming basic using javascript. Today I have described programming basic using php. All programming more or less same. So if you became master in one, you will be master at any language by practicing about one month. 7 things in php are (`variable`, `constant`, `datatype`, `control flow`, `function`, `operator`, `namespace`). Only 2 new things you will know apart fom javaScript. one is `constant` and another is `namespace`


1. Variable     
In php variable will start with `$` sign
~~~php
$name = 'sumon';
~~~
2. constant      
In php when you need to keep some value fixed in entire application you should use constant. By convention people use only uppercase when declare constant. You can write constant in 2 ways. using `const` keyword or `define` function 
~~~php
define('SOME_CONSTANT_NAME', 'sumon');
const SOME_CONSTANT_NAME = sumon;
~~~
3. Datatype
  * Scalar type (who holds only one value)
    * Numbers
      * Integer (absolute number - 10)
      * Floating / Double (Fractional number 13.14)
    * Boolean (True, False)
    * String (Text)
  * Composite type (who holds mix value)
    * Array 
      * Index array
      * Associative array
    ~~~php
      $names = ['sumon', 'sarwar', 'imran'];   //index array
      $names[0]; //sarwar     
      $names = [
        'name1' => 'sumon',
        'name2' => 'sarwar',
        'name3' => 'imran'
      ];
      $names['name2'] = 'sarwar'
    ~~~
    * Object     
      In php, object will get by instantiating a class. to get object we use `new` keyword. A `variable` inside class called `properties`. A `function` inside class called `Method`. 
      ~~~php
      $today = new Date();
      $today->someProperties.
      $today->someMethod().
      ~~~
      In php, working with object called object oriented programming. Object oriented programming has 5 features. `Encapsulation`, `Inheritance`, `polymorphism`, `overriding`, `overloading`     
      * `Encapsulation`: For encapsulation we use 3 visibility filter for class properties.  `public`, `private`, `protected`. When we use `public` we can access class properties or method from anywhere.  When we use `private` we only able to use class properties or method from inside class. When we use `protected` we can use class properties from own class and child class.
      * `Inheritance`:  When I need to share functionality between more class we use `inheritance`. In this case one class will be parent class. One class will be child class. child class `extends` parent class. I can extends only one parent class.
      ~~~php
      class Parent {
      }
      class Child extends Parent {
      }
      ~~~
      * `polymorphism`: When we need to work with multiple features we generally implement polymorphism. In polymorphism we need a `interface` and implement by a class. I can implements lot of `interface`
      ~~~php
      interface Parent {

      }
      interface Uncle {

      }
      class Child implements Parent, Uncle {

      }
      ~~~

4. Control flow
  * iterative
    ~~~php
    //while 
    var $number = 0;
    while($number < 3 ) {
      $names[number];
      $number = $number + 1;
    }
    //for, while, foreach  

    for ( $number = 0; $number < 3; $number ++ ) {
      $names[number]
    }
    for ($number in $names) {
      $names[$number]
    }
    ~~~
  * conditional
    ~~~php
    //if, else, else if, elseif, switch, Ternary
    if (true/false) {
       echo 'if true';
    } else if (true / false) {
      echo 'if this block is true';
    } else {
      echo 'any if block is not true';
    }
    ~~~
5. Function   
  Built in Function 
  ~~~php
  $names = ['sumon', 'sarwar', 'tanim'];
  count($names) // 3
  ~~~

  User Defined function   
  ~~~php
  function add ($number1, $number2) {
    return $number1 + $number2;
  }
  add(2+3);
  add(5+3);
  ~~~
  
6. operator
~~~php
+ - * / % = > < == ===  ++ -- | 
~~~
`%` (Modulus) returns the division remainder    
`++` increse by 1    
`--` decrese by 1    
`==` equal check    
`===` identity check (equl check + datatype check)        

7. namespace
When we give namespace to file we will use `namespace` keyword. When we use this we will use `use` keyword. Keeping namespace like keeping people name.
~~~php
//keeping namespace
<?php
namespace Israt\HelloWorld;
//some php code
?>
<?php
namespace Tofael\HelloWorld;
//some php code
?>

//In 2 cases we keep name HelloWorld. But since we add there app name `Israt` & `Tofael` before So it conflict with each others
//using 
<?php
Use Israt\HelloWorld\Filename;
Use Tofael\HelloWorld\Filename;
?>


~~~

# Basic php tag
~~~
<?php ?>
~~~
so php start tag is `<?php` and end tag is `?>`     

# to create a mini php server
~~~
php -S localhost:8000
~~~
Here `8000` is port number. You can use 4 digit number


# to write something in php

~~~php
echo 'Hello Tanim';
//or
print ('Hello tanim')

~~~
# difference between php and js
When we use some key value in ja we use `:`. Therefore in php it will be `=>`      
~~~
//js
key: value,
key: value

//php
key => value,
key => value
~~~


In `js`, we getting value from object by `.` notation. In `php`, we will getting value by `->` notation.

~~~
//js
object.name;

//php
$object->name;
~~~













