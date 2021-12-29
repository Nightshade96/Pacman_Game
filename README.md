# Pacman AI Implementation

This implementation is the extension of the Pacman project http://ai.berkeley.edu/project_overview.html.

![Pacman gif](http://ai.berkeley.edu/images/pacman_game.gif)

## Dependencies 
Python >= 3.9
Numpy >= 1.21.4

## Human
Play game by running the below command and using ASWD or arrow keys:
```
$ python pacman.py
```

## Alpha-Beta pruning algorithm(baseline AI)
- Running Alpha-Beta algorithm on a pacman game with minimax.
```
$ python pacman.py -p AlphaBetaAgent -l openClassic
```

## IDS algorithm
- IDS: Running IDS algorithm to find the best possible path with evaluation function.
```
$ python pacman.py -p IDSAgent -l mediumClassic
```

Different types of mazes are available in layouts directory. To run above algorithms on layout specified in layouts directory replace -l mediumClassic/openClassic to -l {layoutName}

# Neural Network
Run a model on `MediumClassic` layout for 600 episodes, of which 500 episodes
are used for training.

--Running a Neural network with convulational networks
```
$ python pacmanNN.py -p PacmanDQNAgent -n 600 -x 500 -l mediumClassic
```
500 is the test set and 500 is the training data, smallClassic is the layout

