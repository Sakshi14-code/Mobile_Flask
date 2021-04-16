Mobile Flash Cards
This mobile flash card application is submission for the Udacity React Nano Degree Course

# To Run application:
-clone repository 

# Installs below dependencies for the project to run
npm install
npm install @expo/vector-icons --save

# optional: if you don't have expo installed, use ) 
npm install -g expo-cli

# Start Application 
expo start 
-scan the expo QR code with your android expo app (You'll need to download this first) OR run on a virtual machine on your computer OR plug in your android device and run emulator.

Note :  if you got any issue related to 'font awesome' or fontFamily 'Ionicons' when it is loaded First time on screen , igonore it and click on back button of mobile, after that it will show Home page which conatins Existing Deck List and New Deck Button, use further and explore the application 


Application has been tested on Android using the expo app, mobile device should be on same network. once the QR code is scanned wait for some time , it will bundle and then display the home screen which consist Home and NewDeck.
Click on new deck to creat new deck, enter the new deck name and once done , go to home it will display deck list, you can choose any deck to add question.
To start quiz , deck should contains questions.

# Description
This is a mobile application flashcard application created using React Native. Create Decks of questions and quiz yourself using the
option to add quiz cards, quiz yourself and delete Decks. This application uses Async Storage so studying can be done offline!


## Folder Structure

After creation, your project should look like this:

```
mobile-flash-cards
    README.md
    package.json - dependancey for tha app
    app.json
    App.js - entry point for the application, StackNavigator and Tab nav are created here
    src
        actions
            index.js - contains all actions for adding a deck and a card it used for redux
        components
            AddCardView.js - Form to add a question card to a specified deck
            AddDeckView.js - Form to add a new deck to the local database
            DeckDetailsView.js - Detailed view of the deck from here you can stgart a quiz or add a card
            DeckListView.js - List of decks that have been added to the app
            QuizView.js - View to display question, answer and result fo the quiz
            TextButton.js - a reusable Text Button that can change apperance based on the style you pass to it.
        reducers
            index.js - reducers used by redux to store and modify state
        utils
            colors.js - list of hex colors used for the application
            deckData.js - initial data added for the first two decks
            StorageAPI.js - API used to get, add and modify a deck 
