# data_maker
data maker


## Install
pip install git+https://github.com/skku-shinhan-bank/data_maker.git

## Usage

```python
from data_maker import DataMaker

train_shinhan_data, train_shinhan_label, test_shinhan_data, test_shinhan_label = DataMaker.make_shinhan_issue_class_data(
    "/content/drive/MyDrive/신한은행/training-data/Labeled_Data_2/shinhan_app_review_4.xlsx",
    "/content/drive/MyDrive/신한은행/training-data/text_data_index.txt",
    )

hana_data, hana_label = DataMaker.make_issue_class_data_from_crawled("/content/drive/MyDrive/신한은행/training-data/Labeled_Data_2/hana_app_review.xlsx")
woori_data, woori_label = DataMaker.make_issue_class_data_from_crawled("/content/drive/MyDrive/신한은행/training-data/Labeled_Data_2/woori_app_review.xlsx")
shinhan_data, shinhan_label = DataMaker.make_issue_class_data_from_crawled("/content/drive/MyDrive/신한은행/training-data/Labeled_Data_2/c_shinhan_app_review.xlsx")
```
