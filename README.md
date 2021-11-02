Recreating The Past

Week 1

Recreating Vera Molnar's work

Left: original piece; Right: recreation using Processing

<p float="left">
  <img src="https://user-images.githubusercontent.com/93593792/139861088-52db42d2-29a4-42bc-baf9-2da2f2a3f0f4.png" width="400" /> 
  <img src="https://user-images.githubusercontent.com/93593792/139862059-33faf040-0f84-4913-b394-c7da97589588.png" width="400" />

</p>

////

void setup() {
  size(400, 400);
  background(255);
  rectMode(CENTER);
  frameRate(1);

  push();
    for (int x=0; x<width; x=x+10) 
    for (int y=0; y<height; y=y+10) 
    {   
      translate(10, 10);
      rotate(random(HALF_PI , PI));  ;
      rect(x, y, 0.01, 50);
    }
    pop();
}

void draw() {
}

