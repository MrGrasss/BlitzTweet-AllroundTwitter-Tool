![Screenshot_1](https://github.com/MrGrasss/BlitzTweet-AllroundTwitter-Tool/assets/132838549/db31b208-8707-4359-a337-ce46c5d7cde0)

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

## Future:

- Any feature can and will be added on demand

# Extra Functionality Info

## Login & Setup

- **Note:** Each functionality includes prompts to guide you through any prerequisites needed for it to work. This means you can use any function without having to follow a strict order.

- **Proxies:** Supports sticky/rotating proxies in the following formats:
  - `HOST:PORT@USERNAME:PASSWORD`
  - `HOST:PORT:USERNAME:PASSWORD`
  - `HOST:PORT`
  
- **Tokens:** Format should be either:
  - `username:pass:email:auth:ct0`
  - `auth:ct0`
  
- **Files:** 
  - `mass_replies/keywords.txt` expects one keyword per line.
  - `replies/comments.txt` expects one comment per line; ensure you have more comments than clients.
  - `post_shiller/usernames.txt` expects one username per line; one client will listen to one username.
  - `post_shiller/comments.txt` expects one comment per line; same comments won't get reused so make sure to have a lot.

- **Removed Tokens:** Saved in `acc_checker/removed_tokens.txt`.
- **Locked Tokens:** Saved in `acc_checker/locked_tokens.txt`.

## Account Functionalities

- **Avatar Changer:** Change the avatar of your Twitter accounts.
- **Banner Changer:** Update the banner image for your profiles.
- **Bio Changer:** Modify the bio of your Twitter accounts.
- **DisplayName Changer:** Change the display name of your profiles.

## Tweet Actions

- **Tweet Liker:** Automatically like tweets.
- **Tweet Replier:** Reply to tweets based on specified keywords.


## Mass Actions

- **Mass Tweet Replier:** Bulk reply to multiple tweets fetched by keywords set in mass_replies/keywords.tx.
- **Mass Follower:** Follow multiple accounts in bulk.
- **Mass Retweeter:** Retweet tweets in bulk.
- **Mass Posts Shiller:** Listens to new posts and shills mass comments to them and likes + rts these comments with idle accounts.

## Mass Posts Shiller

### Overview:
The Mass Posts Shiller feature automates the process of monitoring new posts from specified usernames, posting multiple comments on these new posts, and liking and retweeting these comments using idle accounts.

### Prerequisites:
1. **Proxies:** Ensure proxies are set up correctly in the supported formats.
2. **Tokens:** Use the correct format for your Twitter account tokens.
3. **Files:** Prepare the necessary files:
   - `post_shiller/usernames.txt`: One username per line. Each client will listen to one username.
   - `post_shiller/comments.txt`: One comment per line. Ensure you have more comments than clients to avoid reuse.
   - `post_shiller/idl_tokens.txt`: Store your idle tokens here.

### Setup:
1. **Username File:** Populate `post_shiller/usernames.txt` with the usernames whose posts you want to monitor.
2. **Comments File:** Populate `post_shiller/comments.txt` with the comments to be used.
3. **Idle Tokens:** Ensure your idle tokens are stored in `post_shiller/idl_tokens.txt`.
4. **Configure Proxies:** Set up proxies as needed.

### How to Use:
1. **Run the Mass Posts Shiller:** Launch the feature from the main menu.
2. **Monitor New Posts:** The tool will start monitoring new posts from the specified usernames.
3. **Shill Comments:** Once a new post is detected, the tool will post comments from `post_shiller/comments.txt`.
4. **Like and Retweet:** The tool will use idle accounts from `post_shiller/idl_tokens.txt` to like and retweet these comments to boost engagement.

### Example:
1. Add usernames to `post_shiller/usernames.txt`:
   ```
   user1
   user2
   user3
   ```

2. Add comments to `post_shiller/comments.txt`:
   ```
   Great post!
   Very informative.
   Thanks for sharing!
   ```

3. Add idle tokens to `post_shiller/idl_tokens.txt`:
   ```
   auth1:ct0
   auth2:ct0
   auth3:ct0
   ```

4. Ensure your proxies and tokens are configured properly.

5. Run the Mass Posts Shiller and let it handle the rest!

## Suggestions / Feedback

I'm open to any suggestions or feedback!

For questions, you can always contact me on [Telegram](https://t.me/MrGrassss).

---
