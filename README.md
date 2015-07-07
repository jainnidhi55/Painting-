# Painting-
Jackson Pollick Painting 

noStroke();
// position of the car
var i = 20;
var count = 1;

var draw = function() {
    
    mouseDragged = function(){
        if (count === 1){
            fill(24, 66, 89);
        }
        else if (count === 2){
            fill(52, 145, 176);
        }
        else if (count === 3){
            fill(204, 222, 227);
        }
        else{
            fill(154, 124, 194);
        }
        ellipse(mouseX, mouseY, 10 + i/3, 10 + i/3);
        i -= 1;
    };
    if (! mouseIsPressed){
        i = 20;
        if (count <= 3){
            count++;
        }
        else{
            count =1;
        }
    }
};

