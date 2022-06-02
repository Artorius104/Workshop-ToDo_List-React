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

    - Définition des différentes steps -
    Présentation des props -> composants intéractifs -> immutabilité

Our game is now finished, but maybe too simple. Feel free to add some functionnalities to add flavor to the game such as a movement history !

# To Do List application

The second and last part of the workshop will be making a to do list with react.
To do list are widly use in job interviews and are a good exercise to show your skills about the demanded language.
Just like the tic tac toe game, we'll focus on the basic parts for this workshop.

    - Définition des différentes steps -
    Focus sur les useStates
    
Our To do list is now complete. Just like tic tac toe, feel free to add functionnalities to sow off !
