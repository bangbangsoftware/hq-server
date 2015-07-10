HQ Server
=========

What is it?
-----------
HQ as in head quarters, so its a server for the head quarters. Server is pushing it really, it is a deamon that runs and checks rss feeds for new content. When it finds new audio/video content it will download it. All the content it does find it will make into a HTML page and ftp it to a server. Also it (should) tweet the content. It also comes with kicker, this will bounce it, if it appears stuck, ie the html file has not changed, it should also send an error mail with public IP of server. 

Where it's at
-------------
This is a recent convert from python2.7 to 3.x. It is buggy: 
   * Daemon doesn't create PID files, so can't be "stop"ped 
   * Twitter is failing (along with shortend URLS) 
   * Need to put into a virtual environment 
   * Needs major refactoring. The main script needs breaking down into shorter scripts with unit testing and code coverage. Maybe a github associated service can help with the builds and tests.


