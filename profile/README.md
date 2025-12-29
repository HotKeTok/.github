# 🚀 핫케톡: Housing Care Total Service
**[🏆 제 9회 개방형 클라우드 플랫폼(K-PaaS)활용 공모전 서비스 개발 부문 동상(숭실대총장상) 수상작]**

**Target: Digitizing Multi-Family Housing Management. (다가구 주택 관리 디지털화)**

Hotketok은 법적 규제 사각지대에 놓여있던 다가구 주택 관리를 **데이터 기반의 투명하고 체계적인 디지털 관리 시스템**으로 전환하는 플랫폼입니다. 입주민, 집주인, 수리업체 세 주체를 하나로 통합된 효율적인 워크플로우로 연결합니다.

---

## ⚡️ Core Innovation: The Digital Triple Threat

핫케톡은 비(非)아파트 주거 관리에서 발생하는 불투명성, 파편화, 복잡성이라는 세 가지 핵심 문제를 해결합니다.

| Domain | Problem Defined (문제 정의) | Hotketok Solution (핫케톡 솔루션) | Impact (효과) |
| :--- | :--- | :--- | :--- |
| **Finance** | **'깜깜이 관리비'** 문제: 관리 항목 불분명 및 명세서 미제공으로 불신 발생. | **Digital Ledger:** 공과금 자동 수집/분류 및 월별 증감 추이 시각화 제공. 비공식 계좌 관리를 디지털 회계 시스템으로 전환. | **Full Transparency (투명성 확보)**. |
| **Community** | **소통 파편화**: 공식 채널 부재로 층간소음 등 민원이 비공식적 방식으로 진행되어 감정적 대립 심화. | **'Ttokttok' (Smart Connect):** 집주인 공지사항 게시 및 입주민 간 **태그 기반(#층간소음)** 익명 쪽지 소통 채널 제공. | **Structured Communication (체계적 소통)**. |
| **Maintenance** | **복잡한 수리 절차**: '입주민 → 집주인 → 수리업체'의 다단계 구조로 연락 지연 및 비효율성 초래. | **'Ttukttak' (Quick Fix):** **AI 이미지 분석**으로 상세 수리 요청서를 자동 작성하고, 요청부터 완료까지 **4단계 상태를 시각화**하여 절차를 자동화합니다. | **Operational Efficiency (운영 효율성)**. |

---

## 🔑 핵심 기능 하이라이트 (Key Features Highlight)

### 1. 💰 공과금/공동관리비 내역 확인
* **투명한 재정 관리:** 공과금 및 공동관리비 데이터를 자동 수집, 분류하고 월별 납부 내역과 증감 추세를 **그래프와 차트로 시각화**하여 실시간 공유합니다.
* **집주인 관리 기능:** 집주인은 입금·출금 내역을 일자별 회계 리포트로 관리하고, 항목을 직접 추가/수정하여 디지털 회계 시스템을 구축합니다.

### 2. 🗣️ 똑똑: 입주민 간 소통 및 공지
* **공식 공지 채널:** 집주인은 공지사항(건물 점검 일정, 주차 안내 등)을 게시형 공지 기능으로 전달하고 기록할 수 있습니다.
* **익명 기반 상호 소통:** 입주민 간 **태그 기반 쪽지 기능**을 통해 상호 존중과 신뢰를 바탕으로 한 커뮤니티 환경을 조성합니다.

### 3. 🛠️ 뚝딱: 수리 관리 프로세스 자동화
* **AI 요청서 작성:** 수리 증상 사진을 업로드하면 **AI 이미지 인식을 통해 수리요청서 상세 기술서가 자동 작성**되어 요청의 정확도를 높입니다.
* **간편한 견적/승인:** 집주인은 다수의 견적 중에서 합리적인 견적을 비교·선택하여 수리 진행을 확정합니다.
* **실시간 진행 상황:** 수리 과정은 **'업체 찾는 중 → 견적서 선택 → 업체 매칭 → 처리 완료'의 네 단계로 시각화**되어 입주민과 집주인 모두 실시간 확인이 가능합니다.

---

## 🛠️ Tech Stack & K-PaaS Architecture

핫케톡은 네이버 클라우드 플랫폼(NCP)의 **K-PaaS** 환경을 적극 활용하여 유연성, 가용성, 안정성을 갖춘 클라우드 네이티브 아키텍처를 구축했습니다.

### Architecture Overview
<img width="799" height="443" alt="스크린샷 2025-11-04 오후 8 07 40" src="https://github.com/user-attachments/assets/9b6e2ca9-3101-43a3-89c6-fe8e08f5c2c3" />

*Hotketok은 **MSA(Microservice Architecture)** 기반으로 설계되었으며, **NKS (Ncloud Kubernetes Service)** 클러스터 환경에서 컨테이너화된 마이크로서비스를 운영합니다.*

### MSA & Development Efficiency
1.  **MSA Decoupling (MSA 분리):** 높은 시스템 결합도 문제를 해결하기 위해, DDD 기반으로 11개 핵심 비즈니스 기능을 마이크로서비스로 분리했습니다. 이를 통해 **서비스 단위 독립 배포** 및 유연한 확장이 가능해졌습니다.</br>
     <img width="801" height="449" alt="스크린샷 2025-11-04 오후 8 08 41" src="https://github.com/user-attachments/assets/16e31895-cbc1-48e6-a951-ef8ff0dc7b3a" />

2.  **Fully Automated CI/CD (완전 자동화 CI/CD):** NCP의 PaaS 서비스인 **SourcePipeline**을 중심으로 전체 개발 라이프사이클을 자동화했습니다. </br>
    <img width="798" height="449" alt="스크린샷 2025-11-04 오후 8 08 19" src="https://github.com/user-attachments/assets/33c56445-f6c0-4e99-88d9-53ab9839cdc7" />

3.  **Zero-Downtime Deployment (무중단 배포):** `SourceDeploy`의 Rolling Update 전략을 적용하여 개발자가 코드만 커밋하면 무중단 배포 방식으로 NKS 클러스터에 서비스가 자동 반영됩니다.

### Platform Breakdown (플랫폼 구성)

| Component | Backend (BE) | Frontend (FE) | Deployment & Infra (배포 및 인프라) |
| :--- | :--- | :--- | :--- |
| **Technology** | Java, Spring Boot, MySQL, Redis | React JS, JavaScript | NKS, SourcePipeline, Nginx Ingress Controller |
| **User Access** | - | - | 입주민/집주인: 모바일 앱 (App), 수리업체: 웹 포털 (Web) |

---

## 🌐 Vision & Strategic Impact

핫케톡은 주거 관리의 질을 향상시키고, 공공 정책 영역과 연계하여 사회적 가치를 창출합니다.

* **Standardization of Management (관리 표준화):** 비공식 관리 체계를 데이터 기반 표준 프로세스로 전환하여, **공공 관리 체계 편입 기반**을 마련합니다.
* **Data Assetization (데이터 자산화):** 축적된 관리 기록은 행정기관의 주거복지 사각지대 모니터링 및 **정책 의사결정 지원 데이터셋**으로 활용될 수 있습니다.
* **Scalability (확장성):** K-PaaS의 멀티테넌시 구조를 활용하여 **지자체 단위의 로컬 주거관리 SaaS 모델**로 확산 가능하며, 공공 협력형 주거복지 플랫폼 생태계로 발전할 수 있습니다.
* **Market Alignment (시장 연계):** 다가구 매입임대 출자 예산 확대 등 정부 정책 흐름에 따라 **민간형 '다가구 관리 SaaS 플랫폼'**의 핵심 축으로 기능할 것으로 기대됩니다.

---

## 👥 The Team

|  |  |  |  |  |
|:--:|:--:|:--:|:--:|:--:|
| **@sunwoo-h** | **@yminjuu** | **@alswjdghks** | **@shinminkyoung1** | **박지효** |
| FE | FE | BE | BE | DE
