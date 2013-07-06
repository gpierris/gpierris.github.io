#Various Visualization issues


## Requirements


###Grace
Of course we need grace! You could try in ubuntu
```
sudo apt-get install grace
```

###PyGrace
We use the PyGrace python bindings. Not to be confused with pygrace!

Visit [pygrace.github.io](pygrace.github.io) for more info

##Setting dpi resolution

Edit the desired dpi value in the file gracerc.user or add more options and then copy it in the folder ~/.grace/ 

FIXME: Write a script to automate the process by calling a, e.g., setResolution 300


##Writing graph to file

For example, 
```
from PyGrace.grace import Grace
grace = Grace(colors=ColorBrewerScheme('Paired'))
...
grace.write_file("myGraph.eps")
grace.write_file("myGraph.png")
grace.write_file("myGraph.jpeg")
```


