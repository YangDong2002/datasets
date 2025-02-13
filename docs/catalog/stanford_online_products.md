<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>
  <meta itemprop="name" content="stanford_online_products" />
  <meta itemprop="description" content="Stanford Online Products Dataset&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load(&#x27;stanford_online_products&#x27;, split=&#x27;train&#x27;)&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;&lt;img src=&quot;https://storage.googleapis.com/tfds-data/visualization/fig/stanford_online_products-1.0.0.png&quot; alt=&quot;Visualization&quot; width=&quot;500px&quot;&gt;&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/stanford_online_products" />
  <meta itemprop="sameAs" content="http://cvgl.stanford.edu/projects/lifted_struct/" />
  <meta itemprop="citation" content="@inproceedings{song2016deep,&#10; author    = {Song, Hyun Oh and Xiang, Yu and Jegelka, Stefanie and Savarese, Silvio},&#10; title     = {Deep Metric Learning via Lifted Structured Feature Embedding},&#10; booktitle = {IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},&#10; year      = {2016}&#10;}" />
</div>

# `stanford_online_products`


*   **Visualization**:
    <a class="button button-with-icon" href="https://knowyourdata-tfds.withgoogle.com/#tab=STATS&dataset=stanford_online_products">
    Explore in Know Your Data
    <span class="material-icons icon-after" aria-hidden="true"> north_east
    </span> </a>

*   **Description**:

Stanford Online Products Dataset

*   **Homepage**:
    [http://cvgl.stanford.edu/projects/lifted_struct/](http://cvgl.stanford.edu/projects/lifted_struct/)

*   **Source code**:
    [`tfds.image_classification.StanfordOnlineProducts`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/image_classification/stanford_online_products.py)

*   **Versions**:

    *   **`1.0.0`** (default): No release notes.

*   **Download size**: `2.87 GiB`

*   **Dataset size**: `Unknown size`

*   **Auto-cached**
    ([documentation](https://www.tensorflow.org/datasets/performances#auto-caching)):
    Unknown

*   **Splits**:

Split     | Examples
:-------- | -------:
`'test'`  | 60,502
`'train'` | 59,551

*   **Features**:

```python
FeaturesDict({
    'class_id': ClassLabel(shape=(), dtype=tf.int64, num_classes=22634),
    'image': Image(shape=(None, None, 3), dtype=tf.uint8),
    'super_class_id': ClassLabel(shape=(), dtype=tf.int64, num_classes=12),
    'super_class_id/num': ClassLabel(shape=(), dtype=tf.int64, num_classes=12),
})
```

*   **Supervised keys** (See
    [`as_supervised` doc](https://www.tensorflow.org/datasets/api_docs/python/tfds/load#args)):
    `None`

*   **Figure**
    ([tfds.show_examples](https://www.tensorflow.org/datasets/api_docs/python/tfds/visualization/show_examples)):

<img src="https://storage.googleapis.com/tfds-data/visualization/fig/stanford_online_products-1.0.0.png" alt="Visualization" width="500px">

*   **Examples**
    ([tfds.as_dataframe](https://www.tensorflow.org/datasets/api_docs/python/tfds/as_dataframe)):

<!-- mdformat off(HTML should not be auto-formatted) -->

{% framebox %}

<button id="displaydataframe">Display examples...</button>
<div id="dataframecontent" style="overflow-x:auto"></div>
<script src="https://www.gstatic.com/external_hosted/jquery2.min.js"></script>
<script>
var url = "https://storage.googleapis.com/tfds-data/visualization/dataframe/stanford_online_products-1.0.0.html";
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
@inproceedings{song2016deep,
 author    = {Song, Hyun Oh and Xiang, Yu and Jegelka, Stefanie and Savarese, Silvio},
 title     = {Deep Metric Learning via Lifted Structured Feature Embedding},
 booktitle = {IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
 year      = {2016}
}
```

