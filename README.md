# Bot Battlr

Welcome to **Bot Battlr**, the ultimate destination in the known universe for building your very own Bot Army! This is an overview of the project and its functionalities.

## Overview
This React application designed to allow users to browse a list of robots, view details about each robot, and enlist them into their personal army.
## Instructions

Follow these steps to set up and run the project:

1. Clone the project repository.
2. Navigate to the project directory in your terminal.
3. Run `npm install` to install the necessary dependencies.
4. Start the backend server by running `npm run server`.
5. Start the React app by running `npm start`.
6. Open [http://localhost:8002/bots](http://localhost:8002/bots) in your browser to verify that the backend is running correctly.

## Project Structure

- **BotPage**: The top-level component serving as the main container for the entire application.
- **BotCollection** and **YourBotArmy**: Container components responsible for displaying the list of available bots and the user's enlisted bots, respectively.
- **BotCard** and **BotSpecs**: Presentational components for rendering individual bot information in list and full view, respectively.

## Core Deliverables

```The User Can```

- View profiles of all bots in the `BotCollection`.
- Enlist a bot into your army by clicking on it. The enlisted bot will appear in the `YourBotArmy` component. Each bot can be enlisted only once.
- Release a bot from your army by clicking on it. The bot will be removed from the `YourBotArmy`.
- Permanently remove a bot from the service by clicking the red "x" button, deleting the bot from both the backend and the `YourBotArmy`.


#### GET /bots

Returns a list of available bots.

#### DELETE /bots/:id

Deletes a bot by its ID.

## Advanced Deliverables

- Display a detailed view (`BotSpecs`) for each bot instead of enlisting it immediately.
- Implement sorting functionality by health, damage, or armor using a `SortBar` component.
- Filter bots by their class, allowing multiple filters at once.
- Ensure that only one bot from each `bot_class` can be enlisted.

