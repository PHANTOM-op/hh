> ⚠ **Filtering features are currently in beta, and are not yet available for most servers.**

## 🚯 What are filters?
Filters are customizable words (or word patterns) that can have varying numbers of strikes (🚩) associated with them. When a user sends a message containing a filtered word, their message is deleted and they receive the corresponding number of strikes.

## 🚯 Filter Items
A filter is made up of one or more items. Each item can be a word, a quote, or a regex (regular expression), and any combination of these can be used in a single filter. In the following examples, green means a sentence would get filtered (and deleted/striked), and red means the sentence would not get filtered.
### Words
When no special syntax is provided, items in the filter list are treated as words. Words are checked for in a message, taking into account word boundaries.
Example:
```
>>filter add WordExample 1 photos* 
```
```diff
+ The plant performed Photosynthesis
# This is filtered because any word starting with 'photos' is filtered

- I took a photo of the plant
# This is not filtered because this uses the word photo, not a word starting with photos

- Telephotosoft is a weird name for a company
# This is not filtered because only words starting with 'photos' are filtered, but 'Telephotosoft' doesn't start with 'photos'
```
### Quotes
When a word or phrase is surrounded in double quotes (`"`), the exact quote (except for case-sensitivity) is checked for in the message. This ignores word boundaries and checks anywhere within the message and even within words.
Example:
```
>>filter add QuoteFilter 1 "connect"
```
```diff
```
### Regular Expressions
When a word or phrase is surrounded in grave accents (`` ` ``), the word or phrase is treated as a regular expression. This is checked for anywhere in the message.
Example:
```
>>filter add RegexFilter 1 `https?://.*`
```
```diff
```

## 🚯 Filter FAQs
`Q:` **What can I filter?**  
`A:` You can filter words, quotes, or regular expressions. Please see the sections below 

`Q:` **Can a filter be set to zero strikes?**  
`A:` Yes, setting a filter to zero strikes will cause messages containing the word to be deleted, but no strikes will be assigned and no warning DMs will be sent.

`Q:` **What happens if a message hits multiple filters?**  
`A:` Only the filter with the highest strike count will trigger.

`Q:` **Who do filters apply to?**  
`A:` Filters apply to the same users that all automod features apply to; filters will ignore anyone with a role higher than Vortex's highest role or any role that is on the `>>ignore` list.

`Q:` **Why can't I set filters?**  
`A:` Filters are not released to the public yet. If you'd like to be notified when they are public, please join [my development server](https://invite.gg/jagrosh) and type `%roleme Vortex Updates` in a testing channel.