# Dopest-DD-Alpha-Edition
Alpha Testing of Dopest DD for Penny Stocks
## What is Dopest DD?
Curious about penny stonks? Too lazy to do your own research? Perhaps you even read DD (research) posts on reddit penny subs. Well, we are too lazy to even read the DD on penny subs. We would prefer to have a magic machine read it and tell us if it is the Dopest DD or not. So we built a magic machine to do exactly that and decided to give it away for free! 

Dopest DD is a telegram bot that automatically finds the top ranked authors of penny stonk DD (research) posts on reddit in real time and sends 'virtual portfolio' summaries of their DD posting history, including the *1 day, 5 day, and until now percent gains* of each stonk from the date and time they posted each DD. Sound too complicated? Maybe you want to know more? 


## How does Dopest DD work?
You like penny stonk DD (research) posts on Reddit subs like [r/pennystocks](https://www.reddit.com/r/pennystocks/) or [r/RobinHoodPennyStocks](https://www.reddit.com/r/robinHoodPennyStocks/)? Dopest Financial does too! So we decided to find out 'who makes the dopest DD posts'. How? By creating 'virtual portfolios' for every author of a DD post and searching their posting history for previous DD posts. This way as an author makes a new post, we can gather their virtual portfolio of stonks and rank their portfolio on its total gains. We filter out all the authors with a sub-par track record, then we send those results out with a telegram bot in real time. 

### 1 day, 5 day, until now percent change?
Every penny stonk is evaluated based on the percent change from the date and time of the original DD post until 1 day later, 5 days later, and until the date and time of the evaluation. So you can think of these as 3 columns. 

#### Why these days, why percent, why not highs/lows?
Well, we cannot predict the future so we cannot know in advance when the high/lows will be of a stonk. The idea of picking 1 day, 5 day, and until now is based on the following strategy: *If a person were to take all of the positions of the poster's history and blindly sold after 1 day, 5 days, or held until now, what would be their total gains?* The days were selected based on experimentation of different time intervals and to optimize the turn around time of the analysis (historical DD posts of authors must be at least 5 days old). 

#### What about when a post is made and the market is closed?
We calculate the last price avalible to avoid any issues. 


### The filter criteria
* A post is DD when it has either
  * DD in the title
  * or it has a DD flair (DD, research, catalyst, or bullish)
* DD post must have a ticker in the title (with or without '$')
* Author must have at least two analyzable penny stonks
   * Posted at least 5 days ago
   * Stonks must be listed on Yahoo Finance (we use `yfinance` to collect the analytics of the stonk)
   * Penny stonks are all stonks under $5
* One of the total percent (1 day, 5 day, or until now) gains of their virtual portfolio must be at least 20%
* And must have at least 60% correctness (60% of their stonks returned at least 1% gains) 
* And the average gain percent must be at least 5%

to be selected as Dopest DD. These parameters are subject to change during the alpha testing phase.

Every time an author posts a DD post with a ticker in the title, Dopest DD collects their virtual portfolio (up to the last ten DD posts) of all tickers and analyses them, if the DD is the dopest, we pass along the virtual portfolio via telegram bot. That's it.

## It's really free?
Yes. Currently, we are in the alpha testing phase. We are only allowing 100 people to try out Dopest DD. After we are done with alpha testing, we will move to beta testing with more people. This will also be totally free to anyone. Finally, once we are done with our test phases, the telegram bot will STILL be free. We will NEVER sell this as a service. We believe in supporting those penny stonk communities by freely giving access to this analysis tool. 

## Is this project open source?
Yes and no. We don't want to release any code before we have finished our alpha and beta testing. We want to make sure what we have done is up to the standards of the open source community. However, after this we will be more than happy to open source the Dopest DD virtual portfolio filtering system. Transparency is very important to us. We want everyone to know how we perform our analysis and how we come to our results of the Dopest DD. 

## Okay, this is awesome how can I use Dopest DD?
As stated, we are in an alpha testing phase currently. So the best thing would be just to write us for the id of the telegram bot. Once the alpha and beta test phases are complete, we will provide the telegram ID to everyone.
`dopestfinancial at protonmail dot com`

## Who is Dopest Financial?
We are [Bartmoss](https://github.com/AmateurAcademic), [Maxwell](https://github.com/maxwhoppa), and [Milan](https://github.com/MilanLR). Three people who saw a [post on WSB](https://www.reddit.com/r/wallstreetbets/comments/li5vch/i_think_i_found_a_way_to_predict_dips_with_nasdaq/) wrote in the comments with each other and decided to check out the claim together. Although the [original author's hypothsis didn't lead anywhere](https://github.com/AmateurAcademic/WSB-President-Wolfe-Hypothesis), we decided to jointly investigate other oppertunities. That is when Dopest Financial was born. We have been working on Dopest DD in our free time ever since.

## Warnings and important stuff
We are not giving any finical advice. The bot is provided as is. We assume no liability. Also, we are most likely stupid or something…
