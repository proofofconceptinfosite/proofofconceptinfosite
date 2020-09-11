<html>
  <body>
    <h2>Neuroglancer</h2>
    <iframe src="https://neuroglancer-demo.appspot.com/" height="600" width="800" title="Neuroglancer"></iframe>
<script type="text/javascript">
    $(function() {
        var modelid = "fba97329-a355-499e-9252-0adc64b19d2e";
        var modeltype = "Plot";
        var elementid = "8ed68feb-d258-4953-9dfb-fb1c13326509";
        Bokeh.logger.info("Realizing plot:")
        Bokeh.logger.info(" - modeltype: Plot");
        Bokeh.logger.info(" - modelid: fba97329-a355-499e-9252-0adc64b19d2e");
        Bokeh.logger.info(" - elementid: 8ed68feb-d258-4953-9dfb-fb1c13326509");

        var all_models = [ JSON PLOT MODELS AND DATA ARE HERE ];

        Bokeh.load_models(all_models);
        var model = Bokeh.Collections(modeltype).get(modelid);
        var view = new model.default_view({
            model: model, el: '#8ed68feb-d258-4953-9dfb-fb1c13326509'
        });
        Bokeh.index[modelid] = view
    });
</script>
<div class="plotdiv" id="8ed68feb-d258-4953-9dfb-fb1c13326509"></div>
from bokeh.plotting import figure
from bokeh.embed import components

plot = figure()
plot.circle([1,2], [3,4])

script, div = components(plot)
<iframe src="plot"></>
</body>
</html>
