**********
Multi Plot
**********

The Multi Plot object allows the generation of composite grid figures composed by multiple Diffusion Trends and/or Diffusion Prevalence plots.


.. autoclass:: ndlib.viz.bokeh.MultiPlot.MultiPlot
.. automethod:: ndlib.viz.bokeh.MultiPlot.MultiPlot.add_plot(plot)
.. automethod:: ndlib.viz.bokeh.MultiPlot.MultiPlot.plot(width, height)

.. automodule:: ndlib.viz.bokeh.MultiPlot
   :members:

.. code-block:: python
    :linenos:

    import networkx as nx
    from bokeh.io import show
    from ndlib.viz.bokeh.DiffusionTrend import DiffusionTrend
    from ndlib.viz.bokeh.DiffusionPrevalence import DiffusionPrevalence
    from ndlib.viz.bokeh.MultiPlot import Multiplot


    # Diffusion Trend
    vm.add_plot(p)

    # Diffusion Prevalence
    vm.add_plot(p1)
    
    m = vm.plot(ncol=2)
    show(m)