# Depth-Estimation

### 11.18 / 01:50 : DinoV2 구동 성공<br/>
지금까지 실패했던 이유 : cuda version이 안맞았기 때문.<br/>
pytorch 2.0.0은 cuda 12.2.0 지원 X.  -> **cuda version을 11.8.0으로 downgrade하여 해결 완료.** <br/>
<br/>
### 11.25 / 19:00 : DinoV2, Jetson-Inference 구동 및 실험 완료.<br/>
DinoV2 : Grabcut 미활용/활용으로 실험 결과 각각 생성 완료. <br/>
Jetson-Inference : 추출한 Depth Map을 Grayscale로 변환하여 MSE 추출. <br/>
<br/>
### 11.27 : 03:00 실험 환경 세팅 방법 및 MSE 추출 프로그램 작성.<br/>
공통 : Mask 추출하여 Depth Estimation을 진행하는 방안 구현 / Mask 활용,미활용에 따른 MSE 추출 완료.
DinoV2 : DinoV2 환경을 조성할 수 있는 Dockerfile 재정리 및 MSE 추출하는 프로그램을 따로 분리.
Jetson-Inference : Depthnet.py를 사용하여 깊이 맵을 생성하는 쉘 스크립트 작성 및 실험 완료.
