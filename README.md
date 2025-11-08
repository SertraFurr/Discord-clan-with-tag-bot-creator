# Discord Clan With Tag Creator Bot

- No need to buy goofy scammer, just use it in the background

# USELESS ALL DISCORD SERVER HAVE ACCESS TO THIS

## Overview

This bot automatically creates Discord servers and checks if they meet specific criteria based on a MurmurHash3 calculation of the server ID to get Discord clan tag
 
## Features

- Automatically creates Discord servers with customizable names
- Find server that has tag availability
- Automatically deletes servers that don't meet the criteria

# How to transfer

- 2 ways :
  - discordBotClient [discordBotClient](https://github.com/aiko-chan-ai/DiscordBotClient) (May lead to a bot ban)
Or
  - Use `transfer.py` to be able to transfer it (Coming soon)

## Requirements

- Python 3.9+
- discord.py library
- A Discord bot token with the proper permissions

## Installation

1. Clone this repository or download the script
2. Install the required dependencies:

```bash
pip install discord.py
```

3. Edit the script to include your bot token and customize settings

## Configuration

Edit the following variables in the script to customize behavior:

- `TOKEN`: Your Discord bot token
- `SERVER_NAME`: The name given to created servers (default: "Tag server")
- `DELETE_DELAY`: How long to wait before deleting an unwanted server (default: 2 seconds)
- `INTERVAL`: Rate limit interval between creation attempts (default: 120 seconds - DO NOT REDUCE)

## Usage

1. Set up your Discord bot in the [Discord Developer Portal](https://discord.com/developers/applications)
2. Run the script:

```bash
python main.py
```

4. The bot will continue creating and checking servers until it finds one that meets the criteria

## How It Works

The bot uses a MurmurHash3 algorithm to calculate a hash value from the server ID. It specifically looks for servers where:
- The hash value is between 10 and 19, OR
- The hash value is between 60 and 99

This corresponds to specific hash patterns that mean having a discord clan tag experiment inside of it

## Warnings

- Using this bot may potentially violate Discord's Terms of Service
- Use at your own risk
