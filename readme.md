<h4>linereg</h4>
`linereg` generates trendlines by linear regression on user-input data. 

![before trendline](https://github.com/markedwinharvey/linereg/blob/master/media/before.trendline.png)
![after trendline](https://github.com/markedwinharvey/linereg/blob/master/media/after.trendline.png)

The program is invoked from the command line with the command `python start.py`, 
which starts a localhost server (`server.py`), serving on port 8000. 

`linereg.html` is read from file `linereg` and opened in the default browser. 

The simple interface allows points to be drawn in a 400x400 pixel area. 

The 'regression' button sends the point data to `linereg.py` for processing via jquery/ajax. 

Linear regression is performed in python by minimizing the cost function through gradient descent. 

The output (theta values) is returned to `linereg.html` for plotting, where a trendline is drawn over the data. 

FYI the `tools` repo has a generalized numpy-based trendline-finder called trendline.py. 

