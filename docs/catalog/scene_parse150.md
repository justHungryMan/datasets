<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>
  <meta itemprop="name" content="scene_parse150" />
  <meta itemprop="description" content="Scene parsing is to segment and parse an image into different image regions&#10;associated with semantic categories, such as sky, road, person, and bed.&#10;MIT Scene Parsing Benchmark (SceneParse150) provides a standard training and&#10;evaluation platform for the algorithms of scene parsing.&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load(&#x27;scene_parse150&#x27;, split=&#x27;train&#x27;)&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/scene_parse150" />
  <meta itemprop="sameAs" content="http://sceneparsing.csail.mit.edu/" />
  <meta itemprop="citation" content="@inproceedings{zhou2017scene,&#10;title={Scene Parsing through ADE20K Dataset},&#10;author={Zhou, Bolei and Zhao, Hang and Puig, Xavier and Fidler, Sanja and Barriuso, Adela and Torralba, Antonio},&#10;booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},&#10;year={2017}&#10;}" />
</div>

# `scene_parse150`


*   **Visualization**:
    <a class="button button-with-icon" href="https://knowyourdata-tfds.withgoogle.com/#tab=STATS&dataset=scene_parse150">
    Explore in Know Your Data
    <span class="material-icons icon-after" aria-hidden="true"> north_east
    </span> </a>

*   **Description**:

Scene parsing is to segment and parse an image into different image regions
associated with semantic categories, such as sky, road, person, and bed. MIT
Scene Parsing Benchmark (SceneParse150) provides a standard training and
evaluation platform for the algorithms of scene parsing.

*   **Homepage**:
    [http://sceneparsing.csail.mit.edu/](http://sceneparsing.csail.mit.edu/)

*   **Source code**:
    [`tfds.image.SceneParse150`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/image/scene_parse_150.py)

*   **Versions**:

    *   **`1.0.0`** (default): No release notes.

*   **Download size**: `936.97 MiB`

*   **Dataset size**: `Unknown size`

*   **Auto-cached**
    ([documentation](https://www.tensorflow.org/datasets/performances#auto-caching)):
    Unknown

*   **Splits**:

Split     | Examples
:-------- | -------:
`'test'`  | 2,000
`'train'` | 20,210

*   **Features**:

```python
FeaturesDict({
    'annotation': Image(shape=(None, None, 3), dtype=tf.uint8),
    'image': Image(shape=(None, None, 3), dtype=tf.uint8),
})
```

*   **Supervised keys** (See
    [`as_supervised` doc](https://www.tensorflow.org/datasets/api_docs/python/tfds/load#args)):
    `('image', 'annotation')`

*   **Figure**
    ([tfds.show_examples](https://www.tensorflow.org/datasets/api_docs/python/tfds/visualization/show_examples)):
    Not supported.

*   **Examples**
    ([tfds.as_dataframe](https://www.tensorflow.org/datasets/api_docs/python/tfds/as_dataframe)):

<!-- mdformat off(HTML should not be auto-formatted) -->

{% framebox %}

<button id="displaydataframe">Display examples...</button>
<div id="dataframecontent" style="overflow-x:auto"></div>
<script src="https://www.gstatic.com/external_hosted/jquery2.min.js"></script>
<script>
var url = "https://storage.googleapis.com/tfds-data/visualization/dataframe/scene_parse150-1.0.0.html";
$(document).ready(() => {
  $("#displaydataframe").click((event) => {
    // Disable the button after clicking (dataframe loaded only once).
    $("#displaydataframe").prop("disabled", true);

    // Pre-fetch and display the content
    $.get(url, (data) => {
      $("#dataframecontent").html(data);
    }).fail(() => {
      $("#dataframecontent").html(
        'Error loading examples. If the error persist, please open '
        + 'a new issue.'
      );
    });
  });
});
</script>

{% endframebox %}

<!-- mdformat on -->

*   **Citation**:

```
@inproceedings{zhou2017scene,
title={Scene Parsing through ADE20K Dataset},
author={Zhou, Bolei and Zhao, Hang and Puig, Xavier and Fidler, Sanja and Barriuso, Adela and Torralba, Antonio},
booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
year={2017}
}
```

