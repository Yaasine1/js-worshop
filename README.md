# JavaScript workshop

This workshop is about creating a simple instant-chat web application to get started and have a little nose dive with JavaScript\*0.

What are you talking about ?!
We could notice that every day, we communicate through different channels and in many forms, from just writing down a note to someone or for ourselves to get reminded, having a phone call, setting up a timer on the oven or even more prestigious as talking to a rover on another planet.

All these, lets say interactions, have a lot of things in common from a communication standpoint, and could be modeled (maybe over simplified) as:
Actor_A ---message-----> Actor_B
Actor_A <-----message--- Actor_B

first thing, we could label what we want to note or communicate as the "message" or "source information" or name it whatever you want, this "information" has to be stored somewhere (in the human brain, on a piece of paper, on a wall... you name it) base line here, the information must exist and it has to be reachable [for this we're going to use MongoDB\*2 this is where we are going to store our precious information].

This "Actor_A" is simply the initiator of the conversation, is also the emitter of the message, briefly the sender of the information (this Actor, write's an idea on a note, set's a time period on the oven's timer...).
In a world shared between humans and machines if this Actor_A is a human and like's to send some information to Actor_B and it happens that Actor_B is a machine we would need a human-to-machine interface (a fancy way of saying screens, buttons, switches, knobs...), in this world we need a some tools to build an interface that a human understands and could interact with (for this project we're using React\*1 to show some forms and cats photos on an internet browser that supports JavaScript).
"Actor_B" here is the receiver of the message, this actor is our destination when "Actor_A" send's some data as this actor is the machine in this scenario (we're going to use Node.js\*3 )

"Actor_A" and "Actor_B" both could be machines, in a situation like that we use or make API's (a subject for another time)

What are we making here ??
this project will try to realize an implementation of ReactJS framework as the front-end through it the user could interact with:

- sign up form:
  [ userName ] : text-input
  [ password ] : password-input
  [ repeatPassword ] : password-input

  ( createAccount ) : button - when clicked should send the form data to the server
  ( Sign in ) : button - when clicked should display's the sign in form

- sign in form:
  [ userName ] : text-input
  [ password ] : password-input

  ( Sign in ) : button - when clicked should send the form data to the server
  ( createAccount ) : button - when clicked should display's the sign up form

- change password form:
  [ userName ] : text-input
  [ password ] : password-input
  [ repeatPassword ] : password-input

  ( updatePassword ) : button - when clicked should send the form data to the server
  ( Sign in ) : button - when clicked should display's the sign in form

- create room form
  [ roomName ] : text-input

  ( createRoom ) : button - when clicked should send the form data to the server
  ( cancel ) : button - when clicked abort's the current action

- edit account form
  [ userName ] : text-input
  changePassword : when clicked should display's the change password form

  [ changeStatus v ] : dropdown-input
  deleteAccount : when clicked should display's a confirmation dialog

  ( saveChanges ) : button - when clicked should send the form data to the server
  ( cancel ) : button - when clicked abort's the current action

- edit room form
  [ roomName ] : text-input

  deleteRoom : when clicked should display's a confirmation dialog
  ( saveChanges ) : button - when clicked should send the form data to the server
  ( cancel ) : button - when clicked abort's the current action

- confirmation dialog
  ( confirm ) : button - when clicked should confirm the action
  ( cancel ) : button - when clicked abort's the current action

###

\*0 : JavaScript is a scripting or programming language that allows you to implement features on web pages (see more at https://developer.mozilla.org/en-US/docs/Web/JavaScript, https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript)

\*1 : React (also known as React.js or ReactJS) is a front-end JavaScript library for building user interfaces based on UI components. (see more at https://en.wikipedia.org/wiki/React_(JavaScript_library), https://reactjs.org/docs/getting-started.html)

\*2 : MongoDB is document-oriented database program (see more at https://en.wikipedia.org/wiki/MongoDB, https://github.com/mongodb/mongo, https://university.mongodb.com)

\*3 : Node.js is a JavaScript runtime environment that runs on the V8 engine (this V8 engine is what's makes the Chrome browser ticks) and executes JavaScript code outside a web browser (see more at https://en.wikipedia.org/wiki/Node.js, https://nodejs.dev/learn, https://nodejs.org/en/about/).

where can i start ??

download vs code
generate a private and a public keys

open a terminal on macOs or cmd on windows and type
$ ssh-keygen

## client: ReactJS application

## server: expressJs based nodeJs server and application

## design: ui/ux, design pattern

## documentation: documentation about the environment setup

## tests: tests scripts
