# Python-RAT

An Python Remote Administration Tool that works on Discord.
Supports multiple exploitation commands.

# Features

    !help - Help command
    !ping - Ping command
    !cd <path> - Change directory
    !ls - List directory
    !download <file> - Download file
    !upload <link> - Upload file
    !shell <ps> - Execute shell command
    !run <file> - Run an file
    !exit - Exit the session
    !screenshot - Take a screenshot
    !tokens - Get all discord tokens
    !startup - Add to startup

# Setup

## Installing required packages

```bash
pip install -r requirements.txt
```

## Creating the bot

Please go to [Discord Developer Portal](https://discord.com/developers/applications) and create an New Application,
then you need to enter a name like C2 or C&C server. go to Bot in the left sidebar, Press Add Bot Reset The token and put it in [Configuration](##configuration)

## Configuration

Open config.json and fill in your discord token and guild id,
DM me on ``Jeff_#2475`` for help. Example shown below.

```json
{
    "token": "Your discord bot token",
    "guild_id": "The guild id of the C2 server"
}
```

# Compiling to an Executable

To compile this tool to an executable please install an Python compiler like nuitka, pyinstaller or pyarmor pack.
Here is an example of compiling with Pyinstaller

## Installing Pyinstaller

```bash
pip install pyinstaller
```

## Compiling Source

```bash
pyinstaller --onefile --add-data="config.json;." main.py 
```