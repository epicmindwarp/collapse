# collapse
Bot for a reddit sub that requires the OP to provide a statement for link posts within a set time frame

# Requirements
- Python 3.7+
- praw 6.3.1+
- config file (included)
- Login details, and bot client id and secret, placed inside config file (not included)

# Tested on
- Windows 10
- Raspberry Pi 3B+

# How to

1) Download collapse.py and config.py and place them into the same folder
2) In config.py, place your bot login details (U+P), and your client ID and client secret from reddit API
3) In collapse.py, you need to set the following configurations at the top of the script
   - Subreddits to watch over (multreddits are okay, but untested)
   - User Agent - use a better description, or leave as is
   - Number of hours before a post is removed
   - Reply comment body for the bot to reply with
   - Number of seconds to sleep between checks (default to 5 minutes for most subs is fine)
   - RGX - This is regex - don't touch this if you don't understand this
