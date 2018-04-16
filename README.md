# TF-Dataset-Creator
[How to create your own dataset with Tensorflow Object Detection API](http://yongyong-e.tistory.com/31?category=763033).


## Requirements
- Ubuntu 16.04
- Python 3.5
- [Tensorflow 1.4](http://yongyong-e.tistory.com/10)


## Getting Started
Creating virtualenv
1. `git clone https://github.com/yonghankim/TF-Dataset-Creator.git`
2. `cd TF-Dataset-Creator`
3. `virtualenv env --python=python3.5`
4. `source env/bin/activate`

Install Dependencies
- `pip install -r requirements.txt`

xml to csv
- `python xml_to_csv.py`

Convert to TFRecord format
- `python generate_tfrecord.py --csv_input=data/train_labels.csv --output_path=data/train.record`
- `python generate_tfrecord.py --csv_input=data/test_labels.csv --output_path=data/test.record`
