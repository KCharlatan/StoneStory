# StoneStory

My customized stonescript for Stone Story RPG.  
I started getting annoyed with the restrictions on mobile necessitating one-file hero scripts, so I'm modularizing with GitHub.

## Update

With the lack of continued support for mobile script writing from the developer, I've decided this just isn't worth the hassle.  
Shame, because it is pretty fun, well-executed gameplay. But the hoops expected to go through for scripting are nuts.  
All the Dev has to do is _update the manual_ to let people know, "Hey! This doesn't have the greatest experience on mobile devices, and we've decided not to pursue updating it for X reason."

## Starter

Here's the Mindstone script for in game:
```
sys.cacheRemoteFiles=false
var file_gh=＂https://raw.githubusercontent.com/
^KCharlatan/StoneStory/
^refs/heads/main/＂
? !string.Equals(sys.fileUrl,file_gh)
  sys.SetFileUrl(file_gh)
  >`0,0,#red,SET NEW FILE URL!
  loc.pause()

// imports have to be commented on first run
// after starting up the game
// uncomment after file url is set
//import Stone
```
