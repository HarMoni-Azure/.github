# HARMoni  
## Azure Databricks 기반 실시간 IoT 웨어러블 산업 안전 분석 플랫폼

HARMoni는 Wear OS 기반 웨어러블 센서 데이터를 활용하여  
산업 현장의 낙상 사고를 실시간으로 감지·분석하는 Azure 기반 데이터 플랫폼 프로젝트입니다.

본 프로젝트는 단순 모델 성능 중심이 아닌,  
**실제 서비스 환경에서 발생하는 데이터·비용·운영 이슈를 고려한 아키텍처 설계**를 목표로 한다.

## Architecture Overview
- Wear OS (Sensor Data)
- Azure Functions (Event Ingestion)
- Azure Blob Storage (Raw Data)
- Azure Databricks & Delta Lake (Analytics / ML)
- Flutter / Dashboard (Visualization)

## Repositories
- [harmoni_function_app](https://github.com/HarMoni-Azure/harmoni_function_app/blob/main/README.md) : IoT 데이터 수집 (Azure Functions)
- [harmoni_ml](https://github.com/HarMoni-Azure/harmoni_ml) : Databricks 기반 데이터 처리 및 ML
- [harmoni_flutter_wearos](https://github.com/HarMoni-Azure/harmoni_flutter_wearos) : Wear OS 앱
- [HarMoni-swa](https://github.com/HarMoni-Azure/HarMoni-swa) : 대시보드(SWA)


<img width="1647" height="865" alt="이미지" src="https://github.com/user-attachments/assets/8adc926c-ec9c-4d5f-8ee0-938b15427ae9" />

👉 전체 아키텍처 및 설계 문서는 각 레포 README 참고

---

## 1. 프로젝트 배경

산업 현장(건설, 제조, 고위험 작업 환경)에서는 낙상 사고가 빈번하며,  
사고 발생 시 즉각적인 인지가 어려워 **대응 지연 → 중대 사고**로 이어질 가능성이 높다.

기존 CCTV 및 수동 보고 방식은 다음과 같은 한계를 가진다.

- 실시간 감지 및 즉각 알림의 한계
- 소규모 현장 적용 어려움
- 데이터 기반 사고 분석 부재

이에 따라 **웨어러블 IoT + 실시간 데이터 분석 플랫폼**의 필요성이 대두되었다.

---

## 2. 프로젝트 목표

- Wear OS 기반 웨어러블 센서 데이터 수집
- Azure 서버리스 기반 데이터 수집 파이프라인 구축
- Databricks + Delta Lake 기반 Medallion Architecture 구현
- Sliding Window 기반 Feature Engineering 및 ML 학습
- 비용 관리 관점에서 현실적인 실시간/배치 경계 설계
- Edge 환경을 고려한 TFLite 모델 변환 및 배포 구조 설계

---

## 3. 프로젝트 기간

- **2025.12.12 ~ 2025.12.23**

---

## 4. 팀 구성 및 역할

| 이름 | 역할 |
|---|---|
| 고승균 | **팀장 / 프로젝트 총괄, ML 모델 학습 및 평가** |
| 김소윤 | **Azure Cloud 환경 구축, 데이터 파이프라인 및 아키텍처 설계** |
| 남준혁 | **Wear OS 센서 데이터 수집 및 전처리** |
| 문연정 | **ML 모델 학습 및 고도화** |
| 윤정원 | **앱 및 대시보드 개발** |

---

## 5. 기술 스택

### Cloud & Data
- Azure Databricks
- Azure Blob Storage
- Azure Functions (HTTP Trigger)
- Delta Lake

### ML & MLOps
- Python
- TensorFlow / TensorFlow Lite
- MLflow

### Collaboration
- GitHub
- Microsoft Teams
- Miro

---

