![Screenshot_2](https://github.com/user-attachments/assets/1739ed0b-e4b4-431d-8bb4-7238bac5c426)

---

# BlitzTweet

Welcome to the ultimate Twitter automation tool!  
This is a licensed tool and can be purchased by contacting [MrGrassss](https://t.me/MrGrassss).

## Features:

- Mass Tweet Replier
- Avatar Changer
- Banner Changer
- Bio Changer
- DisplayName Changer
- Tweet Liker
- Tweet Replier
- Mass Follower
- Mass Retweeter
- Mass Posts Shiller
- Client Checker
- Equal Follower
- Website Changer
- Clear Tweets
- Mass Tweeter
- MassDM
- Scraper

## Future:

- Any feature can and will be added on demand

# Extra Functionality Info

## Login & Setup

- **Note:** Each functionality includes prompts to guide you through any prerequisites needed for it to work. This means
  you can use any function without having to follow a strict order.

- **Proxies:** Supports sticky/rotating proxies in the following formats:
    - `HOST:PORT@USERNAME:PASSWORD`
    - `HOST:PORT:USERNAME:PASSWORD`
    - `HOST:PORT`

- **Tokens:** Format should be either:
    - `username:pass:email:email_pass:auth:ct0`
    - `username:pass:email:ct0:auth`
    - `auth:ct0`
    - `auth`

- **Files:**
    - `mass_replies/keywords.txt` expects one keyword per line.
    - `replies/comments.txt` expects one comment per line; ensure you have more comments than clients.
    - `post_shiller/usernames.txt` expects one username per line; one client will listen to one username.
    - `post_shiller/comments.txt` expects one comment per line; same comments won't get reused so make sure to have a
      lot.
    - `mass_replies/media` stores media files for replies.
    - `mass_replies/messages.txt` contains the messages to reply with.
    - `mass_replies/tagged_users.txt` includes one username per line for users to be tagged.

- **Removed Tokens:** Saved in `acc_checker/removed_tokens.txt`.
- **Locked Tokens:** Saved in `acc_checker/locked_tokens.txt`.

## Account Functionalities

- **Avatar Changer:** Change the avatar of your Twitter accounts.
- **Banner Changer:** Update the banner image for your profiles.
- **Bio Changer:** Modify the bio of your Twitter accounts.
- **DisplayName Changer:** Change the display name of your profiles.
- **Website Changer:** Change the website of your profiles. Must be a valid url so either "name.com"
  or "https://name.com"

## Tweet Actions

- **Tweet Liker:** Automatically like tweets.
- **Tweet Replier:** Reply to tweets based on specified keywords.
- **Mass Tweeter:** Sends out the same tweets with as many accounts as you want.

## Mass Actions

- **Mass Tweet Replier:** Bulk reply to multiple tweets fetched by keywords set in `mass_replies/keywords.txt`.
- **Mass Follower:** Follow multiple accounts in bulk.
- **Mass Retweeter:** Retweet tweets in bulk.
- **Mass Posts Shiller:** Listens to new posts and shills mass comments to them and likes + rts these comments with idle
  accounts.
- **Mass Tweeter:** Post tweets with media and tagged users in bulk.

## Mass Tweet Replier

### Overview:

The Mass Tweet Replier feature automates the process of replying to multiple tweets based on specified keywords,
using a list of predefined replies.

### Prerequisites:

1. **Proxies:** Ensure proxies are set up correctly in the supported formats.
2. **Tokens:** Use the correct format for your Twitter account tokens.
3. **Files:** Prepare the necessary files:
    - `mass_replies/keywords.txt`: Contains the keywords to search for tweets.
    - `mass_replies/message.txt`: Contains the reply messages.
    - `mass_replies/media`: Store any media files you want to include in the replies.
    - `mass_replies/tagged_users.txt`: Include usernames to be tagged in your replies (one per line).

### Setup:

1. **Keywords File:** Populate `mass_replies/keywords.txt` with the keywords you want to search for in tweets.
2. **Replies File:** Populate `mass_replies/messages.txt` with the reply messages.
3. **Media Directory:** Place any media files you want to use in `mass_replies/media`.
4. **Tagged Users File:** Populate `mass_replies/tagged_users.txt` with the usernames to be tagged in replies.
5. **Replied Tweets File** Replied tweets are saved in `mass_replies/replied_tweets.txt` to keep track of tweets that
   have been responded to, avoiding duplicate replies.

### Limitations:

- A maximum of 4 media items in total (images, GIFs, and videos combined) can be used per tweet.
- Tagging users through media only works on non-verified and public users.
- 100 Tweets per hour per token, tokens that reach this will be automatically removed.

### How to Use:

1. **Run the Mass Tweet Replier:** Launch the feature from the main menu.
2. **Search and Reply:** The tool will search for tweets containing the keywords from `mass_replies/keywords.txt`,
   and reply with messages from `mass_replies/messages.txt`. Emojis are supported in the messages, and you can mark the 
   end of a message with "---". Clients will never search on the same keywords and are automatically divided.
   This will run forever till all clients are dead or have reached their 100 daily time limit.
3. **Include Media and Tags:** If configured, the tool will attach media files from `mass_replies/media` and tag users
   in media from `mass_replies/tagged_users.txt`.

### Example:

1. Add keywords to `mass_replies/keywords.txt`:
   ```
   #keyword1
   #keyword2
   ```

2. Add replies to `mass_replies/message.txt`:
   ```
   Great insight!
   Thanks for the info!
   Really useful post!
   ```

3. Add media files to `mass_replies/media` directory (if any):
   ```
   image1.jpg
   video.mp4
   ```

4. Add tagged users to `mass_replies/tagged_users.txt`:
   ```
   user1
   user2
   user3
   ```

5. Ensure your proxies and tokens are configured properly.

6. **Run the Mass Tweet Replier:** The tool will process the replies and save the replied tweets in a log file. The
   replies will be handled, skipping any already processed tweets.

## Mass Tweeter

### Overview:

The Mass Tweeter feature automates the process of posting tweets with media files and tagging specified users.

### Prerequisites:

1. **Proxies:** Ensure proxies are set up correctly in the supported formats.
2. **Tokens:** Use the correct format for your Twitter account tokens.
3. **Files:** Prepare the necessary files:
    - `mass_tweeter/media`: Store your media files in this directory.
    - `mass_tweeter/message.txt`: Contains the message to be tweeted.
    - `mass_tweeter/tagged_users.txt`: One username per line for the users to be tagged.

### Setup:

1. **Media Directory:** Place the media files you want to tweet in `mass_tweeter/media`.
2. **Message File:** Populate `mass_tweeter/message.txt` with the tweet message.
3. **Tagged Users File:** Populate `mass_tweeter/tagged_users.txt` with the usernames to be tagged.

### Limitations:

- A maximum of 4 media items in total (images, GIFs, and videos combined) can be used per tweet.
- Tagging users through media only works on non-verified and public users.

### How to Use:

1. **Run the Mass Tweeter:** Launch the feature from the main menu.
2. **Select Media:** The tool will prompt you to select the number of images, GIFs, and videos to use (If there is more
   than one gif or video else it’s automatic), ensuring the total does not exceed 4 media items.
3. **Post Tweets:** The tool will read the message, media files, and tagged users, and post tweets accordingly.

### Example:

1. Add media files to `mass_tweeter/media` directory (randomly selected):
   ```
   image1.jpg
   image2.png
   image3.gif
   video.mp4
   ```

2. Add message to `mass_tweeter/message.txt`:
   ```
   Check out our latest updates! 😁
   ```

3. Add tagged users to `mass_tweeter/tagged_users.txt`:
   ```
   user1
   user2
   user3
   ```

4. Ensure your proxies and tokens are configured properly.

5. Run the Mass Tweeter and let it handle the rest!

## Equal Follower

**Description:**

The Equal Follower feature allows you to distribute a list of usernames across multiple Twitter accounts,
ensuring that each account follows a unique set of users without any overlap.

**How It Works:**

1. **Upload Usernames:**
    - Fill `equal_follower/usernames.txt` with the usernames you want to follow. (1 per line)

2. **Set Parameters:**
    - Specify the number of tokens (Twitter accounts) to use.
    - Define the number of usernames each token should follow.

3. **Distribute Follows:**
    - The Equal Follower will allocate usernames to each account sequentially, ensuring no duplicates.

**Usage Example:**

- You have a `usernames.txt` file of 500 usernames.
- You want to use 10 accounts, each following 50 users.
- Equal Follower will ensure each of the 10 accounts follows a unique set of 50 users.

**Caution**

- A fresh account can follow up to 50 people per day and a

warmed-up account up to 80.

## Mass DM

### Overview:

Automate sending direct messages to users scraped by the scraper feature or to a list of specified usernames or user
IDs.

### Prerequisites:

1. **Scraped Users:** Ensure users are scraped and saved in `scraper/user_info.json`.
2. **Usernames:** Alternatively, add usernames to `mass_dm/usernames.txt` or user IDs to `mass_dm/user_ids.txt`.
3. **Proxies:** Ensure proxies are set up correctly in the supported formats.

### Setup:

1. **Message Configuration:** Set up in `mass_dm/config.json` and `mass_dm/message.txt`. Emojis can be added like this
   ❤️.
2. **Attachments:** Store images and videos in `mass_dm/media`, one will be randomly selected.
3. **Use Scraped Users:** Set "use_scraped_users" to "true" in `mass_dm/config.json` to use users from
   `scraper/user_info.json`.

### How to Use:

1. **Run the Mass DM:** Launch the feature from the main menu.
2. **Configure Timing:** Set `seconds_before_dm` and `dm_limit_per_acc` in `mass_dm/config.json`. Instagram's daily DM
   limit is 100.
3. **Send Messages:** The tool will read the message configuration and attachments, and send DMs accordingly.

### Results:

- Successful messages are saved to `mass_dm/processed(user_ids/usernames)/success.txt`, and failed ones
  to `mass_dm/processed(user_ids/usernames)/failed.txt`. Duplicates are skipped on rerun.

## Suggestions / Feedback

I'm open to any suggestions or feedback!

For questions, you can always contact me on [Telegram](https://t.me/MrGrassss).

---
