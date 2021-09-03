# Avalon: The Resistance Logs

https://avalongame.online/ is a site that allows friends to play Avalon: The Resistance in person or via videoconference.

This repository contains JSON-formatted logs of thousands of games from the site.

The log file format is not documented here, but is self-explanatory.

# Insights

Evil wins about 55% of the time (6835 / 12228 games).

Of those wins, Merlin was assassinated 41% of the time (2801 / 6835 games). That means that an evil team successfully assassinates Merlin about 1/3rd of the time (2801 out of 8194 attempts).

## Merlin

In games *without* the Merlin role (ie, the barebones Resistance game), evil has a win percentage of about 50%.

What a great balance! So what happens when we add the powerful Merlin role? Turns out the odds of the good team passing 3 quests goes all the way up to 68% of all games! How great for the good team, right? Except... the odds of the evil team winning actually *increase* from 50% to 57%. If you've played Avalon, you shouldn't be surprised. With Merlin in the game, evil now has a powerful assassination ability, which allows them to eke out a win even after the good team passes 3 missions. In fact, a successful Merlin kill contributes to about 44% of all evil wins.

Based on the stats above, it would seem that the base Resistance game is the more balanced game with its 50-50 good-evil win rate. And yet, an overwhelming 92% of the games played on the site are Avalon games, not Resistance. (Perhaps Avalon is simply the more fun game to play, even if it's not as balanced?)

Now, back to Merlin. Just how vulnerable is he? In games with 5 players, when the Assassin selects a target, Merlin gets killed a whopping 40% of the time!

Merlin is safer with more players, getting killed only about 30-35% of the time at player counts of 6 through 8, dropping to a low of 29% with 9 players. This is still about 2x the expected rate if the evil players were picking out an assassination target completely at random: this shows that evil players are generally pretty good at spotting Merlin, and that being Merlin is quite a dangerous job.

The longer the game goes on, the more likely it is that Merlin will get killed at the end. There's a clear correlation between the total number of quests attempted and how likely Merlin is to get killed. If the good players manage to sweep the game by passing 3 quests in a row starting from the very first mission, Merlin has only about a 1/3rd chance of getting killed. But if it takes good players 5 missions to get 3 wins, Merlin has an almost 50% chance of dying. This makes intuitive sense -- if it takes the good players 5 tries to get 3 successes, it often forces Merlin to become really obvious to make sure the 5th mission is a success, which is also much more likely to give him away.

The only thing that can save Merlin is perhaps the second most powerful role in the game...

## Percival

I expected to see that the Percival gets assassinated instead of Merlin a fair bit (that's kind of his job, after all!), and was surprised to see that it's not the case. In fact, Percival gets assassinated at about the same rate as non-special players on the good team, and the presence of Percival doesn't reduce the odds that Merlin gets killed.

Nevertheless, including Percival in the game does improve the odds of the good team winning by about 5%. It seems that Percival is able to meaningfully reduce the odds that the evil team is able to sabotage 3 missions, even if he's unable to reduce the odds of Merlin being killed.

The other special roles deserve a quick look too:

Having **Oberon** in the game improves the good team's chances by 3-4%. **Mordred** or **Morgana** each improve the evil team's win rate by about the same amount (3-4%).

# Other ideas for data exploration

* Examine whether different cohorts of players have different game meta as evidenced by stats
* Examine how the length of the game in wallclock time affects stats
* Examine whether some players are better in some roles than others (probably not enough of a sample size)
