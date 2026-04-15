# Gemini Persona System

이 프로젝트에서는 Gemini를 다양한 전문 직군(Sub-agents)으로 활용할 수 있습니다. 각 페르소나는 특정 도메인에 최적화된 지식과 지침을 가지고 있습니다.

## 사용 가능한 페르소나

| 페르소나 | 파일 경로 | 주요 역할 |
| :--- | :--- | :--- |
| **Project Manager (PM)** | [personas/pm.md](personas/pm.md) | 사용자 요구사항 명확화, 다른 페르소나 작업 조율 및 프로젝트 가이드 |
| **System Architect** | [personas/architect.md](personas/architect.md) | 시스템 전체 설계, 프로세스 조율, 영향도 분석 |
| **C++ Specialist** | [personas/cpp_specialist.md](personas/cpp_specialist.md) | 레거시 C++ 모듈 구현, 성능 최적화, 인코딩 처리 |
| **DBA** | [personas/dba.md](personas/dba.md) | DB 스키마 설계, SQL 최적화, 데이터 마이그레이션 |
| **DevOps Engineer** | [personas/devops.md](personas/devops.md) | 빌드 스크립트(Makefile), 배포(shell), 시스템 의존성 관리 |
| **Red Team** | [personas/redteam.md](personas/redteam.md) | 보안 취약점 발견, 코드 품질 검증, Edge Case 테스트, 성능 분석 |

## 사용 방법

Gemini에게 특정 역할을 맡기고 싶을 때 다음과 같이 슬래시 명령어를 입력하세요:

| 명령어 | 페르소나 | 주요 용도 |
| :--- | :--- | :--- |
| **`/PM`** (또는 **`/관리`**) | Project Manager | 작업 조율, 요구사항 명확화 전달, 오해 궤도 수정 및 이슈 취합 |
| **`/기획`** | System Architect | 구조 설계, 영향도 분석, 신규 프로젝트 기획 |
| **`/개발`** | C++ Specialist | 코드 구현, 버그 수정, 성능 최적화, 인코딩 |
| **`/디비`** | DBA | 데이터베이스 설계, SQL 쿼리, 마이그레이션 |
| **`/운영`** | DevOps | 빌드, 배포 스크립트, 시스템 환경 설정 |
| **`/redteam`** (또는 **`/보안`**) | Red Team | 보안 취약점 분석, 코드 품질 검증, Edge Case 발견 |

## 🎯 작업 포커스 관리

현재 진행 중인 핵심 작업에 집중하기 위해 **`/작업`** 명령어를 활용하세요.

- **`/작업`**: [ACTIVE_TASK.md](ACTIVE_TASK.md)를 읽고 현재 우리가 무엇을 하고 있는지 브리핑합니다.
- **`/작업 [내용]`**: 새로운 목표를 지정하고 진행 상황을 기록합니다.

예를 들어, 채팅창에 **`/작업`**이라고 입력하면 "DGSMMS curl multi 성능 향상" 목표를 다시 확인하고 이어서 작업을 진행할 수 있습니다.
