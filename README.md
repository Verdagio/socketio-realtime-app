# Connect 5 app
Note: the server side code was taken and modified from the boilerplate project which can be found in my [Github Repo](https://github.com/Verdagio/tsc-express-api)

## Getting started
git clone me! then grab the submodules with 
```git submodule update --init```

Then make sure you have docker installed 

## Tech
This app is built using the following technologies:
 1. Angular
 2. Node
 3. Typescript
 4. Docker
 5. Express
 6. Socket.IO
 7. Mocha & Chai

## Project Summary
### Connect 5 app
This is a fairly simple project to experiment and learn a little about realtime app development. 

It contains a simplistic angular client and a typescript-node express / socket.io server / api.

2 players can connect and play a game of connect 5.

### Summary

The choice to use these technologies is to make maximum use of Typescript across both the client side and server side codebase. Both the client and server side is containerised to simplify running the applications on any environment, all you need is Docker.

The client uses rxJs observables and observers for realtime communication with the server so that when events are carried out on one client, the other will be updated appropriately.

This was the first time using both rxJs & socket.io but was a really interesting task to have realtime comms for each client connected. 

I feel the observables and observers simplified the front end services calling out to the server and vice versa though I feel I didn't utilize them to the best of their ability.

Likewise with Socket.io on the back-end I would have liked to add a bit more abstraction into my code base like that which is in the source repo which I referenced above but was aware of the timeframe.

The mocha tests written were to verify functionality of serverside logic, unfortunately I did not carry out any front end tests as I have limited experience with this.

### Future improvements
 1. I spent little to no time styling this thing... looks like something straight out of 2001, with more time I would probably use Angular material or bootstrap to make the app look astetically pleasing. 
 2. I'd also use a html canvas to draw out the game board.
 3. Better use of abstraction throughout the project
 4. Better use of the rxJS observables & observers.
 5. Test the client side code-base...

## Running the project!
Please see each individual readme for specific commands.

To run all pieces of the project:
```docker-compose up --build```