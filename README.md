# Fargo Scripts

This is a repo of some simple scripts I've made to augment fargo.

# To Use

As of v. 48, including extra javascript is a bit cumbersome. First, you'll need to copy the javascript you want to run to a server somewhere (a public link on Dropbox works fine). Then, you'll want to include a headline with the one-liner below in your outline (changing the URL to the one where you hosted the file). Finally, run the script in Fargo with Control/Cmd + /. 

    (function(u){console.log("loading "+u);$.getScript(u).done(function(o,s){console.log("Done: "+s)}).fail(function(j,s,e){console.log("Failed: "+s);throw e;});return u;})('http://server.something.com/example.js')

Voila. You should now have the extra functionality in there.
