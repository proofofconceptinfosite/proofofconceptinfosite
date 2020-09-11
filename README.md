<html>
  <body>
    <h2>Neuroglancer</h2>
    <iframe src="https://neuroglancer-demo.appspot.com/" height="600" width="800" title="Neuroglancer"></iframe>
    
from bokeh.plotting import figure
from bokeh.resources import CDN
from bokeh.embed import file_html

plot = figure()
plot.circle([1,2], [3,4])
html = file_html(plot, CDN, "my plot")
<iframe src="html"></>
</body>
</html>
