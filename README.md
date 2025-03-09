# Discord Automation Bot by @MeoMunDep

## Overview
This bot automates interactions on Discord, including sending messages, joining and leaving servers, and handling messages using multiple accounts with proxy support.

## Features
- **Auto Messaging**: Sends messages to specified channels.
- **Auto Join Servers**: Joins servers using invite links.
- **Auto Leave Servers**: Leaves specified servers.
- **Proxy Support**: Supports HTTP(S) and SOCKS5 proxies.
- **Auto Message Deletion**: Deletes sent messages after a configurable delay.
- **Multi-language Support**: Configurable message language.

## Installation
### Requirements
- **Node.js** (Version: `22.11.0`)
- **npm** (Version: `10.9.0`)

Download Node.js and npm here: [Download Link](https://t.me/KeoAirDropFreeNe/257/1462).

### Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/MeoMunDep/Discord-Autobot.git
   cd dirscord_autobot
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```
     If you encounter an Execution Policy error on Windows, run:
   ```bash
   Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
   ```
      Then, run the npm install command again.
3. **Configure the bot:**
   Edit `configs.json` to adjust settings.
4. **Prepare input files:**
   - `tokens.txt`: List of Discord tokens (one per line).
   - `chat_ids.txt`: List of channel IDs for messaging.
   - `proxies.txt`: List of proxies (one per line, optional).
   - `join_servers.txt`: List of Discord invite codes.
   - `leave_servers.txt`: List of server IDs to leave.
   - `messages.yaml`: Messages categorized by language.

## Configuration (`configs.json`)
| Setting           | Description                            |
|------------------|--------------------------------|
| `auto_chat`      | Enables/disables auto messaging |
| `delete_message` | Enables message deletion       |
| `join_server`    | Enables auto join servers      |
| `leave_server`   | Enables auto leave servers     |
| `language`       | Defines the language for messages |

Example `configs.json`:
```json
{
  "auto_chat": true,
  "delete_message": true,
  "join_server": true,
  "leave_server": false,
  "language": "en"
}
```

## Usage
Run the bot with:
```bash
node meomundep_discord.js
```

## How It Works
- Reads the configuration and input files.
- Logs into Discord accounts using tokens.
- Uses proxies (if provided) for each account.
- Executes configured tasks (messaging, joining, leaving servers).
- Handles errors and logs events with timestamps.
- Runs continuously in cycles with a countdown between runs.

## Logs and Timestamps
- Each log entry is prefixed with a timestamp.
- The timestamp format is based on the selected language in `configs.json`.

## Notes
- Make sure the tokens are valid and have the necessary permissions.
- Use proxies to avoid rate limits and bans.
- Running multiple accounts at once may require optimization.

## Contact and support
- **Buy me a telegram account** [Here](https://t.me/KeoAirDropFreeNe/312/27801) or [Here](https://github.com/MeoMunDep/MeoMunDep)
- **Contact:** [Contact Me](https://t.me/MeoMunDep)
- **Group:** [Join the Group](https://t.me/KeoAirDropFreeNe)
- **Channel:** [Visit the Channel](https://t.me/KeoAirDropFreeNee)

## License
This project is for educational purposes only. Use responsibly!

