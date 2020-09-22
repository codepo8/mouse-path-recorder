# Mouse Path Recorder

A [small tool to record the mouse position](https://codepo8.github.io/mouse-path-recorder/#help) and get it as a JSON object.

* Start by clicking on the big rectangle and you'll see a small recording icon appear bottom left. Any mouse movement now adds to the dataset. Click again stops the recording.
* Enable "Limit Points" to record fewer points and get in a smaller dataset.
* Once recorded, you can re-play the paths with the play button.
* Edit the dataset in the text box below and save it as a file by clicking the download link.
* The load button allows you to load old datasets. If you load an image, it will become the background to allow you to trace it.
* Click the bin to delete all your work and start over.

## Credits

All work by [Christian Heilmann](https://twitter.com/codepo8). 

## File Format support 

Currently, the generated files are pretty rudimentary, and there may be some tools for conversion in the nearer future. 

The format is a main Object with paths. Each path has its running number as the key and an array of values. The array is a list of the recorded x and y values. 

```
{
    "1": [x,y,x2,y2,x3,y3 … ],
    "2": [x,y,x2,y2,x3,y3 … ]
    …
}
```
## Why?

Well, this is one of those "scratching your own itch" things. We're working on a demo for the Commodore 64, and needed a way to record some hand-writing to replay using sprites.

So, yeah, geek stuff.
