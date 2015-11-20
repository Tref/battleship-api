This application can be checked out and run separately on two different server instances:

The ember application residing in the battleship-ember directory can be started on port 4200 via:

```
ember server
```

and the rails application should be started on port 3000 via:

```
rails server
```

the two applications will communicate with each other via CORS (rails) and the content security policy
in the ember configuration. If you would like to change any of the default behavior, do so there.

***

## README

This README would normally document whatever steps are necessary to get the
application up and running.

#### Things you may want to cover:

- Ruby version
- System dependencies
- Configuration
- Database creation
- Database initialization
- How to run the test suite
- Services (job queues, cache servers, search engines, etc.)
- Deployment instructions
- ...

Please feel free to use a different markup language if you do not plan to run

    rake doc:app

***

### A Simplified Game of Battleship

#### The Goal

Build a game for a variation of Battleship that works via an API.

Traditionally, Battleship has different sized ships that are placed on the board, to keep it simple, our ships will take up a single cell.

#### The API should feature endpoints that will:

- Create a game
- Destroy a game
- Accepts coordinates for the player’s next move.
_ Returns the coordinates for the CPU’s next move.

#### For reference here’s how the game should work:
- The starting board will be 5x5.
- The player starts a game and places 10 ships on the board.
- The player submits their positions on the board via the API.
- The CPU places its ships on the board.
- The player is given the first move and submits coordinates to strike.
- If a ship is hit, it is destroyed.
- Allow the CPU to attack.
- Alternate moves between player and CPU.
- The first player to have all ships destroyed is the loser.

#### Keys of the Challenge
- Focus on building a clean API that uses semantically correct status codes and request methods (GET, POST, PUT, DELETE, etc).
- Build the UI as a web browser client (Ember would be great, but React/Angular as a client is fine too).
- Feel free to use whatever server-side technology you are comfortable with.

#### Bonus (optional)
- Add in user sessions so the server can handle more than one game at a time.
- Add a leaderboard that keeps winner’s initials and ranks them according to the time it took them to win.
- Deploy the application somewhere.

#### Take Aways
Please have fun with the challenge, don’t worry about visual design too much, but be proud of your submission. Enjoy! If you have any questions, feel free to contact us.

For further reference on Battleship: https://en.wikipedia.org/wiki/Battleship_(game)

