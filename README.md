# Dopest-DD-Alpha-Edition
Alpha Testing of Dopest DD for Penny Stocks
## What is Dopest DD?
Curious about penny stonks? Too lazy to do your own research? Perhaps you even read DD (research) posts on reddit penny subs. Well, we are too lazy to even read the DD on penny subs. We would prefer to have a magic machine read it and tell us if it is the Dopest DD or not. So we built a magic machine to do that and decided to give it away for free! 

Dopest DD is a telegram bot that automatically finds the top ranked authors of penny stonk DD (research) posts on reddit in real time and sends 'virtually portfolio' summaries of their DD posting history, including the 1 day, 5 day, and until now percent gains of each stonk from the date and time they posted the DD. Sounds complicated? Maybe you want to know more? 


## How does Dopest DD work?
You like penny stonk DD (research) posts on Reddit subs like [r/pennystocks](https://www.reddit.com/r/pennystocks/) or [r/RobinHoodPennyStocks](https://www.reddit.com/r/robinHoodPennyStocks/)? Dopest Financial does too! So we decided to find out 'who makes the dopest DD posts'. How? By creating 'virtual portfolios' for every author of a DD post and searching their posting history for previous DD posts. This way as an author makes a new post, we can gather their virtual portfolio of stonks and rank their portfolio on its total gains. We filter out all the authors with a sub-par track record, then we send those results out with a telegram bot in real time. The filter criteria is:
* DD post must have a ticker in the title (with out without '$')
* Author must have at least two analzible stonks
  * Posted at least 5 days ago
  * Stonks must be listed on yahoo finance
* One of the total percent (1 day, 5 day, or until now) of their virtual portfolio must be at least 20%
* That same total percent must have at least 60% correctness (60% of their stonks returned at least 1% gains)
* The average gain must be at least 5%

to be labeled Dopest DD.

Every time an author posts a DD post with a ticker in the title, Dopest DD collects their virtual portfolio of all tickers and analzyses them, if the DD is the dopest, we pass along the virtual portfolio via telegram bot. That's it.

## Its really free?
Yes. Currently we are in the alpha testing phase. We are only allowing 100 people to try out the telegram bot. After we are done testing the bot, we will move to beta testing with more people. This will also be totally free to anyone. Finally once we are done with our test phases, the telegram bot will STILL be free. We will NEVER sell this as a service. We believe in supporting those penny stonk communities by freely giving access to this analysis tool. 

## Is this project open source?
Yes and no. We don't want to release any code before we have finished our alpha and beta testing. We want to make sure what we have done is up to the standards of the open source community. However, after this time we will be more than happy to open source the Dopest DD virtual portfolio system. Transparency is very important to us. We want everyone to know how we perform our analysis and how we come to our results of the Dopest DD. 

## Okay, this is awesome how can I use Dopest DD
As stated, we are in an alpha testing phase currently. So the best thing would be just to write us for the id of the telegram bot. Once the alpha and beta test phases are complete, we will provide the telegram ID to everyone. We are even considering making a reddit bot too. 

`dopestfinancial at protonmail dot com`
