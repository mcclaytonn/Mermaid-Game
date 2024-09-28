""Start
    A(("The Guessing Game")) --> n8(("Guess A Number 1 to 1000"))
    n8 --> bB["Computer Generates Number"]
    bB --> np("You Will Have 10 Guesses. Enter Your First Guess.")
    np --> n20{"Game Evaluates Answer?"}-->
    n7(("Incorrect Answer"))
    n7 ---> 10{"You Have Guessed Too Low"}
    10 --> nq("Game Displays Number of Guesses Remaining")
   by--> x(("If Number of Guesses > 0")) 
   x-->sky(("Enter Next Guess"))
    --> ncn{{"Game Evaluates Answer"}}
    n7 --> n10(("You Have Guessed Too High")) 
    n10 --> nq
    n20-->kw("Correct Answer. End Game") 
    ncn-->zzz(("Incorrect Answer, Loop To N7"))-->n20
ncn-->JJ(("Correct Answer. End Game."))
by-->IQ(("If Number of Guesses = 0"))-->s(("End Game."))
nq-->by(("Game Evaluates Number of Guesses"))
    style A fill:#C8E6C9,stroke-width:4px,stroke-dasharray: 0,stroke:#00C853
    style n8 stroke-width:4px,stroke-dasharray: 0,fill:#C8E6C9,stroke:#00C853
    style np stroke:#00C853,stroke-width:4px,stroke-dasharray: 0
    style n7 stroke-width:4px,stroke-dasharray: 0,fill:#BBDEFB,stroke:#2962FF
    style nq stroke-width:4px,stroke-dasharray: 0,stroke:#FF6D00,fill:#FFE0B2
""Finish 
