## How to Play the game.

1. Use arrow keys to move the player and collect the candies.
1. Try to collect the candies in the minimum number of moves possible.

### Rendering random sprites
For each row, one column is randomly selected and a candy is placed in it.

## Assumptions

1. Number of candies is equal to `boardSizeY`.
1. If boardSizeY is 10, then the initial row position of player is 5.

## Bot
A bot using puppeteer has been created to solve the game. On completion, the bot will create a screenshot in root called `completed-game.png`.
### Running the bot
To run the bot run the following command from the project root.
```
node ./bot/complete-game

```

This will run the bot using the [hosted instance](https://trick-or-treat.netlify.com)

#### On custom domain
You can run the bot pointing to another domain by passing it as a CLI argument.
Example to run on localhost:8080

```
node ./bot/complete-game http://localhost:8080
```

The bot should now point to `localhost:8080`

## Local Setup for contribution

1. Fork the repo and clone your forked repo.
1. Create a branch for the feature named `username-featurename`.
1. Run `npm i` to install libraries and tool the project uses.
1. Run `npm run start` to start game.

## Contributors Guide

1. Please create an Issue or comment on existing issue before sending a PR.
1. Make sure all tests are passing. This can be done locally by running `npm run test`. Tests are also run via CI and you'll get a build status right on the PR itself.
1. Run `npm run format` before the final commit.
1. Allow [edits from maintainers](https://help.github.com/en/articles/allowing-changes-to-a-pull-request-branch-created-from-a-fork) on the PR.
