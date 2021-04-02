# Exercise 8 - Event driven programming

## Learning Goals

This exercise targets the understanding of the following subjects:
* To get a taste of event-driven programming (15.1).
* To describe events, event sources, and event classes (15.2).
* To define handler classes, register handler objects with the source object, and write the code to handle events (15.3).
* To define handler classes using inner classes (15.4).
* To define handler classes using anonymous inner classes (15.5).
* To simplify event handling using lambda expressions (15.6).
* To write programs to deal with MouseEvents (15.8).
* To create images using the Image class and to create image views using the ImageView class (14.9).

## Description

In this exercise, we will implement a GUI for the card game Battle. In this game, two players are drawing cards from a deck of cards. A round consists of each player drawing one card. The winner of the round is the player who picks up the higher card. This player is awarded one point. Once the points are awarded. The cards are discarded and the players draw another card until the deck is empty.

## Instructions

1. Create a class `BattleGame` in package `aup.cs.games`.
2. The class should contain a javafx application.
3. The application should contain a top pane and a center pane.
4. The top pane shows the scores of the two players as well as a reset button.
5. The central pane should show the main deck of cards as well as the card drawn by each player for the current round.
6. When the user clicks with the mouse pointer on the central deck, the two top cards are drawn and displayed on each side of the deck.
7. The player with the higher card is scored one point
8. Each card should be represented by an image. [Please use these images](img.zip)
9. The main deck is represented by the card back (155.gif)
10. Once there are no more cards in the deck the scene should change to show a message "Player x has won, please click on the screen to start a new game" where x represents the player who has won (1 or 2).
11. Clicking on the screen will start a new game, similar to the result of pressing the reset button.
12. Please make sure to shuffle the deck when starting a new game
13. Make sure to style and layout your game in a nice way

## Further information

* For shuffling the deck, you can use the `Collections.shuffle` method
* For loading images, you should place them in folder `src/main/resources` and use an `Image` and `ImageViewer`.
* You can use a `LinkedList<Integer>` for holding the cards. `LinkedList` can also be shuffled as above and you can remove top elements. Note, that the faces of the cards are numbered 101-152.
