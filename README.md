# Project_FinFit
 Data-driven healthcare service project
## 목차
## 서비스 소개 (개요)
## 주요 기능 및 담당 업무
## 프로젝트 목표
## 프로젝트 진행관리
## 스킬 앤 툴스
## ▪ Language
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)



## ▪ Backend(server)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=flat&logo=mariadb&logoColor=white)



## ▪ Frontend
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat&logo=bootstrap&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat&logo=chartdotjs&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)



## ▪ Data Science / ML
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=flat&logo=xgboost&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3C5A6F?style=flat&logo=seaborn&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-000000?style=flat&logo=langchain&logoColor=white)



## ▪ API & External Services
![YouTube API](https://img.shields.io/badge/YouTube_API-FF0000?style=flat&logo=youtube&logoColor=white)
![Naver API](https://img.shields.io/badge/Naver_API-03C75A?style=flat)
![Gemini API](https://img.shields.io/badge/Google_Generative_AI-4285F4?style=flat&logo=google&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-3F4C8C?style=flat&logo=grpc&logoColor=white)



## ▪ Dev Tools
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat&logo=visualstudiocode&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)



## 데이터 흐름도, 사용자 흐름도

## 📊 서비스 흐름도 (Mermaid)

```mermaid
flowchart TD
    %% 기본 흐름
    A1["사용자"] --> B1["메인 페이지"]
    B1 --> C1["건강 정보 입력하기"]
    C1 --> D1["입력 폼 (customer.html)"]
    D1 --> E1["customerDB에 저장"]
    E1 --> F1["메인 페이지로 리다이렉트 + 알림창"]
    F1 --> G["기능 선택"]

    %% 기능 버튼 가로 배치
    G --> G1["질병 예측"]
    G --> G2["병원 추천"]
    G --> G3["우울증 예측"]
    G --> G4["체형 분석"]
    G --> G5["운동 자세 교정"]

    %% 질병 예측 흐름
    G1 --> Note1["🧠 모델 예측"]
    Note1 -.-> G1A["4가지 그래프 출력"]
    G1A --> G1B["메인으로 돌아가기"]

    %% 병원 추천 흐름
    G2 --> Note2["🗺️ 지도 API 호출"]
    Note2 -.-> G2A["병원 위치 시각화"]
    G2A --> G2B["메인으로 돌아가기"]

    %% 우울증 예측 흐름
    G3 --> G3A["설문 입력 + 기존 DB"]
    G3A --> Note3["📊 설문 & DB 통합 처리"]
    Note3 -.-> G3B["우울 단계 예측"]
    G3B --> G3C["메인으로 돌아가기"]

    %% 체형 분석 흐름
    G4 --> Note4["📏 DB 기반 체형 분석"]
    Note4 -.-> G4A["체형 분석"]
    G4A --> G4B["맞춤 영상 추천"]
    G4B --> G4C["메인으로 돌아가기"]

    %% 운동 자세 교정 흐름
    G5 --> Note5["📹 실시간 캠 분석"]
    Note5 -.-> G5A["자세 분석 + 리포트"]
    G5A --> G5B["메인으로 돌아가기"]

    %% 회색 주석 스타일 정의
    classDef gray fill=#eee,color=#000,stroke=#999,stroke-width=1px,font-size:12px;
    class Note1,Note2,Note3,Note4,Note5 gray;
```
## 계층구조
## 기능 구현 움짤 (각자)
## how to test
