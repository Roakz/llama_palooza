# roarkzprojects
![Llama Palooza Welcome](/pictures/welcome_page.PNG)

<h1>Application Development Plan</h1>

<h3>Contents</h3>

**1. Statement of Purpose and Scope**<br>
  **1.1** Purpose<br>
  **2.2** Scope<br>

**2. Programming Fundamentals Displayed (Ruby)**<br>
  **2.1** Variable types <br>
  **2.2** Classes & methods<br> 
  **2.3** Arrays<br>
  **2.4** Loops & Conditionals<br>
  **2.5** Error Handling<br>
  
**3. Features**<br>  

**4. User Guide**<br>
  **4.1** User instructions<br>
  **4.2** Game rules<br>

**5. Flow chart diagram**<br>

**6. App implementation**<br>

**7. Conclusion**<br>


<h2>1.Statement of Purpose and Scope</h2>

<h3>1.1 Purpose</h3>

Llama Palooza is being developed as part of my Fast Track coding bootcamp assessment criteria. This Application will demonstrate what I have learnt over the past 2 weeks and bring it all together, into an operational terminal application, in the form of a text based battle game.

<h3>1.2 Scope</h3>

**What will it do?** Llama palooza will be an interactive text based battle game that allows the user/player to choose from 3 Llama clan warriors. Each of these characters will have a varying level of attributes. The player will then enter battle with the Sloth Boss. The Sloth Boss's attributes will be randomly generated and the match will be displayed. The generation Of Sloth Boss's attributes will be within a fair scope to allow for fun and fair game play.

Once the match is displayed a heads and tails choice will go to the player and and the winner will start (either the player or sloth boss). Each player will take turns at attacking (randomly generated attack types) until a winner is apparent. The player will then have the option of playing again or exiting the game. If the player chooses to play again they can then choose if they want to change clans or continue with their current Llama. Sloth boss's attributes will be regenerated to ensure fair game play.

__Have fun!__

__What problem will it solve?__ This is purely for professional and personal development and to meet assessment criteria.

**Whos it for?** This game will be a bit of fun for anybody who enjoys text based game play. Also I hope that some of the methods and features included, within Llama Palooza, will help aspiring developers with their own projects. I also look forward to having access to the finished product to look back at for my own developmental purposes.

<h2>2. Programming Fundamentals displayed (ruby) </h2>

This application will use a range of features to demonsatrate my understanding of the basic principles of programming using the ruby language. Below is an outline of what will be used and where in the app.

<h3>2.1 Variable types</h3>
Llama palooza will need to use multiple variable types during the operation of the program. This program will be built mostly on classes that carry out methods and are called at appropriate times using composition to combine the output into the battle class where neccesary.<br><br> 
Instance variables will play a large role within the Llama and sloth Classes as well as the battle class to hold onto information required to carry out the specific methods. When this information needs to be held, outside of the class, Ruby program local variables will be used and the value of the instance variables returned.<br><br>

 This will assist with reducing unneccesary memory usage and only storing what is required when it is required. Being that this program heavily relies on classes and the calculations carried out in the methods within them.

<h3>2.2 Classes</h3>
As previously stated, in the variable type section, Classes will be a large part of this program. I am planning on structuring the game on 3 main classes. <br><br>

**The first class**  will be the Llama class. Within the llama class there will be 3 sub-classes that inherit directly from the Llama "superclass" to initialize the over-arching attributes of the llamas. Each llama will then have 1 special attribute which will be specified in the specific subclass. This will mean it takes precedance over the superclass for that particular attribute. Although i could have used modules for this i found this to be a DRY-er simpler approach.<br><br>

**The second class**  is the Sloth Boss class. Upon initialization the sloth class will randomly generate its attributes for each attribute area I.E Health, Attack & Hp. This will ensure fair and interesting game play.<br><br>

**Third and final**  will be the battle class. This will execute the battle when initalized and will be composed using the attribute output from the initialized llamas and sloth Boss. I believe that using a class for this is the easiest way to contain the methods and allows it to be called as many times as is needed without creating an abundance of code.<br><br>

<h3>2.3 Arrays</h3>
I will use arrays in 2 sections of the app. The first array used will be if the player wants to randomly generate their llama instead of choosing for themselves. This will be a simple 3 element array containing the three clans which a random sample will be taken from & retuned as a result.<br><br> 
The second use of arrays will be in the battle loop. During battle at each attack an attack description will once again be randomly sampled from the list stored within the array. The Sloth Boss will have its own array of attacks to keep it interesting. These attack descriptions wont effect who wins it is purely for user enjoyment and to keep it interesting. The attributes will mathematically decide who wins. Given more time it could always be updated to include additional attack points depending on attack types etc. However I wanted to demonstrate constraint in planning and carrying out a project.<br><br>

<h3>2.4 Loops and conditionals</h3>
The whole game will be contained within a "Loop DO" loop to ensure continuing game play whilst the player wishes to continue & a secondry Until loop nested within to loop if no new llama is requested. Part of the play on loop will allow an option to change Llama or remain the same. The main loop though will be the battle_loop.(contained within the battle class) This will use boolean operators to continue to loop "Until" a true is returned on a given condition (either players or sloth boss's HP is dimished). <br><br>
Conditionals will be used for selection at several points during the program. There will be a Case used to outline "when" conditions when choosing the laama, or randomize llama option. There us also If else statements contained within the battle class loop.<br><br>

<h3>2.5 Error Handling</h3>
Error handling will be developed through continuous (TDD) Test dirven development during development of this program and as issues are identified they will be resolved. The main areas that will be observed are anywhere that the user has input. I want to ensure that when inputs, other than what are requested, are entered an error will be returned and it will loop back for another opporunity for the user to input the request. <br><br>
 This will arise at picking the Llama clan, heads and tales, anywhere the user needs to press enter to continue, when the user is asked if they want to play again and, if they choose to play again, when they are asked if they want to change clan. <br><br>
From a development point of view i have installed the test-unit Gem which will be used to drive TDD during this project. All tests will be stored in a seperate directory within the projects parent directory. This will keep them accesible for future/continues development of this project. <br><br>

<h2>Features</h2>

Although there is a pretty good in depth look at the features from a users perspective below and a good inside look at the programming fundamentals displayed above in the programming fundamentals section. Here is a breif snapshot of a few of the features included and how they were implemented.

<h2>Randomize your Llama if you dont want to choose</h2>

You can let the computer choose a Llama for you! - This wasnt to difficult. I <br>

<h2>Flip a coin to see who starts</h2>

<h2>The battle loop</h2>

<h2>4. User guide</h2>

This guide will demonstrate how the user can access and use Llama palooza. The app will be presented in such a way that it will contain explicit instructions on how to play and be very easy to self navigate without much direction. each screen will prompt the user onto the next and the rules will be set out in an weasy to understand manner within the app and are also below for your convenience.

<h3>4.1 User instructions</h3>

**Start** <br>
To run the application you must have the latest version of ruby installed with the appropriate GEMS as referenced in the gem file when the repository is downloaded from GitHub. Enter the below command to run the program.<br><br>


![Start up](/pictures/startup.png)


**Exit** <br>
You can exit the application at any time by pressing "contol C"


<h3>4.2 Game rules</h3>
Llama Palooza is a text based battle game in which you will select your preffered Llama to battle the Sloth Boss.
Each Llama has different attributes so choose wisely! Once you have selected a llama the computer will generate the attributes of the Sloth Boss wihtin a fair range for fun and fair gameplay.<br><br>


__A.__ Select a llama from the profile page (choose carefully they all have different attributes which are listed on the selection page.) type your selection 1, 2, 4 or 4 and press ENTER to continue<br><br>


![Choose your Llama](/pictures/user_selection.PNG)<br><br>


__B.__ The computer will randomly generate your matchup and display the match up on screen. Its time to pick heads or tales. The winner gets the first attack! type 1 or 2 to make your choice and press ENTER to continue.<br><br>

![match up](/pictures/match_up.PNG)<br><br>


__C.__ The winner of heads and tails and therefore who will start will be displayed.Press ENTER to continue.<br><br>

![who starts](/pictures/who_starts.PNG)<br><br>


__D.__ The battle begins! press enter after each battle update to continue.<br><br>

![Start up](/pictures/start_battle.PNG)<br><br>


__E.__ If you choose to play on you will be given an option to select a new llama or cotinue with your current selection. Simply enter the appropriate y/n selection and press enter to continue!<br><br>

![Start up](/pictures/play_again.PNG)<br><br>

![Start up](/pictures/new_llama.PNG)<br><br>


__There is only one rule....Have Fun!!!__

<h2>5. Flow chart diagram</h2>

Below i have attached a flow chart diagram which explains the sequential and conditional flow of the game.
I have used a very basic flow control diagram model. The oval indicates the beggining and end, the rectangle is a process and the diamand indicates a decision.All arrows are labelled to indicate which decision was made.

![Flow control](/pictures/flowchart.PNG)

<h2>6. App Implementation</h2>
In order to display efficient project managment & time management skills i will use a free internet tool called Trello. (www.trello.com) This is a great tool that allows me to plan out a to do list, a doing list, and review list and a done list. I have also created some boards in trello for my user stories. The user stories are part of the planning stage that help a developer look at a project from all user angles. This should help create a well rounded product.

<h2>7. Additions & improvements</h2>
In working my way through the design and build of this app alot of refining was done at each stage to help  ensure "agile" workable code. I set out with the goal for it to be as DRY as possible and improvable in the future. Some easily achievable additions to the game would be Multiple sloth's with different attributes, Different attack points for different attacks, a choice of attacks instead of a randomized scenario, a randomisation of the players stats, special in game bonuses for either player just to name a few. It has been designed in such a way that changes to the numbers mathematically should not break the code or require mass searches through code to look for updates. As everything is calculated in methods using the required initial data.

<h1>Hope you enjoy! Feel free to send Feedback on code improvements!!</h1>