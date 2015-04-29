# Intro JavaScript
## Control Flow

| Objectives |
| :--- |
| Apply knowledge of methods and types to solve small exercises |
| Play with control flow structures |

Please try the following exercises in the Chrome console.

First complete all exercises from the [**JS Primitives**](https://github.com/sf-wdi-18/notes/tree/master/lectures/week-01/day_2_intro_js/dawn_js_primitives) lesson.


## Exercises

* Practice using `prompt`, `confirm`, and `alert` try the following. You may want to look them up on **MDN**.
  * Ask the user for the their `firstName`. Then `alert` it.
  * Ask the `user` `"have we met before?"`. If `true` then respond `"nice to meet you"`.
* Get the temperature from the user and alert it back in Celsius.
* Confirm if a user has three friends? Use a loop and `prompt` to collect the names of the `friends`. Alert back the names of the `friends`.
* Prompt the user to give a word. Then alert back the number of vowels.
* Write a loop to solve the following riddle. I am a number between `2` and `100`. I am even and a multiple of 3. I end in `2`. My digits sum to `9`.
* Hard: Generate a random number between 1 and 100, an integer and not a float. Prompt the user to guess the number. Continue prompting the user for a guess using a loop, telling them each time if the number is lower or higher. Alert correct when they guess the number.
* Super Challenge: Given an array of friends






\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

My solutions

``` 
    var person = prompt("Please enter your name");
    window.alert("Hello!," + person);
    if (confirm("Have we met before?")) { 
       console.log("nice to meet you!");
   }

```


```
   var temperature = prompt("What is the temperature in Fahrenheit");
   var celsius = (5/9)*(temperature - 32);
   window.alert("The temperature in Celsius is: " + celsius);

```


```

   var friends = 3;
   var friendsArray = [];
   if (friends === 3) {
      for (var i = 0; i < 3; i++) {
         friendsArray.push(prompt("enter your friends name: "))
      }
   }
   
  window.alert("your three friends are: " + friendsArray);

```


``` 
   var word = prompt("Please enter a word")
   var numberVowels = 0;
   for (var i = 0; i< word.length-1; i++) {
      if (word[i] == "a" ||word[i] == "e" ||word[i] == "i" ||word[i] == "o" ||word[i] == "u") {
         numberVowels += 1
      }
   }
   window.alert("there are " + numberVowels + "in the word" + word) 

```



  ```
  var friends = [
                  "larry",
                  "moe",
                  "curly",
                  "huey",
                  "louie",
                  "dewey"
                  ].


  ```

  write a loop to alert them in some random order. 

var friends = [
"larry",
"moe",
"curly",
"huey",
"louie",
"dewey"
];
var newArray =[];
var value;

value = Math.floor(Math.random()*(6-0)) +0;

while( newArray.length < 6 && newArray.includes(friends[value]) ===  false) {
alert("Hey! " + friends[value]);
newArray.push(friends[value]);
value = Math.floor(Math.random()*(6-0)) 
}
