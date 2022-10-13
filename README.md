# Haqq alarm script

**Usage:** Set the required values in the script

LOCAL_RPC = "localhost:26657" - RPC of your validator node

TRUSTED_API = "https://haqq.api.t.stavr.tech" - Reliable API service
VALOPER = "" - Your valoper address
ADDRESS = "" - Your key address
HEX_ADDRESS = "" - Yor Hex Address
CRITICAL_BLOCKS_GAP = 25 - The maximum number of blocks by how much it is permissible to lag behind
CRITICAL_PEERS_COUNT = 5 - Critical number of peers
UPTIME_WINDOW = 500 - Number of blocks for uptime calculation
TELEGRAM_TOKEN = "" - Your telegram token
TELEGRAM_CHAT_ID = "" - Chat id for receiving messages

**Run one time: **
_python3 haqq_alarm.py_

**Run via crontab once every ten minutes (edit crontab with crontab -e):**
_1,11,21,31,41,51 * * * * python3 $HOME/haqq_alarm.py >> $HOME/haqq_alarm.log 2>&1_
