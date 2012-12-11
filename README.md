What is this?
-----------
This is a plugin for IntelliJ IDEA which reverts active change list every N minutes. Looks like this:

<img src="https://github.com/dkandalov/auto-revert-plugin/blob/master/toolbar.png?raw=true" alt="auto-revert screenshot" title="auto-revert screenshot" align="left" />
<br/><br/><br/><br/>
It can be installed using IntelliJ plugin manager (Settings -> Plugins).<br/>



Why?
-------------------
 - to teach yourself proper TDD. Set up auto-revert to 2 minutes or so. Focus only on one part of red-green-refactor cycle. (See http://jamesshore.com/Blog/Red-Green-Refactor.html or http://butunclebob.com/ArticleS.UncleBob.TheThreeRulesOfTdd)
 - to limit work-in-progress. Auto-revert forces you to commit or lose changes. If committed changes are at least compilable, you won't get involved in big bang refactorings and code changes. It's like Pomodoro but you have to finish something. (http://en.wikipedia.org/wiki/Pomodoro_Technique)
 - not to be too attached to your code. If it's reverted, just write again and probably it will be better this time. (See http://blog.jayfields.com/2009/03/kill-your-darlings.html)
 - it's fun because it's like arcade computer game.
 - it's an experiment to see your limits.


How to use it?
--------------
 - choose how often to revert changes in Settings -> VCS auto-revert
 - start auto-revert (alt+shift+A or click on widget in the toolbar)
 - work on a feature:
   - if your changes auto-reverted before you finish and commit,
     start over and probably think how to make smaller steps
   - if you finish and commit before you run out of time, timer will be reset.
 - if you use really small time intervals (like 2 or 5 minutes), there won't be much
   time to write commit messages. In this case "Quick commit" action can be useful (ctrl+alt+shift+K).


Dedicated to LMAX people.