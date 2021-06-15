# Maze Task: A Minimum Working Example

## The Maze Task

This repository contains everything one needs for a simple maze task implementation, designed to be deployed in the web browser. This task requires participants to progress through a sentence one word at a time, much like a self-paced reading study, but with distractor items that force the participant to select the correct (i.e. grammatical) continuation of the sentence.

## Features of this Implementation

This version of the maze task includes randomizing of within-item conditions, as well as the randomization of the names of characters in vignettes, but obviously your own implementation can do away with these if need be.

Also included in this version are two practice questions. I strongly recommend keeping two practice trials, due to the fact that this task is significantly less intuitive than a standard self-paced reading time study. The first of these examples will automatically highlight the correct word if the participant selects the wrong one, as well as display the ungrammatical sentence they have constructed in so doing. The second example will only inform them that they have selected the wrong word, then ask them to try again.

Additionally, each trial contains an attention check question. Each sentence pair in the main trial has a number of possible questions that can be asked with differing answers, but you can simplify these questions if need be; this might even be advantageous, as the maze task has a substantially higher rate of attention-check failure than a SPRT.

Finally, note that this implementation of the maze task forces participants to move on to the next trial if they incorrectly continue a sentence. This results in the entire sentence being tagged as unanswered, so that it can be excluded from analysis, but still logs the data. This can be advantageous if, for example, the participant fails the continuation AFTER the critical region, and you still want to include that critical item in the analysis. There is a way to make it so that participants will be able to continue on even after pressing the wrong word, or retry. I hope to include this feature in an upcoming release.

Best of luck with your research, and do feel free to reach out to me with any questions.
