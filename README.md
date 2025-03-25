# 📦 WMS (Warehouse Management System)

[](https://capsule-render.vercel.app/api?type=rect&color=gradient&text=WMS%20System&fontColor=ffffff&height=300&fontSize=50)

<br>

## 📚 목차

1. [📌 프로젝트 소개]
2. [⏰ 개발 기간]
3. [⚙ 프로젝트 내 역할 및 기여]
4. [👥 팀원 및 역할 분담]
5. [🧱 클래스 다이어그램 / ERD]
6. [🛠 기술 스택]
7. [🎬 시연 영상]
8. [🚧 기술적 이슈 및 해결 과정]
9. [💬 느낀 점]

<br>

## 📌 프로젝트 소개

- *화주(Client)**와 **관리자(Admin)**의 역할을 분리하여 동작하는 **창고 관리 시스템(WMS)**을 개발함
- **1차 프로젝트**에서는 아래와 같은 기능을 중심으로, **WMS의 기본 구조와 동작 원리**를 이해하고 직접 구현함
    - 제품 입고/출고 처리 기능
    - 재고 수량 관리 및 변경 이력 기록 기능
    - 식재료 보관 조건에 따라 자동으로 구역을 배정하는 기능
    - 관리자가 구역별 온도를 직접 설정·제어할 수 있는 기능
- 이를 통해 **입출고 흐름**, **자동화된 구역 배정 및 재고 관리**, **사용자 역할 기반의 기능 분리** 등
    
    **WMS 시스템이 어떻게 구성되고 동작해야 하는지에 대한 전반적인 구조를 이해함**
    
- 이후 **2차 프로젝트에서는 기능을 확장하고, 구조를 고도화**하는 것을 목표로 함

<br>

## ⏰ 개발 기간

| 단계 | 기간 | 내용 |
| --- | --- | --- |
| 설계 및 ERD | 2025.03.11 ~ 2025.03.14 | 테이블 설계, ERD 작성 |
| 기능 개발 | 2025.03.17 ~ 2025.03.21 | 입고, 출고, 회원 관리 등 |
| 리팩토링 | 2025.03.24 ~ 2025.03.28 | 예외 처리, 구조 개선 등 |

<br>

## ⚙ 프로젝트 내 역할 및 기여

### ✅ 보관 조건 기반 자동화 로직 설계

- **입고 요청이 들어오면, 해당 식재료의 보관 조건과 공간 크기를 고려해서 자동으로 구역을 배정하도록 만듦**
→ 사람이 직접 고르지 않아도, 시스템이 자동으로 적절한 위치를 찾아 배치하게 함

<br>

### ✅ 재고 및 재고 이력 관리 자동화

- **입고/출고가 일어날 때마다 자동으로 재고 수량이 바뀌고, 그 기록이 남도록 트리거를 사용해서 구현함**
    
    → 재고 수량이 실시간으로 반영되고, 변경 이력도 따로 관리되도록 처리함
    
- **입출고 내역을 콘솔에서 실시간으로 조회할 수 있게 만듦**
    
    → 어떤 요청이 언제, 어떤 상태로 처리됐는지 (승인/대기/취소) 바로 확인할 수 있도록 함
    

<br>

### ✅ Git 브랜치 전략 적용 및 관리

- **Git Flow 전략을 기반으로 `main`, `develop`, `feature`, `hotfix` 브랜치를 나누고, 협업 시 충돌 없이 개발할 수 있도록 전략을 세우고 운영함**
- **팀원들이 작업한 코드를 통합하고 관리할 때 효율적으로 병합되도록 브랜치 전략을 적용해서 협업 안정성을 높였음**

<br>

## 👥 팀원 및 역할 분담

| 이름 | 역할 |
| --- | --- |
| 김병곤 | 입고, 재고 깃 관리 |
| 정난희 | 로그인, 회원관리 |
| 정태연 | 출고, 재고 관리 |
| 이정섭 | 창고, 구역 관리 |

<br>

## 🧱 클래스 다이어그램 / ERD

## 📘 클래스 다이어그램

![스크린샷 2025-03-25 162733](https://github.com/user-attachments/assets/171ac64c-85a9-4368-a596-6fc4f50cd2f3)

![스크린샷 2025-03-25 170737](https://github.com/user-attachments/assets/24042629-5326-419c-a7a6-016419de9d47)

![스크린샷 2025-03-25 170758](https://github.com/user-attachments/assets/78539d5b-bdf4-4bee-b46f-0fd9aea93525)




## 🗃️ DB ERD

![스크린샷 2025-03-25 162531](https://github.com/user-attachments/assets/4e653e9a-0acb-4284-a912-2b44fee1e3fe)


<br>

## 🛠 기술 스택

| 구분 | 사용 기술 |
| --- | --- |
| Language | Java (JDK 17) |
| DB | MySQL |
| Tool | IntelliJ IDEA, GitHub |
| 개발 방식 | 순수 Java + JDBC 연동 (No Spring) |

<br>

## 🎬 시연 영상

> 📽 영상 링크: (YouTube 또는 GitHub 링크 첨부)
> 

<br>

## 🚧 기술적 이슈 및 해결 과정

> 벨로그 등 외부 문서 링크 또는 주요 이슈 요약 작성
> 

<br>

## 💬 느낀 점

이번 프로젝트를 통해 단순한 기능 구현을 넘어서, **팀원 간 협업의 중요성**, **역할 기반 시스템 설계**, 그리고 **객체지향 프로그래밍(OOP)의 필요성**을 체감함.

특히 입고/출고와 같은 실제 창고 프로세스를 직접 설계하고 자동화 로직을 구현하면서,

**실제 서비스에서 효율성과 실시간성이 왜 중요한지**, 그리고 이를 **코드와 DB 구조로 어떻게 구현할 수 있는지**에 대해 깊이 고민할 수 있었음.

또한 Git 브랜치 전략을 적용하며 **효율적인 협업 방식**을 경험했고,

**역할 분담을 통한 모듈화와 책임 분리의 중요성**도 함께 배울 수 있었음.

이번 경험을 바탕으로, 이후 프로젝트에서는 **더 확장된 기능과 구조**,

그리고 **유지보수가 용이한 아키텍처 설계**를 목표로 계속 성장해 나갈 계획임.
