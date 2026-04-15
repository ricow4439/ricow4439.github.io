---
layout: cv
title: Jungwoo Lee's CV
---
<img src="./img/ljw.jpg" alt="Profile" width="150" style="border-radius: 50%; display: block; margin-bottom: 20px;" />

# __Jungwoo Lee (이정우)__

Robot Software System Integration & AI Developer

<div id="webaddress">
<!-- <a href="mailto:ricow4439@gmail.com">ricow4439@gmail.com</a> | -->
<a href="https://www.linkedin.com/in/정우-이-486838395">LinkedIn</a>
</div>

## <b><u>Profile</u></b>

안녕하세요! 저는 Software system integration, 로봇의 인지와 행동 추론 등 다양한 분야에 대한 AI 모델을 만들고 있습니다. 

## <u>Skills</u>

#### Good knowledge
- Tensorflow, Torch, ROS

#### Basic knowledge
- Hardware (ST MCU, TI DSP), PLC (LSIS), OrCAD (Circuit Design)

#### Languages
- Python, C++, C#, Perl, Assembly (for debugging)

#### AI
- Claude, Codex, Gemini, Local LLM (MiniMax, Qwen3.5, GPT-OSS) for Coding Agent 

## <u>Experience</u>

`2007.11 - 현재` | 
__[한국로봇융합연구원(Korea Institute of Robotics and Technology Convergence)](https://www.kiro.re.kr)__, 책임연구원 (SI / AI Model Development)

`2004.11 - 2007.09` | 
__한국과학기술연구원 영상미디어연구센터(IMRC)__, 위촉연구원 (로봇 미들웨어 개발)

`2003.12 - 2004.06` | 
__삼성종합기술원 HCI Lab__, 위촉연구원 (하드웨어 개발)

## <u>Education</u>

`2020-2024` | 
__부경대학교 기계시스템공학 박사__  : "A Study on ROV Attitude Control and Marine Glider Detection for Glider Recovery Using a Deep Learning Model" (Ph.D. Dissertation)

`2013-2015` | 
__한국과학기술원 소프트웨어공학 석사__

`1999-2005` | 
__한양대학교 전자통신컴퓨터공학 학사__

## <u>Projects</u>

### 2026
- #### BOP (Benchmark for 6D Object Pose Estimation) : 2025 ~ 진행 중
  - HOPE (NVIDIA Household Objects for Pose Estimation) Dataset에 대한 6D-Pose + Object Size + ID 추정을 위한 모델 개발 (Tensorflow & Torch, from scratch)
  - Encoder-only Transformer (MoE는 layer 별 가변 experts) 설계 적용
  - 모델 입력은 카메라의 Depth -> Point Clouds, 모델 출력은 객체의 6D-Pose + Object Size + ID

- #### Underwater Glider Detection을 위한 3D 위치 추정 : 2025 ~ 2026
  - ROV 탑재된 Camera의 Color Image에서 수중 글라이더의 위치를 추정하는 모델 개선 (Tensorflow, from scratch)
  - Vision Encoder는 Hierarchical Convolutional Neural Network을 설계하고, 가변 MoE 구현 적용
  - __["A Study of the Three-Dimensional Localization of an Underwater
Glider Hull Using a Hierarchical Convolutional Neural Network
Vision Encoder and a Variable Mixture-of-Experts Transformer"](https://www.mdpi.com/2072-4292/18/5/793)__

- #### VLA Training : 2026 ~ 진행 중
  - DROID Dataset을 증강(Depth 생성과 context 추가)하여, VLM(Gemma or Qwen) 모델에 대한 PEFT + Custom Head 로 학습 진행 (Torch)
 
- #### Local Model Fine-tunning : 2026 ~ 진행 중
  - 여러 Local Model의 추론 실행 속도 향상과 특정 도메인이 주어졌을 때의 최적화를 목표로 함
  - Model에 대한 Multi-Modal Encoder Hub, Backbone layers에 대한 동적 라우팅과 PEFT (FFN or MoE), Custom Head 에 대한 시험 진행 

- #### Embedded-AI 를 위한 자원 제한된 하드웨어 적응형 동적 신경망 설계 연구 : 2026 ~ 진행 중
  - 하드웨어 자원 제한(전력, 처리능력)된 경우 모델 추론을 조절하는 동적 신경망 구현
  - YOLO26 Detector 기반 Dynamic Neural Network (Early Exit, Adaptive Routing) 적용 연구 진행 

### 2025
- #### Dishware Pose Estimation : 2025
  - 식당에서 식기 수거를 위한 로봇의 식기 인식을 위한 자세 추정 모델 개발 (Tensorflow, from scratch)
  - Encoder-only Transformer (Custom Attention, MoE) 설계 적용
  - 모델 입력은 카메라의 Color 및 Depth image, 모델 출력은 식기의 6D-Pose + Size + ID로 구성
  - __["Model-Free Transformer Framework for 6-DoF Pose Estimation of Textureless Tableware Objects"](https://www.mdpi.com/1424-8220/25/19/6167)__
  - [![개별 식기 포즈 인식 결과](./img/dishpose_each_4x.jpg)](./img/dishpose_each_4x_convert.mp4)
<details>
  <summary>🔍 클릭하여 영상 보기</summary>
  <br>
  <video src="./img/dishpose_each_4x_convert.mp4" controls width="50%"></video>
</details>

- #### 객체 포즈 추정을 위한 Transformer Model 개선 : 2025
  - 객체의 Point-Cloud로부터 포즈 추정을 위한 Encoder-only Transformer Model에 대한 성능 개선 목표
  - Transformer Model 내부의 Attention 구조 변형과 GQA, RMS Norm의 적용 등에 대한 Ablation study 비교하고, GPU 메모리 사용량을 baseline model 대비 2.5%로 감소
  -  __["A Study on Systematic Improvement of Transformer Models for Object Pose Estimation"](https://www.mdpi.com/1424-8220/25/4/1227)__

### ~ 2024
- #### Title
  - Description  
  - [![설명문구](GIF_파일_주소)](이동할_링크_주소)
    

<!-- ### Footer

Last updated: 2026 -->
