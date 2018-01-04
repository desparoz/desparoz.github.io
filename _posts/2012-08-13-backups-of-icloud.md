---
layout: post
title: "Backups of iCloud Documents in the Cloud"
microblog: false
date: 2012-08-13 21:35 +0300
guid: http://desparoz.micro.blog/2012/08/13/backups-of-icloud.html
---
<p><a href="http://www.apple.com/icloud/"><img style="float: right;" title="" alt="" src="http://desparoz.me/uploads/2017/efc9c122ed.jpg" width="" height="" border="0" /></a>
I had a scary experience over the last couple of days, which I resolved this morning.</p>
<p>I'm working on an important project for a client at the moment, and had a bunch of annotated files saved to iCloud's Documents in the Cloud feature from the excellent <a href="http://smilesoftware.com/PDFpen/">PDF Pen</a> app, which I use on both the <a href="http://smilesoftware.com/PDFpen/iOS/index.html">iPad</a> and my Macs.</p>
<p>I had manually deleted a few unrelated files, and when I returned to the app on iPad, <span style="font-style: italic; text-decoration: underline;">all</span> my files were missing. So I checked on my MacBook Air and my iMac, and same story. Gone!</p>
<p>At this point, I had lost a bit of faith in the iCloud promise (which I am otherwise liking), and was certain that the problem was either a software issue (Smile Software's implementation of iCloud), or with iCloud itself. After calming down, I realised that it was probably user error, but that wasn't getting my documents back.</p>
<p>I was at a bit of loose end, not knowing whether to call Apple Care, or post to a forum or similar, when I saw the blog post by Chris Breen at MacWorld, <a href="http://www.macworld.com/article/1168122/when_documents_in_the_cloud_arent.html"><em>When Documents in the Cloud aren't…</em></a> Chris had been responding to a reader who had "lost" a document he printed as PDF to iCloud:</p>
<blockquote><p>In the Finder, hold down the Option key, click on the Go menu, and choose the now-visible Library command. Locate and open the Mobile Documents folder. Within you’ll find multiple folders. In your case you want the com~apple~mail folder. Inside you’ll find a Documents folder. Within it is your PDF file.</p></blockquote>
<p>Now this didn't address backups, but it did make think that if there is a local copy in the file system, then my Time Machine backups may well have a copy of my missing documents.</p>
<p>The next problem was that the "Library" folder in Finder is hidden, and while the Option-Click approach above works well for finding current documents, I wasn't sure how to approach this in Time Machine. A quick visit to Dr Google found the CNet article <a href="http://howto.cnet.com/8301-11310_39-20062357-285/how-to-access-hidden-files-to-restore-in-time-machine/"><em>How to access hidden files to restore in Time Machine</em></a>.</p>
<blockquote><p>Unfortunately, if you have removed a hidden directory that is within a normally visible directory (as is the case with the entire /etc directory), then the Finder will not allow you to see it by default, so using the "Go to folder" command will not work. Nevertheless you can still restore it using Time Machine by first showing hidden files in the Finder.</p></blockquote>
<p>To show the hidden files, simply open Terminal, and enter this command <a href="#footnote-1">[1]</a>:</p>
<blockquote><p>defaults write com.apple.finder AppleShowAllFiles TRUE;killall Finder</p></blockquote>
<p>Once you've done this, enter Time Machine as usual, browse to the dates you're looking for, and go to the Library&gt;Mobile Documents folder, and you'll see a list of folders for iCloud Documents, sorted by app. Find the right folder, and you should see the files in the iCloud for that App on that Date. Select and Restore, and you should be good to go.</p>
<p>Its kind of nice when things work out! Everything I needed was there, I just had to do some digging. Given that its more than possible that other users will make silly errors like mine, I wonder when Apple will make this type of restoration more seamless. Whilst its easy to use the Revert To function to go back to previous versions of a file within a given app, it doesn't help if you've deleted the whole file. In the meantime, I hope this workaround works for others.</p>
<h2>Updates</h2>
<p id="footnote-1">[1]   The excellent <a href="http://totalfinder.binaryage.com">TotalFinder</a> application provides many extensions to your OSX Finder, including the ability to easily "Show System Files", restoring access to the Library and and other hidden files.</p>
