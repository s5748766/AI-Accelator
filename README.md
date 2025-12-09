# AI-Accelator
## 자료
[_CH02_딥러닝_알고리즘_1_딥러닝_7공식_73.pdf](https://github.com/user-attachments/files/24045586/_CH02_._._1_._7._73.pdf)

[_CH03_딥러닝_알고리즘_2_활성화함수_69.pdf](https://github.com/user-attachments/files/24045636/_CH03_._._2_._69.pdf)

## 인공 신경망 (Artificial Neural Networks - ANN)
- 생체 신경망과 같이 인공 신경망은 커다란 망으로 함께 연결되어 있는 인공신경을 기반으로 구성되어 있음
- 각각의 인공신경은 생체 신경과 같이 간단한 신호 처리가 가능하도록 구현되어있음

### 구조
#### DNN (Deep Learning Neural Network)
<img width="475" height="213" alt="image" src="https://github.com/user-attachments/assets/db9590b1-1fca-409c-a690-4bdecb7fbad5" />

- Hidden Layer가 2개 이상일 때 심층 신경망(Deep Learning Neural Network - DNN) 이라 함

#### CNN (Convolution Neural Network)
<img width="933" height="446" alt="image" src="https://github.com/user-attachments/assets/1a2b2c68-01e8-4c32-8c88-1f89bcaa19ff" />

- CNN은 이미지 인식에 뛰어난 인공 신경망으로 이미지의 특징을 뽑아내는 인공 신경망과 분류를 위한 인공 신경망으로 구성됨
- Fully Connexted Layer 전 단계는 영상 처리 필터 부분이며, Fully Connexted Layer을 구현하는것이 목표

#### RNN (Recurrent Neural Network structure)
<img width="601" height="429" alt="image" src="https://github.com/user-attachments/assets/c6f14cfc-6f26-411b-a8dd-d38172dc6066" />

- 노드에서 나온 값이 다시 되먹임 되는 형태로 인공 신경망이 구성됨
- RNN 형태의 인공 신경망은 문장 인식에 뛰어난 인공 신경망임

#### 인공 신경 처리 단계
<img width="503" height="321" alt="image" src="https://github.com/user-attachments/assets/47de49ef-3681-40d9-8e0e-6a2ed5801126" />

- 인공 신경은 3개의 처리 단계를 수행
  - 각가의 입력 값은 가중치에 의해 커지거나 작아짐
    <img width="1030" height="386" alt="image" src="https://github.com/user-attachments/assets/2e81224f-850f-4da2-b043-5aaa684eef12" />
    
  - 모든 입력 신호들은 더해짐
    <img width="1026" height="210" alt="image" src="https://github.com/user-attachments/assets/7eb08c66-e8c7-4f56-bcfd-0a95f89827b2" />

  - 신호를 활성화
    <img width="1028" height="141" alt="image" src="https://github.com/user-attachments/assets/23fbda51-14cd-4821-9c33-22fcd1d09a2c" />

#### 인공 신경 함수 수식
<img width="551" height="402" alt="image" src="https://github.com/user-attachments/assets/4276ef50-1ee2-440f-808d-1a795d5b1a74" />

- 입력 값 X의 집합
- 입력 값에 대한 가중치 W의 집합
- 편향 입력 값 1
- 편향 B
- 가중치와 편향을 통해 들어오는 입력 값들의 합
- 그 합을 입력으로 받는 활성화 함수 F
- 활성화 함수 F의 출력 OUT

#### 간단한 인공 신경
<img width="318" height="165" alt="image" src="https://github.com/user-attachments/assets/516bc357-51a4-4c82-9ad7-526e5a51dd24" />

- 수식 : y = x*w + 1*b
- 인공 신경의 학습과정은 가중치 W와 편향 B의 값을 조절하는 과정이며, 인공 신경이 적절히 학습되면 입력값 X에 대해 원하는 출력값 Y가 나오게 됨

## 퍼셉트론
- 퍼셉트론 : 여러 입력을 받아 하나의 출력을 내보내는 가장 기본적인 형태의 인공신경망 모델

### 구조
<img width="443" height="231" alt="image" src="https://github.com/user-attachments/assets/cc8254cd-27d4-4ce3-976a-2cca9f73e6d4" />

<img width="492" height="173" alt="image" src="https://github.com/user-attachments/assets/533e84b9-8752-47d9-9f50-579ec6bef912" />

- t-y는 축삭돌기에서 축삭돌기 말를 표현
- t : threshold (역치)
- x1, x2 : 1 or 0 값 중 하나

### 동작 원리
- x1과 x2는 각각 w1과 w2에 곱해져 s로 전달 : s=x1*w1+x2*w2
- s는 t보다 크면 y로 1이 전달, 그렇지 않으면 0이 전달
- t값이 작을 수록 yfh 쉽게 신호 (1)이 전달 됨
- ex) t = 0.1이면 s값은 0.1만 넘으면 y로 1이 전

<img width="380" height="87" alt="image" src="https://github.com/user-attachments/assets/e74f03f8-25f2-459a-bd16-d2257962beb7" />

### 퍼셉트론과 논리 게이트
#### AND 게이트
<img width="1029" height="331" alt="image" src="https://github.com/user-attachments/assets/41bdb675-f121-40f1-8472-2915cb407897" />

#### NAAD 게이트
<img width="1023" height="268" alt="image" src="https://github.com/user-attachments/assets/ae8dc2e8-ed58-4cdd-b9b1-a27c684c2453" />

#### OR 게이트
<img width="1020" height="266" alt="image" src="https://github.com/user-attachments/assets/92cd8624-a15c-4085-b77e-2657d85a10c8" />

### 퍼셉트론 구현 (파이썬)

### 퍼셉트론 한계 XOR 게이트
- 초기에 단층 신경망으로 구성
- XOR 게이트에서 2번 식과 8번 식를 동시에 만족할 수 없음
<img width="1019" height="293" alt="image" src="https://github.com/user-attachments/assets/d2e860cd-b506-4fa4-9958-f3b9e824c13b" />

### 다층 퍼셉트론으로 해결 XOR 게이트
- 다층 퍼셉트론 : 입력층, 은닉층, 출력층으로 구성
<img width="1020" height="199" alt="image" src="https://github.com/user-attachments/assets/f166d36a-484e-4aca-986d-09658bacb238" />

- 두개의 입력값, 하나의 출력값을 가진 단층 퍼셉트론 3개를 조합
<img width="667" height="217" alt="image" src="https://github.com/user-attachments/assets/8b7b56bc-8b4c-4521-94a2-ff4678c40a8c" />

### 파이썬으로 구현
<img width="677" height="618" alt="image" src="https://github.com/user-attachments/assets/080b8d92-7781-4229-b4d3-fdbff996859a" />

## 딥러닝 7 공식!
- 딥러닝 7 공식을 이용하여 딥러닝의 동작 원리 이해
- 순전파, 목표값, 오차, 역전파 오차, 역전파, 학습률
- 학습 방법 : 가중치 w와 편향 b의 값을 조정

### 딥러닝 제 1 공식 : 순전파
<img width="295" height="149" alt="image" src="https://github.com/user-attachments/assets/5826b511-f627-4c7a-9368-a0e880f8c41e" />

- 입력 노드 1개, 출력 노드 1개, 편향으로 구성된 단일 인공 신경
- 이 인공 신경을 학습 시키면 다음과 같이 가중치와 편향의 값이 바뀌게 됩니다. 즉, 신호 전달 강도가 더 세지거나 약해짐

#### 순전파 수식
- y는 예측값, x는 입력값, w는 가중치, b는 편향
<img width="539" height="146" alt="image" src="https://github.com/user-attachments/assets/c5e3540d-c937-4c8e-8093-5692d3b44b86" />

### 딥러닝 제 2 공식 : 평균 제곱 오차
- 딥러닝 제 2 공식
<img width="644" height="44" alt="image" src="https://github.com/user-attachments/assets/0f992f7b-b58f-4d26-8835-3d3caeaa9651" />

- 1 공식에서 나온 y = 7이라는 값을 목표한 10이라는 값으로 바꾸고 싶은데, 이 경우 yT에 10을 넣고 평균 제곱 오차 계산!

### 딥러닝 제 3 공식 : 역전파 오차
- 딥러닝 제 3 공식
<img width="646" height="44" alt="image" src="https://github.com/user-attachments/assets/42f6e6fe-d02c-4814-ac08-5cedeeee13ae" />

- yE에 대한 y 방향의 기울기를 나타냄
- w와 b의 값을 변경해야함
- 역전파에 사용할 오차값을 의미
- 기울기가 0인 지점을 찾는 것이 목표

### 딥러닝 제 4 공식 : 입력 역전파
- 딥러닝 제 4 공식
<img width="927" height="268" alt="image" src="https://github.com/user-attachments/assets/20aa0562-8aa7-4219-8f61-1a23c69c3e1a" />

- xE의 오차는 yE의 오차 * w
- 기울기(-3)를 거꾸로 보냄

### 딥러닝 제 5 공식 : 가중치, 편향 순전파
- 딥러닝 제 5 공식
<img width="963" height="334" alt="image" src="https://github.com/user-attachments/assets/ee98a5c5-1b4b-4e61-b6ba-7cfa13090077" />

### 딥러닝 제 6 공식 : 가중치, 편향 역전파
- 딥러닝 제 6 공식
<img width="833" height="241" alt="image" src="https://github.com/user-attachments/assets/a6322693-8f32-41ac-8ff4-b351ebdd1b9b" />

### 딥러닝 제 7 공식 : 신경망 학습
- 딥러닝 제 7 공식
<img width="712" height="81" alt="image" src="https://github.com/user-attachments/assets/ff1c87ae-9f7f-42e8-88bf-cc3f3a634aee" />

- wE는 가중치 역전파 오차, bE는 편향 역전파 오차
- lr(learning rate)은 학습률을 의미



#### 신경망 학습 (파이썬)
- 신경망 학습
<img width="349" height="183" alt="image" src="https://github.com/user-attachments/assets/c5110581-8a22-4955-820d-70d0401c5eb2" />

- 학습률 적용
<img width="350" height="190" alt="image" src="https://github.com/user-attachments/assets/3169ecc8-3155-427b-a8bc-a6cca03a4a71" />

- α는 학습률을 의미
- 학습률의 값은 0.001로 시작하여 학습이 진행되는 상황에 따라 조금씩 늘리거나 줄여서 사용

```
x = 2
w = 3
b = 1
yT = 10 
lr  = 0.01

for epoch in range(1800):
    y = x * w + 1 * b
    E = (y - yT)**2 / 2
    yE = y - yT
    wE = yE*x
    bE = yE*1
    w -= lr*wE
    b -= lr*bE
    print(f'epoch = {epoch}')
    print(f' y : {y:.3f}')
    print(f' w : {w:.3f}')
    print(f' b : {b:.3f}')
    
    if E < 0.0000001 :
        break

```

### 딥러닝 반복 학습
<img width="321" height="187" alt="image" src="https://github.com/user-attachments/assets/bf27ddea-893e-442e-a3d0-203e515210a6" />

## 연습문제
### 문제 1
<img width="570" height="636" alt="image" src="https://github.com/user-attachments/assets/a2418d72-f965-40e4-a813-3b6776e36d95" />

```
x1, x2 = 0.05, 0.10
w1, w2, w3, w4, w5, w6 = 0.15, 0.20, 0.25, 0.30, 0.40, 0.55
b1, b2, b3 = 0.35, 0.45, 0.60
y1T, y2T, y3T= 0.01, 0.99, 0.50
lr = 0.01

for epoch in range(2000):
    y1 = x1*w1 + x2*w2 + 1*b1
    y2 = x1*w3 + x2*w4 + 1*b2
    y3 = x1*w5 + x2*w6 + 1*b3
    E = ((y1-y1T)**2 + (y2-y2T)**2 + (y3-y3T)**2)/2
    y1E = y1-y1T
    y2E = y2-y2T
    y3E = y3-y3T
    w1E = y1E*x1
    w2E = y1E*x2
    b1E = y1E*1
    w3E = y2E*x1
    w4E = y2E*x2
    b2E = y2E*1
    w5E = y3E*x1
    w6E = y3E*x2
    b3E = y3E*1
    w1 = w1-lr*w1E
    w2 = w2-lr*w2E
    b1 = b1-lr*b1E
    w3 = w3-lr*w3E
    w4 = w4-lr*w4E
    b2 = b2-lr*b2E
    w5 = w5-lr*w5E
    w6 = w6-lr*w6E
    b3 = b3-lr*b3E
       
    
    if E < 0.0000001:
        print(f'epoch = {epoch}')
        print(f' y1 : {y1:.3f}')
        print(f' y2 : {y2:.3f}')
        print(f' y3 : {y3:.3f}')
        print(f' w1 : {w1:.3f}')
        print(f' w2 : {w2:.3f}')
        print(f' b1 : {b1:.3f}')
        print(f' w3 : {w3:.3f}')
        print(f' w4 : {w4:.3f}')
        print(f' b2 : {b2:.3f}')
        print(f' w5 : {w5:.3f}')
        print(f' w6 : {w6:.3f}')
        print(f' b3 : {b3:.3f}')
        break
```

### 문제 2
<img width="570" height="770" alt="image" src="https://github.com/user-attachments/assets/13ab9f95-14fd-4c54-b455-51e5b8d9c488" />

```
x1, x2, x3 = 0.02, 0.05, 0.12
w1, w2, w3, w4, w5, w6 = 0.15, 0.20, 0.02, 0.27, 0.37, 0.52
b1, b2 = 0.12, 0.39
y1T, y2T = 0.02, 0.98
lr = 0.01

for epoch in range(2000):
    y1 = x1*w1 + x2*w2 + x3*w3 + 1*b1
    y2 = x1*w4 + x2*w5 + x3*w6 + 1*b2
    E = ((y1-y1T)**2 + (y2-y2T)**2)/2
    y1E = y1-y1T
    y2E = y2-y2T
    
    w1E = y1E*x1
    w2E = y1E*x2
    w3E = y1E*x3
    b1E = y1E*1
    w4E = y2E*x1
    w5E = y2E*x2
    w6E = y2E*x3
    b2E = y2E*1
    
    w1 = w1-lr*w1E
    w2 = w2-lr*w2E
    w3 = w3-lr*w3E
    b1 = b1-lr*b1E
    w4 = w4-lr*w4E
    w5 = w5-lr*w5E
    w6 = w6-lr*w6E
    b2 = b2-lr*b2E
    
    if E < 0.0000001:
        print(f'epoch = {epoch}')
        print(f' y1 : {y1:.3f}')
        print(f' y2 : {y2:.3f}')
        print(f' w1 : {w1:.3f}')
        print(f' w2 : {w2:.3f}')
        print(f' w3 : {w3:.3f}')
        print(f' b1 : {b1:.3f}')
        print(f' w4 : {w4:.3f}')
        print(f' w5 : {w5:.3f}')
        print(f' w6 : {w6:.3f}')
        print(f' b2 : {b2:.3f}')
        break
```
