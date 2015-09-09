# rudy

Puzzle 1

right();
down();
down();
down();
down();
down();
down();
down();
right();
right();
right();
right();
up();
up();
right();
right();

Puzzle 2

function move(direction,total) {
  var count = 0;
  while (count < total) {
    direction();
    count = count + 1;
  }
}

move(down,6);
move(right,3);
move(up,2);
move(right,2);
move(down,3);

Puzzle 3

function move(direction,total) {
  var count = 0;
  while (count < total) {
    direction();
    count = count + 1;
  }
}


move(down,2);
var color = getColor();
move(down,3);
move(right,2);
setColor(color);
move(right,2);
move(up,1);

Puzzle 4

function move(direction,total) {
  var count = 0;
  while (count < total) {
    direction();
    count = count + 1;
  }
}

move(down,4);
move(right,1);
var color = getColor();
move(down,1);
setColor(color);
move(right,3);
move(up,1);
var color = getColor();
move(down,1);
setColor(color);
move(right,2);


Puzzle 5

function move(direction,total) {
  var count = 0;
  while (count < total) {
    direction();
    count = count + 1;
  }
}

function decide() {
  if (getColor() == "blue") {
  down();
} else {
  up();
}
  }

move(right,2);
decide();
move(right,2);
decide();
move(right,2);
decide();
move(right,3);


Puzzle 6

function move(direction,total) {
  var count = 0;
  while (count < total) {
    direction();
    count = count + 1;
  }
}

function decide2() {
 var initial = getColor(); 
  if (getColor() == "blue") {
  down();
  down();
  down();
    if (getColor() == "blue") {
      right();
      down();
    } else {
      left();
      down();
    }
} else {
  up();
  up();
  up();
   if (getColor() == "blue") {
      right();
      up();
    } else {
      left();
      up();
    }
 }
  }

move(right,1);
decide2();

Puzzle 7

function move(direction,total) {
  var count = 0;
  while (count < total) {
    direction();
    count = count + 1;
  }
}


function solve(direction) {
 while (getColor() != "red") {
  direction();
} 
}


solve(down);
move(right,2);
solve(up);
move(right,2);
solve(down);
move(right,2);
solve(up);
move(right,2);
solve(down);
move(right,1);


Puzzle 8

function move(direction,total) {
  var count = 0;
  while (count < total) {
    direction();
    count = count + 1;
  }
}


move(down,8);
move(right,2);
move(up,7);
move(right,2);
move(down,7);
move(right,2);
move(up,7);
move(right,2);
move(down,7);
move(right,1);
