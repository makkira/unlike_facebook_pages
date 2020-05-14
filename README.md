# unlike_facebook_pages
Mass Unlike FB Pages

Remember when we all went through the mass liking phase of FB. When we found that hundreds of lines that just "spoke to us." Well, this is a clunky way to unlike all of those pages, clearing your like history from all kinds of shame.  
  
Step 1 -- go to the Pages page  
Step 2 -- Right click on the "Like" Button and go to the inspect tool  
Step 3 -- Go to the console  
Step 4 -- Copy button class name, should look something like `<button class=271k _271l _271m _1qjd _3-9a _7tvm _7tv2 _7tv4"`  
This is where it gets wonky, working on a simpler way to do this:  
Step 5 -- Scroll down until you get to the end of your Liked Pages  
Step 6 -- Paste the following into the console, it'll lag for a bit but patience  
``` let b = document.querySelectorAll('button._271k._271l._271m._1qjd._3-9a._7tvm._7tv2._7tv4') // change into your class names   
for(i = 0; i < b.length; i++){   
      b[i].click() 
}```

