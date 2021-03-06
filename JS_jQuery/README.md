#jQuery#

jQuery is a JavaScript library that makes it easy to interact with the DOM.

You can access it using `jQuery` or the shorthand `$`.

###Typical things we do with jQuery###
####Get and set the value of an input#####

`$('input').val()`


`$('input').val('my value')`


####Click on something or react to a click####
`$('button').click()`
```
$('button').click(function(){
    console.log('do something');
}
```


####Do something once the DOM has been loaded#####
```
$(document).ready(function(){
    console.log('document is ready');
}
```

### Aims for this lesson ###
* [Selectors](http://codylindley.com/jqueryselectors/)
* Removing / hiding elements
* Adding / removing classes (and what you can do with them)
* Running code when page is loaded
* Getting / setting values of elements

###Task 1 – Pet Shop###

#### 1.0 - Setup ####
*	Create an HTML document with Bootstrap and jQuery loaded
*	Add a `<h1>`Title to your page (the name of your shop)
*	Add pictures of kittens (hint: http://placekitten.com)

#### 1.1 – Selection####
* Practice removing a kitten / all kittens
* Practice highlighting a kitten (hint: try adding a class)
* Count how many kittens there are (hint: you need the length of the array)

N.B. By highlight, I mean emphasize in some way

#### 1.2 – Interaction####
*	Create a button to hide / show all the kittens (hint: `onclick` is an easy way)
*	Add a text input and button. Update the Title of your shop with the input’s value when the button is clicked
*	Update the title automatically when the input is changed
*	Create a way to easily ‘open’ and ‘close’ the shop

#### 1.3 – Interaction 2####
*	Highlight a kitten on click (hint: `$(this)` )
*	Toggle a highlight when on click 
*	Highlight just that kitten on click 


#### 1.3.5 Animation ####
* Apply a different [jQuery animation](http://www.w3schools.com/jquery/jquery_animate.asp) to each of your kittens when clicked (hint: `.animate()`)
* Add [animate.css](http://daneden.github.io/animate.css/) to your project and use this to animate your kittens

####1.4 – Adding elements####
*	Create a button to add a kitten (hint: `.append`)
*	Create X number of kittens on page load


####1.5 – Dom and Data####
*	Create JSON kittens with at least `name`, `imageSrc` and `price` and loop through the kittens, creating them on page load
*	Assign data to the kittens represented in the DOM (hint: HTML data attribute)
*	On click, create a message with the kitten’s name e.g. “I like Fluffy the best’

####1.6 – Bootstrap Modals####
*	Treat clicking on the kittens as a purchase. Confirm the purchase with a bootstrap modal. User redirected to a new page if he confirms purchase.


### Task 2: Create a checkout page ####
This excercise is to practise validation

#### 2.0 - HTML page with inputs####
* include name, address & a selection
* Submit button

#### 2.1 - Validate the inputs ####
* Check that the inputs are correct
* Use bootstrap [validation](http://getbootstrap.com/css/)
* Alert the user if something is wrong / missing

#### 2.2 - Modal on success ####
* Use a [bootstrap modal](http://getbootstrap.com/javascript/#modals) to indicate success

### Task 3: Create minesweeper ###
Minesweeper is a simple game where you click on tiles. Some tiles have mines underneath!

#### 3.0 - Create a simple, one-player game with static mines ####
* Mines can be in the same place (hint: use `hasClass` to check if a tile is a `mine` tile)

#### 3.1 - Randomize position of mines ####
* X mines should be distributed randomly

#### 3.2 - Make it playable ####
* Support 2 players
* Add a reset button

#### 3.3 - Make it sociable ####
* At the end of the game, add a bootstrap modal which encourages your user to share

#### 3.4 - Add settings ####
* Create an object `options = {mines: 13,...`
* Make number of tiles (X x Y) variable (hint: use `apend`)
* Make number of mines variable

#### 3.5 - Gambling! ####
* Allow users to bet on the result of the game

#### 3.6 - Make it sexy ####
* Add sound effects
* Add anmiations


