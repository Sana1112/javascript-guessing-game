// GLOBAL VARIABLE TO STORE RANDOM NUMBER
let number = null;

// HELPER FUNCTION TO GENERATE A RANDOM NUMBER
function genRandom(min, max) {
  return Math.floor(Math.random() * (max - min) ) + min;
}

// TODO #2: Define startGame() and playGame() functions here
function startGame(){
    console.log("ABC"); 
    number = genRandom(-20,20); 
    let clues = " ";
    if ( number > -20 && number < 20){
        clues += "The number is between -20 and 20. <br>";
    }else return

    if(number > -21 && number < 0) {
        clues += "Number is negative. <br>"; 
    }else if (number > 0 && number < 20){
        clues += "Number is positive. <br>";
    }else { 
        clues += "Number is zero. <br>"; 
    }
    if (number % 2 === 0) {
        clues += "Number is even. <br>";
    }else { 
        clues += "Number is odd. <br>";
    }
    if (number % 3 === 0) { 
        clues += "Number is divisible by 3. <br>";
    }else { 
        clues += "Number is not divisible by 3. <br>"; 
    }
    document.getElementById("clues").innerHTML = clues; 
}


function playGame() {
    let guess; 
    if (number == null){
        alert("Click New Game"); 
        return null; 
    } else { 
        guess = prompt ("Enter number: "); 
    } 
    if (guess == number ){ 
        alert("The correct answer is: " + number + ". You win!"); 
    } else { 
        alert("The correct answer is: " + number + ". You lose!"); 
    }
    number = null; 
}

// WAIT FOR THE PAGE TO LOAD BEFORE ADDING LISTENERS
window.addEventListener("load", function(){
    
    // TODO #1: Set listeners for buttons here
    document.getElementById("newGame").addEventListener("click", startGame); 
    document.getElementById("guessNumber").addEventListener("click", playGame); 
});
