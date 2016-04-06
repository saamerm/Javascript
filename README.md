For people interested in the web detrack, learn material and bootstrap.
#Jquery 
Javascript is a language  Jquery simply a library written in javascript
jquery but dojo kindo. same syntax. PARTS-
1) Dom - provides a consistent cross-browser way of working with the DOM. Provides a simplified technique for accessing elements in the DOM using CSS selectors.
2)ajax - Privudes several simple methods you can use to exchange data with a web server using Ajax and easy ways to work with the data
3)events & 
4)effects - built in effects & animations

Two different ways->

var result=$("body");
A DOM selector 
var result2=$.get("");
Utilty class
focus on components, selectors. 
$ signs is jquery. 
Dont clash or race conditions. 
$ or jquery. var html=document.getElementById(""); var body=$("body"); 

$(document).ready(function()){
                  });
//is the same as 
$(function(){}); //since we are passing a function

var $=function(obj){ 
};

$(document);

//$ sign is not just a function

//Eg
var $=function(x){
  return 9+x;
};
var result=$(9);//18
//prototype means base class
$.prototype.subtract=function(x){
  return x-1;
};
car result2=$.subtract(9);//8
//AJAX in JQuery
var result=$("body");
var result2=$.get("");

//SELECTORS
//Selectors are CSS based JQuery base
//There s an expression you can do but thats the only difference
$("a"
 
 Every btn object thats inside a span
 $("span .btn")

//The small piece of page, partial, not the whole body, just piece of code that will be placed multiple times.
<a href="http://www.google.com">Me</a>
 //Doesnt have a target=...
a ("a[href]")
a ("a[href='http://www.google.com']")
//Every a tag with that link that doesnt have a target defined
a ("a[href='http://www.google.com']:not([target])")
//Every a tag with http in the beginning that doesnt have a target defined
a ("a[href^='http']:not([target])").each(function(){
  //Anything within square brackets means you are selecting an attribute  
  //this.html() will error out since html is not a javascrip call
  $(this).attr("target","_blank");
  $(this).attr("target","_blank").text("go away"); //chaining
  $(this)
    .attr("target","_blank")
    .text("go away"); 
});

  var context="span";
$(".btn", "span")

//<a href=".." data-target="#myframe">Abs</a>
$("a[data-target]").attr('data-target');
//convention over configuration
$("a[data-target]").data('target');
//If you want to store something in that, storing the dom element as the key. I think this is how you write it
$("a[data-target]").data('target',{x:1});

//if you want to grab every input 
//::before after nth child last child
$(":input") //or visible hidden $(":input") 
//a:not/has/is
$("a:has(.doit)") // is the same as $("a.doit") 

//Below shows that 
<div class="view-a">
  <a href="..." data-target="..">ABC</a>
</div>
  
var context=".view-a"
$("a[href^='http']:not([target])", context).each (function){
 $(this)
....
});

EVENTS
Ready is basically on load of page
You cannot add an event handler to an event that doesnt exist.
<button type="button">Go</a>
<script>
  $("button").on('click',function()[
  $("button").on('click dblclick',function()[
  //..This will work to add an event handler to an element
  //click is the name like the html window event handler. like mouseover, etc. Also like $("button").click(function()[
//Event is fired three times 
    //$("button"). trigger handler is also a good way of going about
    //Below will only let it fire off once
    $("button").one('click dblclick',function(){});
    //Below is to remove the event handler->dispose any memory leak and cover tracks
      $("button").off('click',function())[
        //Killing the ability to be clicked
      var handler=function(){};
        $("button").off('click',handler)[

//]);
//  </script>
    
    //Makes sense to just delegate the event
    <button type="button">Go</a>
    <button type="button">Go</a>
    <button type="button">Go</a>
    <button type="button">Go</a>
    <button type="button">Go</a>
    <script...></script>
    <script>
    $("button").on('click',function(){
    
    });
    //Event delegation or BUBBLING, doing an event handler on the body tag. I know that there is going to be a body tag and only one
    $("body").on('click','button',function(){
        });
    //Helps a lot with ordering of operations
    </script>
    //--------------------------------
    
    //You can name space your events
    <script...></script>
    <script>
    $("button").on('click.travis.ui',function(){
    
    });
    $("button").triggerHandler("click");
    $("button").off('.travis');    
    </script>
    //THIS IS BAD <body onload=""> <button onclick="javascript:alert('hi');"> <button onclick="javascript:alert('hi');"><button onclick="javascript:alert('hi');">
    
    $('[title]').tooltip(options);
    //All titles get tooltips
    //#Go to getbootstrap.com/javascript/#tooltips
    //#PLUGINS
    //
    $([title]').')
  //Animation boolean true Apply a CSS fade transition to the tooltip
  //container string/false false Basically its a string or a boolean of a type false
  $('[title]').tooltip({
    animation:true;
  });  
  {key:'value';
    }
   a boolean of a type false
  $('[title]').tooltip({
    delay:{
  show:500,hide:300
  }  });  
  //HOMEWORK Take the exact html  frm the website getbootstrap. An example of each one
  //$('[title]').tooltip({
    placement:top;
  }  });  
  //OR
  $('[title]').tooltip({
    placement:function(element, target){
  $(el).css({
  top:50;//top:target.offset().top+10; also
  })
  }  });  
  //There is no return type
  
  //Play most with Modal
  //Heres the title, heres the body, and i make it one method
  //Skip scroll spy
  //Until tooltip
# Javascript
Put your script just before the body tag
Place the javascript after document.ready to prevent the blink 
http://eloquentjavascript.net/02_program_structure.html
Eloquent book

-++-First App-++-
+++===+++

<!DOCTYPE html>
<html>
<head>
<script>
<!--<script type="text/javascript"> is assumed You can also do <script type="template" id="mytemplate">-->
<!-- <h1>{{Name}}</h1> Gives you the Name attribute of the tag -->
<!-- Window is assumed, window.alert() Alert -->
var x;
var y=9;
<!-- message="Hello World!"; is incorrect because it makes it a window.message-->
var message="Hello World!";
console.log(message);
<!-- alert("Hello World"); -->
alert(message);
</script>
</head>
<body>
</body>
</html>
____________
#About JS
Creating a simple JS app 
Using Visual Web Dev exp edi to create JS apps
JS Language Basics
DOM DOcument Object Model
jQuery library 
JS Best Practices & Conventions
(What about NodeJS and EmberJS)

JS used to show or hide a web page elemts in response to a users interaction
Client side form field validation
Animation Interactivity Style.
Client server data exchange does not require full page refreshes-You dont need http post & get 

