```text
  / ____| |               | |      |  _ \| |                     
 | |    | | __ _ _   _  __| | ___  | |_) | | __ _ _ __ ___   ___ 
 | |    | |/ _` | | | |/ _` |/ _ \ |  _ <| |/ _` | '_ ` _ \ / _ \
 | |____| | (_| | |_| | (_| |  __/ | |_) | | (_| | | | | | |  __/
  \_____|_|\__,_|\__,_|\__,_|\___| |____/|_|\__,_|_| |_| |_|\___|
                                                                   
  🔍 Finding which Claude instance wrote that shit! 🔍
```
Find git commits in conversations.json

usage: claude-blame [-h] [--conversations CONVERSATIONS] [--full] commit_hash

Find which Claude instance wrote that commit!

positional arguments:
  commit_hash           Git commit hash (partial or full)

options:
  -h, --help            show this help message and exit
  --conversations CONVERSATIONS, -c CONVERSATIONS
                        Path to conversations.json export (default: ~/Downloads/conversations.json)
  --full, -f            Search for full commit hash instead of first 7 characters

Examples:
  claude-blame abc123f
  claude-blame abc123f --conversations ~/Downloads/conversations.json
  claude-blame --full abc123f456def789  # Use full hash
