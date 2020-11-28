# Machine Learning: How to make Quick Draw game using Convolutional Neural Network

A Javascript Machine Learning Project on making a game like **Quick, Draw!**. It is an online game that challenges players to draw a doodle and then artificial intelligence guesses what the drawings represent.

This repo contains source code for implementing this game step by step.

Here is the video in which I explained the entire project:  
https://youtu.be/AsYczuDBGp0  


## Project Info

The game is made in HTML5 using [Phaser 2 framework](https://phaser.io/) and [TensorFlow.js library](https://js.tensorflow.org/) for machine learning. 

To classify images, I implemented an **Artificial Intelligence (AI)** based on **Machine Learning (ML)** and **Convolutional Neural Network (CNN)**.

The model was trained on a small subset of the [Quick Draw Dataset](https://quickdraw.withgoogle.com/data).

Here is a screenshot of the fully completed project:  
  
![Doodle Predictor Screenshot](https://github.com/ssusnic/Machine-Learning-Doodle-Recognition/raw/master/screenshots/machine_learning_doodle_s1_640x360.png "Doodle Predictor Screenshot")

To play the game online, visit my official website:  
https://www.askforgametask.com/tutorial/machine-learning/quick-draw/

To read more tutorials and play my other games, check the homepage:  
https://www.askforgametask.com


## Running the Game

To play this game locally, you need to run it in a browser using a local web server as follows:

1. install, configure and run a web server: for instance, let's suppose your server is XAMPP installed in **C:\Xampp** 
2. navigate to the server document root: **C:\Xampp\htdocs**
3. create a new folder called 'doodle_predictor': **C:\Xampp\htdocs\doodle_predictor**
4. download the project
5. copy all project files directly in **C:\Xampp\htdocs\doodle_predictor**
6. now you should have the following folder structure under **C:\Xampp\htdocs\doodle_predictor**:  
	**\assets** (with game resources)  
	**\data** (with datasets)  
	**\libs** (with libraries)  
	**\part1** (with source files of the part 1)  
	...  

7. open a web browser and navigate to the **http\://localhost:\<port\>/doodle_predictor/part1**  
  to run the game of the part 1


## Parts of the Project

This project is divided into 8 parts.  
Each part contains a fully commented source code so you can easily follow the game development step by step.  

Here are short descriptions of each part:


## Part 1: Setup 

- creating the Main Program with the main state
- defining all substates of the main state
- building the basic game structure with the main loop where the entire game logic will be implemented
- creating a new User Interface class to allow users an interaction with the game


## Part 2: Getting Data
 
- creating a new CNN class for implementing a Convolutional Neural Network model
- loading three datasets (car, fish and snowman)
- splitting datasets into training and test data
- shuffling data


## Part 3: Building the Model
 
- creating a sequential CNN model
- adding layers to the model
- compiling the model


## Part 4: Training the Model

- fetching batches of data
- training, testing and evaluating the model
- plotting graphs of the model loss and accuracy during training


## Part 5: Predicting Samples

- fetching batches of samples 
- predicting fetched samples


## Part 6: Drawing Doodles

- creating a new Painter class to allow users to draw their own doodles with the mouse
- defining painting objects: drawing area, bitmaps, pencil
- adding a function for drawing a smooth line between two points using quadratic curves


## Part 7: Recognizing Doodles

- resizing doodle drawing to the required size of 28x28
- normalizing array of pixels before passing it as the input of the CNN model
- predicting doodle


## Part 8: Adding More Doodle Categories

- adding 10 doodle categories

