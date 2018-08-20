# The Amazing Mouse Maze
### By: dotfig

## How to Play

![Maze Game](https://github.com/dotfig/the-amazing-mouse-maze/blob/master/maze1.png)

#### Start off my hovering your mouse over the letter 'S' which is surrounded by a green box.
````
function startClick() {
    var x = document.getElementsByClassName("boundary");

    for (var i = 0; i < x.length; i++) {
        x[i].style.backgroundColor = "#eeeeee";
        if (x[i].style.backgroundColor != "red") {
            var s = document.getElementById("status").innerHTML = "Move your mouse over the 'S' to begin.";
        }
    }
}
````

#### Carefully move the mouse between the path. If the mouse hits the boundary, you will lose the game and will be forced to start over.
````
function overBoundary() {
    var x = document.getElementsByClassName("boundary");

    for (var i = 0; i < x.length; i++) {
        x[i].style.backgroundColor = "red";
        if (x[i].style.backgroundColor == "red") {
            var s = document.getElementById("status").innerHTML = "You Lose!";
        }
    }
}
````

#### To win the game, hover over the letter 'E' without any errors!
````
function overEnd() {
    var x = document.getElementsByClassName("boundary");

    for (var i = 0; i < x.length; i++) {
        if (x[i].style.backgroundColor != "red") {
            var s = document.getElementById("status").innerHTML = "You win!";
        }
    }
}
````

#### Watch out and dont cheat, we got the covered.
````
function noCheat() {
    var x = document.getElementsByClassName("boundary");

    for (var i = 0; i < x.length; i++) {
        x[i].style.backgroundColor = "red";
        if (x[i].style.backgroundColor == "red") {
            var s = document.getElementById("status").innerHTML = "Nice Try...";
        }
    }
}
````


### Good Luck!
