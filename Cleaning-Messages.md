### How do I clean messages?
* To clean messages, simply use the `>>clean` command, along with parameters for what you want to clean

### Parameters
These parameters can be provided in any order, and multiple parameters can be used at once. Running the command with 3 parameters is the same as running the command 3 times, each with one of those parameters.
* `<numPosts>` - number of posts to delete; between 2 and 1000; default is 100
* `bots` - cleans messages by bots
* `embeds` - cleans messages with embeds
* `links` - cleans messages containing links
* `images` - cleans messages with uploaded or embeded images or videos
* `@user` - cleans messages only from the provided user
* `<userId>` - cleans messages only from the provided user (via id)
* `"quotes"` - cleans messages containing the text in quotes
* `` `regex` ``  - cleans messages that match the regex

Remember, for numPosts, @user, and userID, you use the value you want. For bots, embeds, links, and images, you use the literal words "bots", "embeds", "links", and/or "images". For quotes or regex, surround the text you want to clean in either quotes (") or grave accents (\`)

### Examples
* `>>clean bots images 500` - In the past 500 messages, cleans all messages by bots, as well as all messages that contain images
* `>>clean links @jagrosh` - In the past 100 messages, cleans all messages that contain links, as well as all messages by jagrosh
* `>>clean bots "!" embeds` - In the past 100 messages, cleans all messages by bots, all messages that contain an exclamation point (!), as well as all messages that contain embeds
* `>>clean 200` - Cleans all of the past 200 messages