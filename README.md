# Rock-Paper-Scissors
import random
def rock_paper_scissors(prev_play, opponent_history=[]):
    opponent_history.append(prev_play)
    if len(opponent_history) > 2:
        return opponent_history[-2]
    else:
        return random.choice(["R", "P", "S"])
