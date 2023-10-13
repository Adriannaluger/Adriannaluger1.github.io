As climate change is on the rise wildfire are becoming more frequent. The report from the Trump administration said that the warmer our country gets the more combustible it will be, and that with continued release of greenhouse gases fires will be more frequent. Fires may no longer just be a Western United States problem but a national problem. We know this because we have already seen increased burning in the West from dryer forests, warmer summers resulting in less snow, droughts, and by looking at human behavior where people are increasingly intruding into wildland areas. Unfortunately, this will only worsen climate change as fires increase carbon emissions setting off a deadly positive feedback loop.

Pierre-louis, K., &amp; Popovich, N. (2018, November 27). Climate change is fueling wildfires nationwide, New Report warns. The New York Times. https://www.nytimes.com/interactive/2018/11/27/climate/wildfire-global-warming.html 






<style>*[data-root-id],
*[data-root-id] > * {
  box-sizing: border-box;
  font-family: var(--jp-ui-font-family);
  font-size: var(--jp-ui-font-size1);
  color: var(--vscode-editor-foreground, var(--jp-ui-font-color1));
}

/* Override VSCode background color */
.cell-output-ipywidget-background:has(
    > .cell-output-ipywidget-background > .lm-Widget > *[data-root-id]
  ),
.cell-output-ipywidget-background:has(> .lm-Widget > *[data-root-id]) {
  background-color: transparent !important;
}
</style>


The national hydrography dataset (NHD) represents water drainage networks in the United States. This includes features such as rivers, streams, canals, lakes, ponds, streamgages, etc. This dataset includes line, area, and point features. It is typically mapped at 1:24,000 scale or larger and maintained through Stweardship partnerships. It is available as a geodatabase and shapfile. The geodatabase maintains detailed features while a shapefile simplifies its structure. 

National Hydrography Dataset. National Hydrography Dataset | U.S. Geological Survey. (n.d.). https://www.usgs.gov/national-hydrography/national-hydrography-dataset 

### National Hydrology (HU4) area




    <Axes: >




    
![png](vector_files/vector_6_1.png)
    


The data contains spatial database of wildfires in the United States from 1992 to 2020. It was acquired from the reporting systems from federal, state, and local fire organizations. It required discovery date, final fire size, and a point location at least as precise and 1-square mile grid. It also had basic error checking and cleaning for repeat records which results in 2.3 million wildfire records. 

Fires data:

    fire_gdf does not exsist. Loading...





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>FOD_ID</th>
      <th>FPA_ID</th>
      <th>SOURCE_SYSTEM_TYPE</th>
      <th>SOURCE_SYSTEM</th>
      <th>NWCG_REPORTING_AGENCY</th>
      <th>NWCG_REPORTING_UNIT_ID</th>
      <th>NWCG_REPORTING_UNIT_NAME</th>
      <th>SOURCE_REPORTING_UNIT</th>
      <th>SOURCE_REPORTING_UNIT_NAME</th>
      <th>LOCAL_FIRE_REPORT_ID</th>
      <th>...</th>
      <th>FIRE_SIZE</th>
      <th>FIRE_SIZE_CLASS</th>
      <th>LATITUDE</th>
      <th>LONGITUDE</th>
      <th>OWNER_DESCR</th>
      <th>STATE</th>
      <th>COUNTY</th>
      <th>FIPS_CODE</th>
      <th>FIPS_NAME</th>
      <th>geometry</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>FS-1418826</td>
      <td>FED</td>
      <td>FS-FIRESTAT</td>
      <td>FS</td>
      <td>USCAPNF</td>
      <td>Plumas National Forest</td>
      <td>0511</td>
      <td>Plumas National Forest</td>
      <td>1</td>
      <td>...</td>
      <td>0.10</td>
      <td>A</td>
      <td>40.036944</td>
      <td>-121.005833</td>
      <td>USFS</td>
      <td>CA</td>
      <td>63</td>
      <td>06063</td>
      <td>Plumas County</td>
      <td>POINT (-121.00582 40.03694)</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>FS-1418827</td>
      <td>FED</td>
      <td>FS-FIRESTAT</td>
      <td>FS</td>
      <td>USCAENF</td>
      <td>Eldorado National Forest</td>
      <td>0503</td>
      <td>Eldorado National Forest</td>
      <td>13</td>
      <td>...</td>
      <td>0.25</td>
      <td>A</td>
      <td>38.933056</td>
      <td>-120.404444</td>
      <td>USFS</td>
      <td>CA</td>
      <td>61</td>
      <td>06061</td>
      <td>Placer County</td>
      <td>POINT (-120.40443 38.93305)</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>FS-1418835</td>
      <td>FED</td>
      <td>FS-FIRESTAT</td>
      <td>FS</td>
      <td>USCAENF</td>
      <td>Eldorado National Forest</td>
      <td>0503</td>
      <td>Eldorado National Forest</td>
      <td>27</td>
      <td>...</td>
      <td>0.10</td>
      <td>A</td>
      <td>38.984167</td>
      <td>-120.735556</td>
      <td>STATE OR PRIVATE</td>
      <td>CA</td>
      <td>17</td>
      <td>06017</td>
      <td>El Dorado County</td>
      <td>POINT (-120.73554 38.98416)</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>FS-1418845</td>
      <td>FED</td>
      <td>FS-FIRESTAT</td>
      <td>FS</td>
      <td>USCAENF</td>
      <td>Eldorado National Forest</td>
      <td>0503</td>
      <td>Eldorado National Forest</td>
      <td>43</td>
      <td>...</td>
      <td>0.10</td>
      <td>A</td>
      <td>38.559167</td>
      <td>-119.913333</td>
      <td>USFS</td>
      <td>CA</td>
      <td>3</td>
      <td>06003</td>
      <td>Alpine County</td>
      <td>POINT (-119.91332 38.55916)</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>FS-1418847</td>
      <td>FED</td>
      <td>FS-FIRESTAT</td>
      <td>FS</td>
      <td>USCAENF</td>
      <td>Eldorado National Forest</td>
      <td>0503</td>
      <td>Eldorado National Forest</td>
      <td>44</td>
      <td>...</td>
      <td>0.10</td>
      <td>A</td>
      <td>38.559167</td>
      <td>-119.933056</td>
      <td>USFS</td>
      <td>CA</td>
      <td>3</td>
      <td>06003</td>
      <td>Alpine County</td>
      <td>POINT (-119.93304 38.55916)</td>
    </tr>
  </tbody>
</table>
<p>5 rows × 38 columns</p>
</div>



    /opt/conda/lib/python3.10/site-packages/geopandas/geodataframe.py:206: UserWarning: Pandas doesn't allow columns to be created via a new attribute name - see https://pandas.pydata.org/pandas-docs/stable/indexing.html#attribute-access
      super().__setattr__(attr, val)


         column_name                  ylabel                                 title
    0  max_fire_size  Fire Size (million ha)  Largest fire on record in the region
    1      num_fires         Number of Fires   Total number of fires in the region


    /opt/conda/lib/python3.10/site-packages/holoviews/core/util.py:1175: FutureWarning: unique with argument that is not not a Series, Index, ExtensionArray, or np.ndarray is deprecated and will raise in a future version.
      return pd.unique(values)
    /opt/conda/lib/python3.10/site-packages/holoviews/core/util.py:1175: FutureWarning: unique with argument that is not not a Series, Index, ExtensionArray, or np.ndarray is deprecated and will raise in a future version.
      return pd.unique(values)
    /opt/conda/lib/python3.10/site-packages/holoviews/core/data/pandas.py:39: FutureWarning: Series.__getitem__ treating keys as positions is deprecated. In a future version, integer keys will always be treated as labels (consistent with DataFrame behavior). To access a value by position, use `ser.iloc[pos]`
      return dataset.data.dtypes[idx].type
    /opt/conda/lib/python3.10/site-packages/holoviews/core/data/pandas.py:39: FutureWarning: Series.__getitem__ treating keys as positions is deprecated. In a future version, integer keys will always be treated as labels (consistent with DataFrame behavior). To access a value by position, use `ser.iloc[pos]`
      return dataset.data.dtypes[idx].type
    /opt/conda/lib/python3.10/site-packages/holoviews/core/data/pandas.py:39: FutureWarning: Series.__getitem__ treating keys as positions is deprecated. In a future version, integer keys will always be treated as labels (consistent with DataFrame behavior). To access a value by position, use `ser.iloc[pos]`
      return dataset.data.dtypes[idx].type
    /opt/conda/lib/python3.10/site-packages/holoviews/core/data/pandas.py:39: FutureWarning: Series.__getitem__ treating keys as positions is deprecated. In a future version, integer keys will always be treated as labels (consistent with DataFrame behavior). To access a value by position, use `ser.iloc[pos]`
      return dataset.data.dtypes[idx].type
    /opt/conda/lib/python3.10/site-packages/holoviews/plotting/bokeh/plot.py:987: UserWarning: found multiple competing values for 'toolbar.active_drag' property; using the latest value
      layout_plot = gridplot(
    /opt/conda/lib/python3.10/site-packages/holoviews/plotting/bokeh/plot.py:987: UserWarning: found multiple competing values for 'toolbar.active_scroll' property; using the latest value
      layout_plot = gridplot(





    BokehModel(combine_events=True, render_bundle={'docs_json': {'2968439c-1a9f-476c-bb81-2ce5707391e5': {'version…



### Fire Density Plot 
This plot shows us the fire densities in the National Hydrography dataset region. Because the region is fairly small the densities are all very similar but if we were to be looking at a bigger study area we may see more variety of colors. The density is somewhere between 508.5 to 508.  






<div id='p1224'>
  <div id="d76dafbf-df78-4175-b131-add91cfea68b" data-root-id="p1224" style="display: contents;"></div>
</div>
<script type="application/javascript">(function(root) {
  var docs_json = {"84cfd46e-3d36-4cf2-a3fb-b21d141e86ad":{"version":"3.2.2","title":"Bokeh Application","roots":[{"type":"object","name":"Row","id":"p1224","attributes":{"name":"Row01953","tags":["embedded"],"stylesheets":["\n:host(.pn-loading.pn-arc):before, .pn-loading.pn-arc:before {\n  background-image: url(\"data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHN0eWxlPSJtYXJnaW46IGF1dG87IGJhY2tncm91bmQ6IG5vbmU7IGRpc3BsYXk6IGJsb2NrOyBzaGFwZS1yZW5kZXJpbmc6IGF1dG87IiB2aWV3Qm94PSIwIDAgMTAwIDEwMCIgcHJlc2VydmVBc3BlY3RSYXRpbz0ieE1pZFlNaWQiPiAgPGNpcmNsZSBjeD0iNTAiIGN5PSI1MCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjYzNjM2MzIiBzdHJva2Utd2lkdGg9IjEwIiByPSIzNSIgc3Ryb2tlLWRhc2hhcnJheT0iMTY0LjkzMzYxNDMxMzQ2NDE1IDU2Ljk3Nzg3MTQzNzgyMTM4Ij4gICAgPGFuaW1hdGVUcmFuc2Zvcm0gYXR0cmlidXRlTmFtZT0idHJhbnNmb3JtIiB0eXBlPSJyb3RhdGUiIHJlcGVhdENvdW50PSJpbmRlZmluaXRlIiBkdXI9IjFzIiB2YWx1ZXM9IjAgNTAgNTA7MzYwIDUwIDUwIiBrZXlUaW1lcz0iMDsxIj48L2FuaW1hdGVUcmFuc2Zvcm0+ICA8L2NpcmNsZT48L3N2Zz4=\");\n  background-size: auto calc(min(50%, 400px));\n}",{"type":"object","name":"ImportedStyleSheet","id":"p1227","attributes":{"url":"https://cdn.holoviz.org/panel/1.2.3/dist/css/loading.css"}},{"type":"object","name":"ImportedStyleSheet","id":"p1308","attributes":{"url":"https://cdn.holoviz.org/panel/1.2.3/dist/css/listpanel.css"}},{"type":"object","name":"ImportedStyleSheet","id":"p1225","attributes":{"url":"https://cdn.holoviz.org/panel/1.2.3/dist/bundled/theme/default.css"}},{"type":"object","name":"ImportedStyleSheet","id":"p1226","attributes":{"url":"https://cdn.holoviz.org/panel/1.2.3/dist/bundled/theme/native.css"}}],"min_width":600,"margin":0,"sizing_mode":"stretch_width","align":"start","children":[{"type":"object","name":"Spacer","id":"p1228","attributes":{"name":"HSpacer01963","stylesheets":["\n:host(.pn-loading.pn-arc):before, .pn-loading.pn-arc:before {\n  background-image: url(\"data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHN0eWxlPSJtYXJnaW46IGF1dG87IGJhY2tncm91bmQ6IG5vbmU7IGRpc3BsYXk6IGJsb2NrOyBzaGFwZS1yZW5kZXJpbmc6IGF1dG87IiB2aWV3Qm94PSIwIDAgMTAwIDEwMCIgcHJlc2VydmVBc3BlY3RSYXRpbz0ieE1pZFlNaWQiPiAgPGNpcmNsZSBjeD0iNTAiIGN5PSI1MCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjYzNjM2MzIiBzdHJva2Utd2lkdGg9IjEwIiByPSIzNSIgc3Ryb2tlLWRhc2hhcnJheT0iMTY0LjkzMzYxNDMxMzQ2NDE1IDU2Ljk3Nzg3MTQzNzgyMTM4Ij4gICAgPGFuaW1hdGVUcmFuc2Zvcm0gYXR0cmlidXRlTmFtZT0idHJhbnNmb3JtIiB0eXBlPSJyb3RhdGUiIHJlcGVhdENvdW50PSJpbmRlZmluaXRlIiBkdXI9IjFzIiB2YWx1ZXM9IjAgNTAgNTA7MzYwIDUwIDUwIiBrZXlUaW1lcz0iMDsxIj48L2FuaW1hdGVUcmFuc2Zvcm0+ICA8L2NpcmNsZT48L3N2Zz4=\");\n  background-size: auto calc(min(50%, 400px));\n}",{"id":"p1227"},{"id":"p1225"},{"id":"p1226"}],"margin":0,"sizing_mode":"stretch_width","align":"start"}},{"type":"object","name":"Figure","id":"p1249","attributes":{"margin":[5,10],"sizing_mode":"fixed","align":"start","x_range":{"type":"object","name":"Range1d","id":"p1238","attributes":{"tags":[[["Longitude","Longitude",null]],[]],"start":-7872441.094181293,"end":-7374119.669377842,"reset_start":-7872441.094181293,"reset_end":-7374119.669377842,"min_interval":5}},"y_range":{"type":"object","name":"Range1d","id":"p1239","attributes":{"tags":[[["Latitude","Latitude",null]],{"type":"map","entries":[["invert_yaxis",false],["autorange",false]]}],"start":5696441.390657181,"end":6144398.791229952,"reset_start":5696441.390657181,"reset_end":6144398.791229952,"min_interval":5}},"x_scale":{"type":"object","name":"LinearScale","id":"p1259"},"y_scale":{"type":"object","name":"LinearScale","id":"p1260"},"title":{"type":"object","name":"Title","id":"p1252","attributes":{"text_color":"black","text_font_size":"12pt"}},"renderers":[{"type":"object","name":"TileRenderer","id":"p1282","attributes":{"level":"underlay","tile_source":{"type":"object","name":"WMTSTileSource","id":"p1278","attributes":{"url":"https://c.tile.openstreetmap.org/{Z}/{X}/{Y}.png","attribution":"&copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors"}}}},{"type":"object","name":"GlyphRenderer","id":"p1296","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1287","attributes":{"selected":{"type":"object","name":"Selection","id":"p1288","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1289"},"data":{"type":"map","entries":[["xs",[[[{"type":"ndarray","array":{"type":"bytes","data":"Bp/H6AhDXcGeQV7RZv5cwRY7WYW0BF3BJ0M9c2zdXMFyB/ZMJOlcwRmaBuLV0lzBUEHYo7GlXMHUpWamhpxcwd871MctwFzBP7NWmkmXXMEni5VR9YdcwfE5+5XXSVzBexwQsUVpXMF6HF8xTpFcwWz4S4wMlVzBadhEyNmtXMEMOK4T17hcwU6JEcg28FzBdyCzXAYfXcFDncW9jm5dwb3aaN+dkF3BkuLSrNCwXcFldBkHjrJdwTHt4ppg313Byi14L+/cXcHvkeovhIldwWh+Gw4jcF3B4dO9i5NbXcE="},"shape":[28],"dtype":"float64","order":"little"}]]]],["ys",[[[{"type":"ndarray","array":{"type":"bytes","data":"csXGuxpKV0HHYCZL70tXQUP+GwPUOFdBLa1p9TQnV0Evl049SRdXQSf3QGsB31ZBe89+riToVkFqrJWgkLlWQSb3JvPmhVZBkfV92VVqVkFwUXGxGTpWQZne9e6XFVZBJJ7vwGLfVUEfjhq79/pVQau0id304VVBdB0AW2b1VUH8FDz2pONVQSlhJkkNMlZBXUsDL65DVkHBMkXyBjJWQcIKAtabVlZB6q3XgeEKVkHx9d6vtyhWQTUcMU0ZJFZBTuc9ADSGVkGvvCIol9hWQYhGNevQK1dBSf+ix84VV0E="},"shape":[28],"dtype":"float64","order":"little"}]]]],["fire_density_per_ha",{"type":"ndarray","array":{"type":"bytes","data":"3UtKCs7Af0A="},"shape":[1],"dtype":"float64","order":"little"}],["name",{"type":"ndarray","array":["St. John"],"shape":[1],"dtype":"object","order":"little"}]]}}},"view":{"type":"object","name":"CDSView","id":"p1297","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1298"}}},"glyph":{"type":"object","name":"MultiPolygons","id":"p1293","attributes":{"xs":{"type":"field","field":"xs"},"ys":{"type":"field","field":"ys"},"line_color":{"type":"value","value":"white"},"fill_color":{"type":"field","field":"fire_density_per_ha","transform":{"type":"object","name":"LinearColorMapper","id":"p1286","attributes":{"palette":["#0c0786","#100787","#130689","#15068a","#18068b","#1b068c","#1d068d","#1f058e","#21058f","#230590","#250591","#270592","#290593","#2b0594","#2d0494","#2f0495","#310496","#330497","#340498","#360498","#380499","#3a049a","#3b039a","#3d039b","#3f039c","#40039c","#42039d","#44039e","#45039e","#47029f","#49029f","#4a02a0","#4c02a1","#4e02a1","#4f02a2","#5101a2","#5201a3","#5401a3","#5601a3","#5701a4","#5901a4","#5a00a5","#5c00a5","#5e00a5","#5f00a6","#6100a6","#6200a6","#6400a7","#6500a7","#6700a7","#6800a7","#6a00a7","#6c00a8","#6d00a8","#6f00a8","#7000a8","#7200a8","#7300a8","#7500a8","#7601a8","#7801a8","#7901a8","#7b02a8","#7c02a7","#7e03a7","#7f03a7","#8104a7","#8204a7","#8405a6","#8506a6","#8607a6","#8807a5","#8908a5","#8b09a4","#8c0aa4","#8e0ca4","#8f0da3","#900ea3","#920fa2","#9310a1","#9511a1","#9612a0","#9713a0","#99149f","#9a159e","#9b179e","#9d189d","#9e199c","#9f1a9b","#a01b9b","#a21c9a","#a31d99","#a41e98","#a51f97","#a72197","#a82296","#a92395","#aa2494","#ac2593","#ad2692","#ae2791","#af2890","#b02a8f","#b12b8f","#b22c8e","#b42d8d","#b52e8c","#b62f8b","#b7308a","#b83289","#b93388","#ba3487","#bb3586","#bc3685","#bd3784","#be3883","#bf3982","#c03b81","#c13c80","#c23d80","#c33e7f","#c43f7e","#c5407d","#c6417c","#c7427b","#c8447a","#c94579","#ca4678","#cb4777","#cc4876","#cd4975","#ce4a75","#cf4b74","#d04d73","#d14e72","#d14f71","#d25070","#d3516f","#d4526e","#d5536d","#d6556d","#d7566c","#d7576b","#d8586a","#d95969","#da5a68","#db5b67","#dc5d66","#dc5e66","#dd5f65","#de6064","#df6163","#df6262","#e06461","#e16560","#e26660","#e3675f","#e3685e","#e46a5d","#e56b5c","#e56c5b","#e66d5a","#e76e5a","#e87059","#e87158","#e97257","#ea7356","#ea7455","#eb7654","#ec7754","#ec7853","#ed7952","#ed7b51","#ee7c50","#ef7d4f","#ef7e4e","#f0804d","#f0814d","#f1824c","#f2844b","#f2854a","#f38649","#f38748","#f48947","#f48a47","#f58b46","#f58d45","#f68e44","#f68f43","#f69142","#f79241","#f79341","#f89540","#f8963f","#f8983e","#f9993d","#f99a3c","#fa9c3b","#fa9d3a","#fa9f3a","#faa039","#fba238","#fba337","#fba436","#fca635","#fca735","#fca934","#fcaa33","#fcac32","#fcad31","#fdaf31","#fdb030","#fdb22f","#fdb32e","#fdb52d","#fdb62d","#fdb82c","#fdb92b","#fdbb2b","#fdbc2a","#fdbe29","#fdc029","#fdc128","#fdc328","#fdc427","#fdc626","#fcc726","#fcc926","#fccb25","#fccc25","#fcce25","#fbd024","#fbd124","#fbd324","#fad524","#fad624","#fad824","#f9d924","#f9db24","#f8dd24","#f8df24","#f7e024","#f7e225","#f6e425","#f6e525","#f5e726","#f5e926","#f4ea26","#f3ec26","#f3ee26","#f2f026","#f2f126","#f1f326","#f0f525","#f0f623","#eff821"],"low":507.0503027822686,"high":509.0503027822686}}},"hatch_color":{"type":"field","field":"fire_density"}}},"selection_glyph":{"type":"object","name":"MultiPolygons","id":"p1304","attributes":{"xs":{"type":"field","field":"xs"},"ys":{"type":"field","field":"ys"},"line_color":{"type":"value","value":"white"},"line_alpha":{"type":"value","value":1.0},"line_width":{"type":"value","value":1},"line_join":{"type":"value","value":"bevel"},"line_cap":{"type":"value","value":"butt"},"line_dash":{"type":"value","value":[]},"line_dash_offset":{"type":"value","value":0},"fill_color":{"type":"field","field":"fire_density_per_ha","transform":{"id":"p1286"}},"fill_alpha":{"type":"value","value":1.0},"hatch_color":{"type":"field","field":"fire_density"},"hatch_alpha":{"type":"value","value":1.0},"hatch_scale":{"type":"value","value":12.0},"hatch_pattern":{"type":"value","value":null},"hatch_weight":{"type":"value","value":1.0}}},"nonselection_glyph":{"type":"object","name":"MultiPolygons","id":"p1294","attributes":{"xs":{"type":"field","field":"xs"},"ys":{"type":"field","field":"ys"},"line_color":{"type":"value","value":"white"},"line_alpha":{"type":"value","value":0.1},"fill_color":{"type":"field","field":"fire_density_per_ha","transform":{"id":"p1286"}},"fill_alpha":{"type":"value","value":0.1},"hatch_color":{"type":"field","field":"fire_density"},"hatch_alpha":{"type":"value","value":0.1}}},"muted_glyph":{"type":"object","name":"MultiPolygons","id":"p1295","attributes":{"xs":{"type":"field","field":"xs"},"ys":{"type":"field","field":"ys"},"line_color":{"type":"value","value":"white"},"line_alpha":{"type":"value","value":0.2},"fill_color":{"type":"field","field":"fire_density_per_ha","transform":{"id":"p1286"}},"fill_alpha":{"type":"value","value":0.2},"hatch_color":{"type":"field","field":"fire_density"},"hatch_alpha":{"type":"value","value":0.2}}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1258","attributes":{"tools":[{"type":"object","name":"WheelZoomTool","id":"p1242","attributes":{"zoom_on_axis":false}},{"type":"object","name":"BoxZoomTool","id":"p1243","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1004","attributes":{"syncable":false,"level":"overlay","visible":false,"left_units":"canvas","right_units":"canvas","bottom_units":"canvas","top_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}},"match_aspect":true}},{"type":"object","name":"HoverTool","id":"p1248","attributes":{"tags":["hv_created"],"renderers":[{"id":"p1296"}],"tooltips":[["fire_density_per_ha","@{fire_density_per_ha}"],["name","@{name}"]]}},{"type":"object","name":"PanTool","id":"p1272"},{"type":"object","name":"ResetTool","id":"p1273"}],"active_drag":{"id":"p1272"}}},"left":[{"type":"object","name":"LinearAxis","id":"p1266","attributes":{"ticker":{"type":"object","name":"MercatorTicker","id":"p1276","attributes":{"mantissas":[1,2,5],"dimension":"lat"}},"formatter":{"type":"object","name":"MercatorTickFormatter","id":"p1277","attributes":{"dimension":"lat"}},"axis_label":"Latitude","axis_label_text_font_size":"0pt","major_label_policy":{"type":"object","name":"AllLabels","id":"p1269"},"major_label_text_font_size":"0pt","major_tick_line_color":null,"minor_tick_line_color":null}}],"right":[{"type":"object","name":"ColorBar","id":"p1300","attributes":{"location":[0,0],"ticker":{"type":"object","name":"BasicTicker","id":"p1299","attributes":{"mantissas":[1,2,5]}},"major_label_policy":{"type":"object","name":"NoOverlap","id":"p1301"},"label_standoff":8,"major_tick_line_color":"black","bar_line_color":"black","color_mapper":{"id":"p1286"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1261","attributes":{"ticker":{"type":"object","name":"MercatorTicker","id":"p1274","attributes":{"mantissas":[1,2,5],"dimension":"lon"}},"formatter":{"type":"object","name":"MercatorTickFormatter","id":"p1275","attributes":{"dimension":"lon"}},"axis_label":"Longitude","axis_label_text_font_size":"0pt","major_label_policy":{"type":"object","name":"AllLabels","id":"p1264"},"major_label_text_font_size":"0pt","major_tick_line_color":null,"minor_tick_line_color":null}}],"center":[{"type":"object","name":"Grid","id":"p1265","attributes":{"axis":{"id":"p1261"},"grid_line_color":null}},{"type":"object","name":"Grid","id":"p1270","attributes":{"dimension":1,"axis":{"id":"p1266"},"grid_line_color":null}}],"min_border_top":10,"min_border_bottom":10,"min_border_left":10,"min_border_right":10,"output_backend":"webgl"}},{"type":"object","name":"Spacer","id":"p1306","attributes":{"name":"HSpacer01966","stylesheets":["\n:host(.pn-loading.pn-arc):before, .pn-loading.pn-arc:before {\n  background-image: url(\"data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHN0eWxlPSJtYXJnaW46IGF1dG87IGJhY2tncm91bmQ6IG5vbmU7IGRpc3BsYXk6IGJsb2NrOyBzaGFwZS1yZW5kZXJpbmc6IGF1dG87IiB2aWV3Qm94PSIwIDAgMTAwIDEwMCIgcHJlc2VydmVBc3BlY3RSYXRpbz0ieE1pZFlNaWQiPiAgPGNpcmNsZSBjeD0iNTAiIGN5PSI1MCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjYzNjM2MzIiBzdHJva2Utd2lkdGg9IjEwIiByPSIzNSIgc3Ryb2tlLWRhc2hhcnJheT0iMTY0LjkzMzYxNDMxMzQ2NDE1IDU2Ljk3Nzg3MTQzNzgyMTM4Ij4gICAgPGFuaW1hdGVUcmFuc2Zvcm0gYXR0cmlidXRlTmFtZT0idHJhbnNmb3JtIiB0eXBlPSJyb3RhdGUiIHJlcGVhdENvdW50PSJpbmRlZmluaXRlIiBkdXI9IjFzIiB2YWx1ZXM9IjAgNTAgNTA7MzYwIDUwIDUwIiBrZXlUaW1lcz0iMDsxIj48L2FuaW1hdGVUcmFuc2Zvcm0+ICA8L2NpcmNsZT48L3N2Zz4=\");\n  background-size: auto calc(min(50%, 400px));\n}",{"id":"p1227"},{"id":"p1225"},{"id":"p1226"}],"margin":0,"sizing_mode":"stretch_width","align":"start"}}]}}],"defs":[{"type":"model","name":"ReactiveHTML1"},{"type":"model","name":"FlexBox1","properties":[{"name":"align_content","kind":"Any","default":"flex-start"},{"name":"align_items","kind":"Any","default":"flex-start"},{"name":"flex_direction","kind":"Any","default":"row"},{"name":"flex_wrap","kind":"Any","default":"wrap"},{"name":"justify_content","kind":"Any","default":"flex-start"}]},{"type":"model","name":"FloatPanel1","properties":[{"name":"config","kind":"Any","default":{"type":"map"}},{"name":"contained","kind":"Any","default":true},{"name":"position","kind":"Any","default":"right-top"},{"name":"offsetx","kind":"Any","default":null},{"name":"offsety","kind":"Any","default":null},{"name":"theme","kind":"Any","default":"primary"},{"name":"status","kind":"Any","default":"normalized"}]},{"type":"model","name":"GridStack1","properties":[{"name":"mode","kind":"Any","default":"warn"},{"name":"ncols","kind":"Any","default":null},{"name":"nrows","kind":"Any","default":null},{"name":"allow_resize","kind":"Any","default":true},{"name":"allow_drag","kind":"Any","default":true},{"name":"state","kind":"Any","default":[]}]},{"type":"model","name":"drag1","properties":[{"name":"slider_width","kind":"Any","default":5},{"name":"slider_color","kind":"Any","default":"black"},{"name":"value","kind":"Any","default":50}]},{"type":"model","name":"click1","properties":[{"name":"terminal_output","kind":"Any","default":""},{"name":"debug_name","kind":"Any","default":""},{"name":"clears","kind":"Any","default":0}]},{"type":"model","name":"FastWrapper1","properties":[{"name":"object","kind":"Any","default":null},{"name":"style","kind":"Any","default":null}]},{"type":"model","name":"NotificationAreaBase1","properties":[{"name":"js_events","kind":"Any","default":{"type":"map"}},{"name":"position","kind":"Any","default":"bottom-right"},{"name":"_clear","kind":"Any","default":0}]},{"type":"model","name":"NotificationArea1","properties":[{"name":"js_events","kind":"Any","default":{"type":"map"}},{"name":"notifications","kind":"Any","default":[]},{"name":"position","kind":"Any","default":"bottom-right"},{"name":"_clear","kind":"Any","default":0},{"name":"types","kind":"Any","default":[{"type":"map","entries":[["type","warning"],["background","#ffc107"],["icon",{"type":"map","entries":[["className","fas fa-exclamation-triangle"],["tagName","i"],["color","white"]]}]]},{"type":"map","entries":[["type","info"],["background","#007bff"],["icon",{"type":"map","entries":[["className","fas fa-info-circle"],["tagName","i"],["color","white"]]}]]}]}]},{"type":"model","name":"Notification","properties":[{"name":"background","kind":"Any","default":null},{"name":"duration","kind":"Any","default":3000},{"name":"icon","kind":"Any","default":null},{"name":"message","kind":"Any","default":""},{"name":"notification_type","kind":"Any","default":null},{"name":"_destroyed","kind":"Any","default":false}]},{"type":"model","name":"TemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"BootstrapTemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]},{"type":"model","name":"MaterialTemplateActions1","properties":[{"name":"open_modal","kind":"Any","default":0},{"name":"close_modal","kind":"Any","default":0}]}]}};
  var render_items = [{"docid":"84cfd46e-3d36-4cf2-a3fb-b21d141e86ad","roots":{"p1224":"d76dafbf-df78-4175-b131-add91cfea68b"},"root_ids":["p1224"]}];
  var docs = Object.values(docs_json)
  if (!docs) {
    return
  }
  const py_version = docs[0].version.replace('rc', '-rc.').replace('.dev', '-dev.')
  const is_dev = py_version.indexOf("+") !== -1 || py_version.indexOf("-") !== -1
  function embed_document(root) {
    var Bokeh = get_bokeh(root)
    Bokeh.embed.embed_items_notebook(docs_json, render_items);
    for (const render_item of render_items) {
      for (const root_id of render_item.root_ids) {
	const id_el = document.getElementById(root_id)
	if (id_el.children.length && (id_el.children[0].className === 'bk-root')) {
	  const root_el = id_el.children[0]
	  root_el.id = root_el.id + '-rendered'
	}
      }
    }
  }
  function get_bokeh(root) {
    if (root.Bokeh === undefined) {
      return null
    } else if (root.Bokeh.version !== py_version && !is_dev) {
      if (root.Bokeh.versions === undefined || !root.Bokeh.versions.has(py_version)) {
	return null
      }
      return root.Bokeh.versions.get(py_version);
    } else if (root.Bokeh.version === py_version) {
      return root.Bokeh
    }
    return null
  }
  function is_loaded(root) {
    var Bokeh = get_bokeh(root)
    return (Bokeh != null && Bokeh.Panel !== undefined)
  }
  if (is_loaded(root)) {
    embed_document(root);
  } else {
    var attempts = 0;
    var timer = setInterval(function(root) {
      if (is_loaded(root)) {
        clearInterval(timer);
        embed_document(root);
      } else if (document.readyState == "complete") {
        attempts++;
        if (attempts > 200) {
          clearInterval(timer);
	  var Bokeh = get_bokeh(root)
	  if (Bokeh == null || Bokeh.Panel == null) {
            console.warn("Panel: ERROR: Unable to run Panel code because Bokeh or Panel library is missing");
	  } else {
	    console.warn("Panel: WARNING: Attempting to render but not all required libraries could be resolved.")
	    embed_document(root)
	  }
        }
      }
    }, 25, root)
  }
})(window);</script>



    [NbConvertApp] Converting notebook vector.ipynb to markdown
    /opt/conda/share/jupyter/nbconvert/templates/base/display_priority.j2:32: UserWarning: Your element with mimetype(s) dict_keys(['application/javascript', 'application/vnd.holoviews_load.v0+json']) is not able to be represented.
      {%- elif type == 'text/vnd.mermaid' -%}
    /opt/conda/share/jupyter/nbconvert/templates/base/display_priority.j2:32: UserWarning: Your element with mimetype(s) dict_keys([]) is not able to be represented.
      {%- elif type == 'text/vnd.mermaid' -%}
    [NbConvertApp] Support files will be in vector_files/
    [NbConvertApp] Writing 29578 bytes to vector.md

