
userChoice = prompt("Do you choose rock, paper, or scissors?");
userChoiceLwr = userChoice.toLowerCase();

computerChoice = Math.random();



if(computerChoice <= .33){
  computerChoice = "Rock";
}
else if(computerChoice > .34 && computerChoice <= .67){
  computerChoice = "Paper";
}
else {
  computerChoice = "Scissors";
}

console.log(computerChoice);

var compare = function(choice1, choice2){
  if(choice1 === choice2){
    return "It's a tie!";
  }
  else if(choice1 === "rock"){
    if(choice2 === "paper"){
      return "You Lose! Paper beats rock.";
    } else {
      return "You win! Rock Beats Scissors."
    }
  }
  else if(choice1 === "paper"){
    if(choice2 === "scissors"){
      return "You lose! Scissors beats paper.";
    } else {
      return "You win! Paper beats rock";
    }
  }

};

compare(userChoiceLwr, computerChoice);

