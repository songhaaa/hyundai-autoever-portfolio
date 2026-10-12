
<div align="center">

# AI Research Portfolio

### LLM | RAG & Multi-Agent | Deep Learning | AI Optimization

**문제를 정의하고, 직접 설계하며, 결과로 검증하는 AI 개발자**

<br>

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-17406D?style=flat-square)
![RAG](https://img.shields.io/badge/RAG%20%26%20Agent-2474B5?style=flat-square)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-5865A8?style=flat-square)

<br>

### 📄 [View Full Portfolio (PDF)](./현대오토에버_포트폴리오_김송하.pdf)

*현대오토에버 AI 데이터 서비스 개발 직무 지원 포트폴리오*

</div>

---

## 👩‍💻 About Me

고려대학교 인공지능학과에서 석사학위를 취득했으며, LLM 추론 최적화와 딥러닝 모델의 성능 개선을 중심으로 연구했습니다.

- **LLM & Agent:** 검색 근거의 신뢰성 향상과 Multi-Agent 기반 추론 구조 설계
- **Model Optimization:** 정확도를 유지하면서 추론 연산량을 줄이는 효율화 전략 개발
- **Robust AI:** 불완전한 라벨과 사용자 간 데이터 분포 차이에 대응하는 딥러닝 모델 설계
- **AI Applications:** 데이터 전처리부터 모델 학습, 성능 평가, 웹서비스 구현까지 경험

연구 과정에서 문제의 원인을 분석하고, 개선 방법을 직접 구현한 뒤 다양한 실험으로 효과를 검증하는 데 집중했습니다.

---

## 🚀 Featured Projects

### 01. Multi-Agent RAG for Reliable Question Answering

**선택지별 근거 검증 및 재검색을 활용한 RAG 추론 성능 개선**

`Python` `LLM` `RAG` `Multi-Agent` `Information Retrieval`

**Problem**
- 기존 RAG는 특정 정답 후보를 지지하는 근거에 치우쳐 선택지 간 상충하는 정보를 충분히 비교하지 못하는 한계가 존재했습니다.

**Approach & Contribution**
- 선택지별 지지 및 반박 근거를 병렬 탐색하는 Dual-Branch Retrieval 설계
- Evidence Scoring 기반 근거 평가 및 재검색 대상 선별
- Agent별 검색, 검증, 지식 보완 역할을 분담하고 선택지 간 충돌에 따라 Targeted Re-retrieval 수행
- 전체 Multi-Agent 구조 설계, Python 구현 및 실험 분석 주도

**Results**
- 3개 의료 QA 벤치마크에서 기존 방식 대비 평균 정확도 **+3.48%p 향상**

---

### 02. Efficient LLM Reasoning with Implicit CoT

**Early-Exit 기반 LLM 추론 효율 최적화**

`Python` `LLM` `Implicit CoT` `Early-Exit` `Model Optimization`

**Problem**
- 기존 Implicit CoT는 문제 난이도와 관계없이 고정된 추론 단계를 수행하여 불필요한 연산이 발생했습니다.

**Approach & Contribution**
- 중간 추론 상태를 분석하여 불필요한 추론을 조기 종료하는 Early-Exit 전략 설계
- Confidence, Latent Consistency, Reasoning Stability, Answer Agreement를 활용한 종료 조건 구성
- 1B/3B 규모 LLM과 4개 수학 추론 데이터셋을 대상으로 성능 및 추론 효율 비교 실험 수행

**Results**
- 평균 정확도 **56.2% 유지**
- 평균 Latent Reasoning Step **7.7% 감소**

---

### 03. CASPER: Semi-Supervised EEG Emotion Recognition

**신뢰도 기반 의사라벨 보정과 프로토타입 갱신을 통한 학습 안정화**

`Python` `PyTorch` `Semi-Supervised Learning` `Prototype Learning`

**Problem**
- EEG 데이터는 라벨 확보가 어렵고 노이즈가 많으며, 준지도 학습 초기의 부정확한 의사라벨과 프로토타입이 반복 반영되면서 Confirmation Bias가 발생합니다.

**Approach & Contribution**
- Confidence Bank를 활용한 적응형 2단계 의사라벨 보정 구조 설계
- 거리 가중치 기반 프로토타입 업데이트로 부정확한 클래스 중심의 영향을 완화
- 모델 설계, 학습 파이프라인 구현, 비교 실험 및 결과 분석 주도

**Results**
- 기존 SOTA 대비 평균 정확도 **+2.09%p 향상**
- **ICASSP 2026 제1저자 논문 발표**
- 국내 특허 1건 출원 및 소프트웨어 저작권 1건 등록

---

### 04. HiProCo: Cross-Subject EEG Generalization

**계층적 프로토타입 정렬을 통한 피험자 간 일반화 성능 개선**

`Python` `PyTorch` `Contrastive Learning` `Domain Generalization`

**Problem**
- EEG는 피험자마다 신호 분포가 달라, 전체 데이터를 평균한 단일 클래스 프로토타입만으로는 개인차를 충분히 반영하기 어렵습니다.

**Approach & Contribution**
- Subject-specific Class Prototype 기반 대조학습 설계
- Global Class Prototype과의 계층적 정렬을 통해 피험자 간 분포 차이 완화
- Wilcoxon Signed-Rank Test를 활용해 성능 개선의 통계적 유의성 검증

**Results**
- 기존 SOTA 대비 평균 정확도 **+2.32%p 향상**
- 국제저널 *Expert Systems with Applications* 제1저자 논문 투고
- 국내 특허 1건 출원

---

### 05. Speech Emotion Recognition Web Application

**CNN-Transformer 기반 음성 감정 인식 및 웹서비스 개발**

`Python` `CNN` `Transformer` `Mel-Spectrogram` `Django`

**Problem**
- 화자별 음성 특성과 발화 환경 차이로 인해 규칙 기반 방식만으로는 안정적인 감정 분류가 어렵습니다.

**Approach & Contribution**
- RAVDESS 음성 데이터 전처리 및 Mel-Spectrogram 특징 추출
- CNN과 Transformer Encoder를 결합한 7개 감정 분류 모델 개발
- Django 기반 음성 업로드 및 감정 분석 결과 확인 웹서비스 구현

**Results**
- 감정 분류 정확도 약 **57% 달성**
- 한국외국어대학교 캡스톤설계 **27개 팀 중 1위, 최우수상 수상**
- 2023 SW인재 페스티벌 우수작품 발표

---

## 🔬 Additional Research & Projects

| Research | Key Contributions | Publication |
|:---|:---|:---|
| **RAG-based Knowledge Connection** | FLAIR Baseline 구현, 8개 데이터셋 비교 실험, Human Evaluation 및 논문 검수 | EMNLP 2025 |
| **Cross-Subject Visual Brain Decoding (CroSS)** | Soft Alignment 및 Subject-aware Normalization 기반 모델 최적화, 실험 및 논문 검수 | ACM SAC 2026 |
| **Multi-Level EEG-to-Image Alignment** | EEG와 CLIP의 다층 시각 표현 정렬 연구에서 실험 최적화 및 논문 검수 | ICASSP 2026 |
| **Wine Quality Classification** | R 기반 데이터 전처리, 변수 선택, 4개 머신러닝 모델 구현 및 비교 | Data Mining Project |

---

## 🏆 Publications & Achievements

| Category | Achievement |
|:---|:---|
| International Conference | ICASSP 2026 제1저자 발표 |
| International Conference | EMNLP 2025 공저 |
| International Conference | ACM SAC 2026 공저, Honorable Mention in AI & Agents |
| International Journal | Expert Systems with Applications 제1저자 논문 투고 |
| Best Paper Award | NCAEIC 2023 |
| Intellectual Property | 국내 특허 3건 출원, SW 저작권 1건 등록 |
| Capstone Design | 최우수상, 27개 팀 중 1위 |

---

## 🛠️ Technical Skills

| Category | Skills |
|:---|:---|
| Programming | Python, R, Java, C/C++ |
| AI Framework | PyTorch |
| Generative AI | LLM, RAG, Multi-Agent, Implicit CoT |
| Machine Learning | Deep Learning, Contrastive Learning, Semi-Supervised Learning |
| Data & Application | Data Preprocessing, Model Evaluation, Django |
| Development Tools | Git, Linux |

---

<div align="center">

### 📬 Contact

**Email:** songhakim00@gmail.com

*Thank you for visiting my portfolio!*

</div>
