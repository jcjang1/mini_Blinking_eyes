# Mini_Project - Blinking_eyes

Yolo v4 모델을 Darknet을 이용해 Training하고 Webcam을 통해 real time Detecting 하는 project 진행

- drive_class.ipynb : Data 전처리 코드를 class화
  - all_data_path : 학습을 위한 이미지의 모든 데이터 경로를 한 txt 파일에 write하여 저장하는 함수
  - pick_data_path : 사용할 이미지의 경로만 한 txt파일에 write하여 저장하는 함수
  - shuffle_pick : 학습시 데이터를 골고루 사용할 수 있도록 shuffle하는 함수
  - resize_img : image resizing 함수
  - data_split_txt : train / valid / test로 split하는 함수
  - json_path : 사용할 이미지의 json파일 경로만 모아주는 함수
  - json_to_txt : json파일을 불러와 모델 학습을 위해 (label, x, y, w, h)로 변환하여 txt파일에 저장 시키는 함수

- drive_run.ipynb : 데이터 전처리 및 모델 학습, webcam으로 실행
