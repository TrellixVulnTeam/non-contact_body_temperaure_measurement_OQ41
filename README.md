# iot와 얼굴인식을 이용한 비접촉 체온측정기기
### 기능
1. 온도 측정과 출입자 정보 저장 및 관리
> + 온도 측정은 열화상 카메라와 열 센서로 측정
> + QR 코드를 통하여 출입자 정보 확인
> + 모든 정보는 서버의 데이터 베이스에 저장

![way](https://user-images.githubusercontent.com/78341072/149776735-4e4a3a6b-4740-4082-a3a6-ffe17e1c586b.png)

2. 얼굴 인식을 통한 사람 얼굴 위치 확인 및 카메라 이동
> + 카메라에 인식된 얼굴의 위치에 따라 카메라가 모터를 통해 상하 이동하여 얼굴을 중앙에 위치하도록 함
3. 주변 환경에 따라 계산된 보정 온도를 추가하여 측정 온도의 정확도를 증가 
> + 내부 환경과 외부 환경 데이터로 지도 학습을 통해 보정 온도를 계산하여 측정 온도와 합산
-------
### 사용 하드웨어 및 소프트웨어
+ 라즈베리파이4 8gb
+ 7인치 라즈베리파이 디스플레이
+ 라즈베리파이 카메라 v2
+ MLX90614 비접촉 온도센서
+ AMLA_150mm 리니어 액추에이터
+ 28BYJ-48
+ flir dev kit 열화상 카메라 + usb 연결 포트
+ getthermal 프로그램
+ firebase

![hw2](https://user-images.githubusercontent.com/78341072/149776530-05fce5be-8787-4705-bc7e-70b4f39beb59.png)
--------------------
### 실행
1. getthermal 설치 및 실행 (https://github.com/groupgets/GetThermal)
2. run.py 실행
```
  sudo run.py
```
