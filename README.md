query_dpla
==========

<a href="https://twitter.com/QueryDPLA">QueryDPLA</a> is a Twitter bot that searches the <a href="http://dp.la">Digital Public Library of America</a> for a term tweeted at it, picks one of the first five results at random, and tweets the item's title and URI back to the querier. QueryDPLA is written in Python 2.7. It uses <a href="https://github.com/tweepy/tweepy">Tweepy</a> to communicate with the Twitter API and <a href="https://github.com/bibliotechy/DPyLA">DPyLA</a> to communicate with the <a href="http://dp.la/info/developers/codex/">DPLA API</a>.

<h2>Known Issues (in process of being fixed)</h2>
<ul>
<li>The program is unable to parse unicode characters and may crash upon encountering one.</li>
<li>The bot is unable to distinguish between search terms and references (e.g. if someone tweets "@QueryDPLA (some message about it rather than intended for it)", the bot will search for all text in the tweet that comes after "@QueryDPLA" and reply accordingly.</li>
</ul>
