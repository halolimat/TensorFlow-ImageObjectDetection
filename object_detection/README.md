
# Tensorflow Image Objects Summarizer

We use the original TensorFlow Object Detection API [link](https://github.com/tensorflow/models/tree/master/research/object_detection) to summarize images for better retrieval during natural disasters.

### Output Classes

We created a mapping for our objects of interest related to our disasters use-case to three classes (i.e., Person, Animal, and Vehicles) as follows:

```json
{ "person": "person",
  "cat": "animal", 
  "dog": "animal", 
  "elephant": "animal", 
  "cow": "animal", 
  "giraffe": "animal", 
  "zerba": "animal", 
  "bear": "animal", 
  "sheep": "animal", 
  "horse": "animal",
  "boat": "vehicles", 
  "truck": "vehicles", 
  "car": "vehicles", 
  "bus": "vehicles"}

### How to use

```python
from ObjectDetector import ObjectDetector
OD = ObjectDetector()
OD.extract(image_url)
```

The example output for the image below is: {"person": 8}

<p align="center">
  <img src="https://www.mmtimes.com/sites/mmtimes.com/files/styles/mmtimes_ratio_c_normal_detail_image/public/news-images/flood-1.jpg?itok=yQk9tJXo" width=70%>
</p>
