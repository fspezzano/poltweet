# poltweet
Twitter Interaction networks among Members of the U.S. Congress

This repository contains the Twitter interaction networks among members of the U.S. Congress (from 112th Congress to 115th Congress) used in the paper 
"Chamberlain J.M., Spezzano F., Kettler J., Dit B., A Network Analysis of Twitter Interactions by Members of the U.S. Congress. 
Accepted for publication in the ACM Transactions on Social Computing journal (2020)."

If you use this data, please cite our paper.

For each chamber (House and Senate), we modeled interactions (retweet, @mention, quote) using directed graphs. Each politician is representedby a node. 
For each node, the following information is provided: twitter_account, first and last name, party, inferred party, DW_nominate score, state, Twitter account, 
and tweet count.

For instance:
{'dw_nominate': 0.556, 
'filtered_tweet_count': 557, 
'first_name': 'Paul', 
'inferred_party': 'R', 
'label': '18916432', 
'last_name': 'Ryan', 
'party': 'R', 
'state': 'WI', 
'twitter_account': 'SpeakerRyan'}

For each network, outbound edges represent an action that was initiated by the node. In our @mention graphs, edges are drawn from the node that authored 
a tweet to each node that was @mentioned. In our retweet graphs, edges are drawn from the node that sent the retweet to the node that was retweeted. 
Around 2015 Twitter added the quote feature (also known as “retweet with comment”). We construct quote graphs, where edges are drawn from the node that 
sent the quote to the node that was quoted. 
