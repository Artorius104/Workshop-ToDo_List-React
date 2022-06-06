# Workshop-ToDo_List-React

# Installation process

- Download nodeJs via :

    Official Website :
    
        https://nodejs.org/en/
 
    Package manager : 
    
    Arch Linux :
        
         pacman -S nodejs npm

    Fedora :
        
         sudo dnf module install nodejs:16
    
    Ubuntu :
        
         curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
         sudo apt-get install -y nodejs

    For another operative system :
    
        https://nodejs.dev/download/package-manager/

Finally, check the installation with node -v

  - Then, create your React application with the following line :
  
        npx create-react-app <my-app>

<my-app> being the name of your application.

Once it is done, go inside newly created directory and run the application with : npm start
Your application is set and ready to bu used !

For useful graphical assets, we recommend you to install the React framework's Material-ui, which contain UI tools to help you ship new features faster :
  
        npm install @mui/material @emotion/react @emotion/styled
        npm install @mui/icons-material
  
You'll find everything you need on the react official website https://reactjs.org/ and mui official website https://mui.com/ .

# Tic Tac Toe Game
    
The first part of this workshop is about making a simple tic tac toe game. We'll focus on implementing only the necessary part of the game.
Your application is going to be written in inside "App" inside index.js.
    
# STEP 01
    
Create a "Game" class which will contain our main implementation of the game, inside, use the "render" method to display your jsx.

Then, create a "Board" and "Square" functions which will return nothing for the moment.
"Square" will be called by "Board" which itself will be called by "Game".
    
# STEP 02

Using "Board" and "Square", display three rows of square.
You can use this CSS code for the squares :
    
        .square {
            background: #fff;
            border: 1px solid #999;
            float: left;
            font-size: 24px;
            font-weight: bold;
            line-height: 34px;
            height: 34px;
            margin-right: -1px;
            margin-top: -1px;
            padding: 0;
            text-align: center;
            width: 34px;
        }

Then, display the status of the game on top of the board with the following status : "Next player: X".
You can create your own methods and use it to display one square at a time.
    
# STEP 03

Try to send numbers from 0 to 8, from "Board" to "Square" using a method. Display those values inside the squares.

To send values from a component to another means sending arguments from a parent component to his child(dren). To use the argument(s) in the child: "props" is your friend.
    
# STEP 04
    
Now we want to display an 'X' when we click on a square. To do this, think about onClick and useState or this.state.

States, are somethings that you are going to use all the time. It is going to be useful to maintain the value of each of the 9 squares in one location. They are declared as constant.

Create a state in "Board" and send it's value to "Square".
    
# STEP 05
    
In Board, create a state which will contain an array. This array will represent all of our squares.

Create a function handleClick(i) in "Board" which will modify the element i from the array.

This function will be called each time we click on a square. Is there a way for a child component to use a function of the parent ?

Remember, a state is not a regular variable and is constant. Do you know how to modify a state ? Look for "Immutability" and guess why it is important.
    
If "Square" is using states from itself, find a way to remove them so that the component uses only states' information from the parent. If you did so, good job, keeping the state of all squares in the Board component will allow it to determine the winner in the future.

Since the Square components no longer maintain state, the Square components receive values from the Board component and inform the Board component when they’re clicked. In React terms, the Square components are now controlled components. The Board has full control over them.
    
# STEP 06
   
We're almost done ! Our Tic Tac Toe looks good but there's only one player...

Create a new state to determine to either put an 'X' or an 'O' depending the player.
    
Changes wil also be handled by handleClick function.
    
Change the status displayed accordingly.
    
# STEP 07
    
One more thing remaining, decides when a game is finished and who the winner is.
   
Still inside the Board component, declare a "winner" variable which will contain the return value of the "calculateWinner" funcion. This create that function which will take our array representing the squares as argument will obviously return if a winner has been decided.
    
    
We're all set !
You're game is finished but still pretty simple...
What if I want to restart my game ? Or if I want to come back to a specific move ? Look for more or continue on this workshop with the next exercise.


# To Do List application

The second and last part of the workshop will be making a to do list with react.

With all you've seen in the last exercise, you have everything to make you're own application.
    
Although I have no doubt you can make something pretty with CSS, if you want to make a professional and beautiful looking To Do list, you'll find EVERYTHING YOU NEED in Material-ui !
    
Material-ui is a React framework to beautify your applications, some of it's assets will be familiar to you and it is simple to use.

To do list are widly use in job interviews and are a good exercise to show your skills about the demanded language. Don't hesitate to implement as many functionnalities as possible and to post it on your GitHub or social medias.
    
# Thank you for doing this workshop, and may the To Do list be with you !
