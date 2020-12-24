## Welcome!

This is a placeholder for my various hobby tech projects.  Right now I'm mostly playing with Peloton and Whoop data that's produced by my devices, but I also do some Jewish Scholarship coding on the side.

This is an informal index of some of the most recent projects I've been playing with. If you're interested, I'd love to hear your ideas. As always, PRs are most certainly welcome!

### Peloton Projects

1. [peloton-api-spec](https://github.com/pelo-tech/peloton-api-spec) - One thing that really bugged me was how inconsistently the Peloton APIs were used in various scripts and projects I saw on the web. Wouldn't it be great if we just had a properly documented (or almost properly documented) schema describing what the API could actually do? Perhaps we can generate client-side code, or just use a spec viewer to properly test drive the API.. Nothing was there, so to start, I took what I could discover, and published it on SwaggerHub and here.

2. [peloton-google-sheet](https://github.com/pelo-tech/peloton-google-sheet) - The next pet peeve was the need to constantly go an download an excel of my workouts from Peloton. Wouldn't it be great if I had this automatically up to date somewhere in a Google Sheet, so perhaps I can visualize it with something like Google Data Studio?  Using the APIs I documented, I wrote some code that could then easily be scheduled to run every 8-12 hours to synchronize my google sheet with my peloton data. There's a video explaining how to set it up, and many people have found it quite useful (and done some pretty awesome visualizations on top of the data).

3. [pelo-challenge-google-sheet](https://github.com/pelo-tech/pelo-challenge-google-sheet) - Built on the above foundational elements I created a google sheet with code that can easily follow people who sign up via a Google Form, and then provided a toolkit to easily track their participation in known rides/events.  A few different challenges/competitions have used it, and it makes a good prototype for small group challenges. To properly scale this one obviously needs to build a real app to host on the cloud somwhere, but for a really convenient start, this has been great.

4. [custom-powerzone](https://github.com/pelo-tech/custom-powerzone) - This was a small project I decided to cook up one morning to create my own powerzone ride (e.g. via a 'Just Ride') and try to draw some seasonal holiday pictures into my Graph. In my case, Xmas tree and a Hannuka Menora. I created a webpage that would guide me through the zone instructions, and projected that onto my screen while playing my favorite songs on spotify.  I found it pretty useful. All you need to do is tweak the hardcoded data model to give it a try (right now it's a single HTML page so it doesn't need to be deployed anywhere special).   I'd love to see your graphs!
 
5. [pelo-buffergate-sheet](https://github.com/pelo-tech/pelo-buffergate-sheet) - This was a project I created to help identify the bufferring of rides when many of us outside the US were experience regular delays in the streams. Using the tech described above, a google form can be filled out by anyone interested which will result in them receiving a mail with all their buffered rides year to date, while at the same time a database is maintained of these rides to plot out where and when they happen.   It definitely showed those of use who were affected that we were not alone!

### Whoop Projects

1. [whoop-api-spec](https://github.com/pelo-tech/whoop-api-spec) - Similar to Peloton - Whoop data is all locked up and difficult to get and analyze. I decided to look into what was possible, and as I went along, documented a proper API spec that we could then reference to experiment and unlock some of the data that we were producing. Together with my peloton data I've produced some pretty interesting Google Data Studio visualizations.

2. [whoop-google-sheet](https://github.com/pelo-tech/whoop-google-sheet) - I really wanted my whoop data accessible in a spreadsheet so I can plot/analyze it, etc.  Using the API I documented, I created some code that helps maintain up to date whoop metrics in a google sheet - with a trigger which keeps it up to date automatically.

 
### Jewish Scholarship Projects

1. [DafYomi Portal Extension](https://github.com/DovOps/DafYomi)- I created a simple chrome extension to help with my daily learning of Daf Yomi while using the [Daf Yomi Portal](https://daf-yomi.com).  In essence, I wanted to open PDFs of the 4 relevant amudim of today's learning (Yesterday's Amud Bet, today's full daf, and tomorrows Amud Aleph).  By injecting a button to the daf-yomi homepage, I'm able to open these tabs, maximize the PDF they contain, and focus the screen directly on them for easy use and screen sharing during online shiurim.

2. [Sefaria OpenAPI Spec](https://github.com/DovOps/Sefaria-OpenAPI-Spec) - One thing that's awesome about [Sefaria](https://sefaria.org) is that it has a rich API and thrives on integration. One thing that annoyed me is that the API wasn't documented with a standard schema, which meant I couldn't play around with API endpoints without writing code. I decided to take a stab at writing an Open API spec for Sefaria and published it to SwaggerHub (and here) so I could have my own test rig to play with API calls. It's not 100% complete but it did the trick (PRs welcome until they take it over and make this a standard part of their platform).

3. [Sefaria Sidebar Extension](https://github.com/DovOps/SefariaSidebarExtension) - While learning Daf Yomi, we often found ourselves leaning on Sefaria to get some of the references off the page. Instead of switching context, I thought it would be a good idea to bring the references onto the page in a non-intrusive way by using a Chrome extension to inject a Daf-specific reference toolbar onto the most popular Daf Yomi portals. I created a flexible daf recognizer that would invite anyone to contribute new sites to the list, and this has been very helpful in my daily learning.  This project - much to my surprise - won the ["Powered By Sefaria" Programming Contest](https://www.sefaria.org/powered-by-sefaria-contest-2020)  in the summer of 2020. 


