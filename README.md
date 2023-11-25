# Depth-Estimation

### 11.18 / 01:50 : DinoV2 구동 성공<br/>
지금까지 실패했던 이유 : cuda version이 안맞았기 때문.<br/>
pytorch 2.0.0은 cuda 12.2.0 지원 X.  -> **cuda version을 11.8.0으로 downgrade하여 해결 완료.** <br/>
<br/>
### 11.25 / 19:00 : DinoV2, Jetson-Inference 구동 및 실험 완료.<br/>
DinoV2 : Grabcut 미활용/활용으로 실험 결과 각각 생성 완료. <br/>
Jetson-Inference : 추출한 Depth Map을 Grayscale로 변환하여 MSE 추출. <br/>
