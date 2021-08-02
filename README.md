# Slippi Stats Application
## about
This repository contains three submodules that link to the three components of this application

1. SlippiOverlay - the Electron application that handles file management and window tracking
2. SlippiStatsBackend - the graphql/postgreSQL backend for my website
3. SlippiStatsWebsite - all of the front end code that handles the UI of the app using React/Next.js

This application is still a work in progress so things that look incomplete are just placeholders that will be fixed in time.

## Demonstration

The first thing you will see when you run the app is the green navbar that appears at the top of the game window. From here you can login to your account or register a new account. In the video you will see me demonstrate the tracking ability of the overlay. Then i will login/logout and then attempt to register as a user that already exists. Once I am logged in as chris3 you will see the stats page that is currently uninitialized as we have played no games. The overlay can be toggled on and off by pressing 'e'

https://user-images.githubusercontent.com/65579262/127787704-d6f3b2a9-97cc-4c55-8338-39ce544b2458.mp4

When a user creates an account for the first time, they also need to do some initial setup for the app to function. with a key bind (currently ctrl+o) the user opens a prompt that asks for the location of their game folder and which characters the user prefers to play as. Once the user submits their answers the application stores this info, but it can be changed at any time by simply hitting the key bind again. 


https://user-images.githubusercontent.com/65579262/127787773-48555569-6275-4184-9d46-21eac72b9253.mp4

After setting up the app all that needs to be done is hit the key bind for processing stats (currently shift+e). On the right you will see the Slippi folder where all my games are stored. The application will process all these files and then move them into a new folder it creates called old_games. Users are then free to delete the old games as the cumulative stats from those games are stored by the app allowing users to gain back several gigabytes of space since most players have thousands of these files in this folder. Once the files are processed you will see the stats page update with the statistics for your most recently played game along with some aggregate stats for all your games.

https://user-images.githubusercontent.com/65579262/127787825-2aeb8346-3c43-435f-9f2f-6b5031b0dbd7.mp4


In this last video I show that you can navigate to the friends page by either clicking the icons in the top left or by cycling through the icons using the arrow keys. I also show the way the app restructures its content based on the size of the window. Since no user is going to play this game on a phone there's no reason to handle screen sizes much smaller than shown.

https://user-images.githubusercontent.com/65579262/127787821-2678591c-d11c-43a2-b4c2-eb6785970d21.mp4






