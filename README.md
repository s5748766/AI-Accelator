# AI-Accelator
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


