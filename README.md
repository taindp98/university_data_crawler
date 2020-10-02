
Mục tiêu Project:

+ Thu thập gần 1 triệu dữ liệu điểm thi THPT Quốc gia năm 2019, 2020
 
+ Thu thập điểm chuẩn đại học 2014 - 2019

+ Phân tích dữ liệu

  

# Development

```bash
# OS Any (Ubuntu - Recommend)

#install python 
# detail: deploy/docs/install_python.md

#install python 3.7
# detail: deploy/docs/install_python37.md


git clone https://github.com/beecost/bee-university.git
cd bee-university
git config credential.helper store
 

virtualenv venv -p python3.7
source venv/bin/activate
pip install -r requirements.txt

# Update folder path in init.py
python init.py
python init_server.py

# Crawl danh sách url trường đại học
python crawler/crawler_university_list.py
# Crawl điểm chuẩn từ 2014 - 2019
python crawler/crawl_diemchuan.py
# Crawl điểm thi 2020 64 tỉnh thành
python crawler/diemthi2020/crawler_diemthi2020.py
```
