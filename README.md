# DACON_growth
![20220524_122407](https://user-images.githubusercontent.com/84311270/169942540-34089cc3-c47d-42bd-9310-76bfe6c50147.png)
식물 생육을 위한 최적의 환경 도출.

## Dataset
1. train_dataset [Folder]  
 ├ LT [Folder]  
 │ ├ LT_01 [Folder]  
 │ │ ├ DAT00.png  
 │ │ ├ DAT01.png  
 │ │ ├ DAT02.png  
 │ │ └  ...  
 │ └  ...  
 ├ BC [Folder]  
 │ ├ BC_01 [Folder]  
 │ │ ├ DAT00.png  
 │ │ ├ DAT01.png  
 │ │ ├ DAT02.png  
 │ │ └  ...  
 │ └  ...  

2. test_dataset [Folder]  
 ├ LT [Folder]  
 │ ├ 1003 [Folder]  
 │ │ ├ idx_LT_1003_00010.png  
 │ │ ├ idx_LT_1003_00019.png  
 │ │ ├ idx_LT_1003_00034.png  
 │ │ └  ...  
 │ └  ...  
 ├ LT [Folder]  
 │ ├ 1088 [Folder]  
 │ │ ├ idx_BC_1088_00010.png  
 │ │ ├ idx_BC_1088_00030.png  
 │ │ ├ idx_BC_1088_00036.png  
 │ │ └  ...  
 │ └  ...  

 ├ test_data.csv  
 │ ├ idx : 테스트 데이터 인덱스값  
 │ ├ before_file_path : 이전 사진 이미지 파일명  
 │ ├ after_file_path : 이후 사진 이미지 파일명  



3. sample_submission.csv  
idx : test_data.csv의 index와 매칭  
time_delta : test_data.csv에서의 before_file_path에 해당하는 이미지부터 after_file_path에 해당하는 이미지까지 식물의 생육기간을 예측 

## Model
MobileNet을 사용하여 진행.
