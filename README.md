What If?
=======

I always wanted to collect statements around "What if I had done blah blah", thinking of the possible timelines that we avoided (or wished were true). So I decided to search through twitter for tweets with a phrase above, and maybe compile it into a book of regrets. But *without using code*.

##Wait, what is this NaNoGenMo?

This is the second edition of *National Novel Generation Month*, that @dariusk started (organized?) last year. Read more about the [NaNoGenMo here](https://github.com/dariusk/NaNoGenMo-2014). Major updates (& hopefully feedback) on my project at [NaNoGenMo 2014 issue #88](https://github.com/dariusk/NaNoGenMo-2014/issues/88).

##Collecting Data
Using IFTTT to collect data. Created a recipe [to search tweets & generate a json](https://ifttt.com/recipes/219769-search-tweets-and-generate-a-json). Using a json instead of csv because I'm slightly unsure about extra commas in the tweet messing up the import.

Search query #1: ("what if I had" OR "What if you had" OR "What if she had" OR "What if he had")
Search query #2: ("what if" had)

Saved as: 
```json
{"tweet": "{{Text}}", "created_at": "{{CreatedAt}}", "user": "{{UserName}}", "user_dp": "{{UserImageUrl}}", "link": "{{LinkToTweet}}"},
```

Current data dump (updated daily) on [what-if-had-v2.txt](https://github.com/rasagy/what-if/blob/master/what-if-had-v2.txt)

##Example data

Here are some (hand-picked) tweets from the first 12 hours:

* What if you had to do all that I do, unnoticed, and all alone? Would you still have the same attitude?
* What if I had it. Would I be the best?
* What if I had those answers you needed!
* What if she had no one to talk to or seek attention from? What would she do?
* What if I had one more night for goodbye

##ToDo

* Keep a check on SPAM. Keep updating query with possible keywords that you want to filter
* Take a shot at one piece of json and see how it imports in Excel
* Think about design & random elements
