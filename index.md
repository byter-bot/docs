# Introduction
!> This document is still WIP, and some info may be missing

Also check out the [beta bot](https://discord.com/api/oauth2/authorize?client_id=743302147927441459&permissions=388160&scope=bot)

Need help? Join the [support server](https://discord.gg/ZKHjRcy9bd)!

# Commands
?> Below are listed all current commands as of the stable bot, with additional info as to the bot's
help command. <br> **Note:** `[argument]` and `<argument>` are used for required and optional arguments
respectively

## Fun
### 2048
Starts a 2048 minigame

**Syntax:** `b!2048 <size>`

| Command  | Aliases | Arguments |
| -------- | ------- | --------- |
| `b!2048` | None    | `<size>`: board size between 2 and 8 |

### cat
Fetches a random cat image

**Syntax:** `b!cat`

| Command | Aliases | Arguments |
| ------- | ------- | --------- |
| `b!cat` | None    | None      |

## Info
### ping
Pong!

Shows current bot ping / latency

**Syntax:** `b!ping`

| Command  | Aliases | Arguments |
| -------- | ------- | --------- |
| `b!ping` | None    | None      |

### time
Gets current time in given timezone, or UTC offset

Refer to [this link](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones)
for available timezones, near-equal queries also work

**Syntax:** `b!time [timezone]`

| Command  | Aliases | Arguments |
| -------- | ------- | --------- |
| `b!time` | None    | `[timezone]`: Name of the timezone or UTC offset |

### whatis
Tries to fetch & gather info about an ID

Currently supports members & users, servers, channels and emotes

**Syntax:** `b!whatis [id]`

| Command    | Aliases | Arguments |
| ---------- | ------- | --------- |
| `b!whatis` | `b!?`   | `[id]`: an user, server, channel or emote ID |

## Stats
### stats
Shows multiple statistics for the bot

**Syntax:** `b!stats`

| Command   | Aliases | Arguments |
| --------- | ------- | --------- |
| `b!stats` | None    | None      |

## Text
### base64decode
Decodes given base64 text

**Syntax:** `b!base64decode [text]`

| Command          | Aliases    | Arguments |
| ---------------- | ---------- | --------- |
| `b!base64decode` | `b!b64dec` | `[text]`: base64 text to decode |

### binarydecode
Decodes given binary text

**Syntax:** `b!binarydecode [text]`

| Command          | Aliases    | Arguments |
| ---------------- | ---------- | --------- |
| `b!binarydecode` | `b!bindec` | `[text]`: binary text to decode |

### fullwidth
ｗｉｄｅ

Formats your text using full-width characters

**Syntax:** `b!fullwidth [text]`

| Command       | Aliases  | Arguments |
| ------------- | -------- | --------- |
| `b!fullwidth` | `b!mono` | `[text]`: text to format |

### hashtext
Hashes given text with chosen algo

You can list available algorithms by running the command without arguments

**Syntax:** `b!hashtext <algo> <text>`

| Command      | Aliases  | Arguments |
| ------------ | -------- | --------- |
| `b!hashtext` | `b!hash` | `<algo>`: algorithm to use |
|              |          | `<text>`: text to hash |

### regex
Matches an regex pattern against text

**Syntax:** `b!regex [pattern] [text]`

| Command   | Aliases | Arguments |
| --------- | ------- | --------- |
| `b!regex` | `b!re`  | `[pattern]`: pattern to use |
|           |         | `[text]`: text to match |

### sregex
Matches and replaces an regex pattern against text

**Syntax:** `b!regex [pattern] [text]`

| Command    | Aliases | Arguments |
| ---------- | ------- | --------- |
| `b!sregex` | `b!sre` | `[pattern]`: pattern to use |
|            |         | `[replacement]`: text to replace with |
|            |         | `[text]`: text to match |

### base64encode
Encodes given text to base64

**Syntax:** `b!base64encode [text]`

| Command          | Aliases             | Arguments |
| ---------------- | ------------------- | --------- |
| `b!base64encode` | `b!base64`, `b!b64` | `[text]`: text to encode |

### text2binary
Encodes given text to binary ascii

**Syntax:** `b!binaryencode [text]`

| Command          | Aliases             | Arguments |
| ---------------- | ------------------- | --------- |
| `b!binaryencode` | `b!binary`, `b!bin` | `[text]`: text to encode |

### textimg
Converts an image to text / ascii art

An image should be attached to the message - links aren't supported as of now

**Syntax:** `b!textimg`

| Command     | Aliases      | Arguments |
| ----------- | ------------ | --------- |
| `b!textimg` | `b!asciiart` | None      |

### unicodeinfo
Gives info about an unicode character

Query could be the character, it's (full) name or unicode point (hexadecimal value)

**Syntax:** `b!unicodeinfo [query]`

| Command         | Aliases | Arguments |
| --------------- | ------- | --------- |
| `b!unicodeinfo` | `b!uc`  | `[query]`: character, name or unicode point to query |

## Utils
### embed
Generates an embed with color, title and description

**Syntax:** `b!embed <color: #5050fa> [title] [description]`

| Command   | Aliases | Arguments |
| --------- | ------- | --------- |
| `b!embed` | `b!emb` | `<color>`: embed color, defaults to #5050fa |
|           |         | `[title]`: embed title |
|           |         | `[description]`: embed description |

### embedraw
Generates an embed using raw JSON data

You can refer to [this link](https://leovoel.github.io/embed-visualizer/) for testing an embed
before sending the command, and to learn about possible fields

**Syntax:** `b!embedraw [data]`

| Command      | Aliases  | Arguments |
| ------------ | -------- | --------- |
| `b!embedraw` | `b!embr` | `[data]`: json data to be used |

### poll
Create a poll with title, description and options

Options should be split by commas, if none then default to thumbs up / down

**Syntax:** `b!poll [title]; <description>, <emote>: <option 1>, <emote>: <option 2>...`

| Command  | Aliases | Arguments |
| -------- | ------- | --------- |
| `b!poll` | None    | `[title]`: Title for the poll |
|          |         | `<description>`: Description for the poll, should be after an `;` |
|          |         | `<emote>: <option X>`: Option name for the poll, optionally with an custom emote |

## Web
### wikipedia
Searches wikipedia

| Command       | Aliases  | Arguments |
| ------------- | -------- | --------- |
| `b!wikipedia` | `b!wiki` | `<limit>`: Maximum amount of results to show (1-25), defaults to 4 |
|               |          | `<query>`: Text to search |
