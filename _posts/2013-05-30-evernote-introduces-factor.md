---
layout: post
title: "Evernote Introduces 2 Factor Support (and more)"
microblog: false
date: 2013-05-30 16:00 +0300
guid: http://desparoz.micro.blog/2013/05/30/evernote-introduces-factor.html
---
<p>I&#8217;m a big fan of <a href="http://desparoz.com/2-factor-support/">2 factor security</a> for critical information stored online (in the &#8220;cloud&#8221;). After the <a href="http://desparoz.com/blog/2013/03/03/evernotes-password-hack-and-the-security-of-your-stuff-in-the-cloud">attempted hacking on Evernote</a> back in March, I made the following resolutions regarding the security of my online data:</p>

<blockquote>
<p>Clearly this issue has made me re-consider aspects of my own approach to information security, and has reinforced others. I recommend that everyone do the same, and take at least the following actions:</p>

<ol>
<li><p>Use only reputable services that provide 2-factor authentication for cloud storage of personal, sensitive or confidential data;</p></li>
<li><p>Have a personal password management policy that includes never re-using passwords, and never using dictionary passwords. Use of an app like 1Password, LastPass or similar may help.</p></li>
</ol>
</blockquote>

<p>At the time I wrote that post, Google and Dropbox were the main services to have implemented 2 factor security, and it&#8217;s been pleasing to see that other services have commenced implementation of 2 factor security, including <a href="http://blog.app.net/2013/03/13/added-security-for-your-app-net-account/">App.net</a>, <a href="http://desparoz.com/blog/2013/03/22/apples-two-step-verification-has-a-good-security-backup">Apple</a> <a href="#fn:1" id="fnref:1" title="see footnote" class="footnote">[1]</a>, <a href="https://www.facebook.com/note.php?note_id=10150172618258920">Facebook</a>, <a href="http://blog.fastmail.fm/2013/05/03/google-authenticator-now-supported-for-two-factor-authentication/">Fastmail</a> (my email host of choice) and <a href="https://blog.twitter.com/2013/getting-started-login-verification">Twitter</a> <a href="#fn:2" id="fnref:2" title="see footnote" class="footnote">[2]</a>, and most recently, <strong><a href="http://blog.evernote.com/blog/2013/05/30/evernotes-three-new-security-features/">Evernote</a></strong>.</p>

<p>I was initially disappointed with what I first read about <a href="http://blog.evernote.com/blog/2013/05/30/evernotes-three-new-security-features/">Evernote&#8217;s 2 factor security implementation</a> because the first blog post I read indicated the implementation was SMS based. However, on reading Evernote&#8217;s blog post I saw they indicated a choice of SMS or authentication with Google Authenticator.</p>

<p><img src="http://desparoz.me/uploads/2017/2dcb1f9392.jpg" alt="Evernote implements 2 factor security, and more" id="en2p" /></p>

<p>I&#8217;ve set Evernote 2 factor up using Google Authenticator <a href="#fn:3" id="fnref:3" title="see footnote" class="footnote">[3]</a>, and am delighted that my major online services have at least begun implementation of 2 factor support. Fastmail, Evernote and Dropbox are the most important for me, and they each have good 2 factor support. The main piece still missing (for me) is iCloud, although the data stored there is less security critical.</p>

<p>Evernote&#8217;s implementation works well, but is only for Evernote Premium users at this time. A couple of important things should be borne in mind when implementing it (or for that matter, any 2 factor security system).</p>

<ol>
<li>Ensure that you have updated the corresponding app (or apps) on every device before implementation; and,</li>
<li>Save the backup codes provided in a secure repository (print the out or save them in a secure location like 1Password).</li>
</ol>

<p>Evernote&#8217;s latest security updates also includes a couple of additional things (available for all users) - <em>Authorised Applications</em> (and the ability to revoke access remotely) and <em>Access History</em>.</p>

<p>Hop to it. With this implementation, Evernote (the best online repository of <em>stuff</em>) is now even better.</p>

<div class="footnotes">
<hr />
<ol>

<li id="fn:1">
<p>So far, Apple&#8217;s implementation seems to be a bit of a lame duck, because it doesn&#8217;t seem to do very much. I&#8217;ve not actually seen it request a code since the initial setup, and it doesn&#8217;t seem to be connected (at this time) to iCloud or the iTunes/App Stores. <a href="#fnref:1" title="return to article" class="reversefootnote">&#160;&#8617;</a></p>
</li>

<li id="fn:2">
<p><a href="http://www.informationweek.com/security/management/twitters-two-factor-authentication-5-rea/240155539">Twitter&#8217;s implementation has been quite critically received</a>, primarily because authentication is by SMS and doesn&#8217;t allow multiuser capability (like Facebook). <a href="#fnref:2" title="return to article" class="reversefootnote">&#160;&#8617;</a></p>
</li>

<li id="fn:3">
<p><a href="http://desparoz.com/blog/2013/4/11/the-de-google-fying-of-my-online-life">I have moved away from many of Google&#8217;s app and services</a>. At the time I originally wrote this post, I was using Google Authenticator, but now use <a href="https://itunes.apple.com/au/app/authy/id494168017?mt=8&amp;uo=4&amp;at=11l4Ky">Authy</a> instead. It&#8217;s a nice little app for the job (update 29/8/13). <a href="#fnref:3" title="return to article" class="reversefootnote">&#160;&#8617;</a></p>
</li>

</ol>
</div>
