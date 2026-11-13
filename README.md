# 2026 BAQU4 Autonomous Driving Team

> **Date:** 2026-10-30  
> **Competition:** 2026 대학생 AI·SW 모빌리티 경진대회 — 자작자율차 부문  
> **Award:** 특별상 (자작자율차 설계 부문)

[![BAQU4 Competition Video](https://img.youtube.com/vi/D8cXiHYWWPs/hqdefault.jpg)](https://www.youtube.com/watch?v=D8cXiHYWWPs&t=930s)

---

## 1. System Overview

BAQU4는 **하드웨어팀, 제어팀, 인지판단팀**으로 구성된 자작 자율주행 차량 개발팀입니다.

| Team | Responsibilities |
|---|---|
| **Hardware** | 차량 섀시 및 기구부 설계·제작, 하드웨어 시스템 구성 |
| **Vehicle Control** | 구동 모터, 조향 모터, 브레이크 및 ASMS 개발 |
| **Perception & Planning** | 센서 기반 환경 인식, 위치 추정, 주행 판단 및 상위제어 알고리즘 개발 |

각 시스템은 독립적으로 개발 및 검증되었으며, 최종적으로 차량 단위의 통합 자율주행 시스템으로 구성되었습니다.

**본 저장소는 제어팀과 인지판단팀의 소프트웨어 프로젝트 및 관련 개발 자료를 관리합니다.**

---

## 2. Project Repositories

### 2.1 Vehicle Control — 제어팀

차량의 종방향·횡방향 제어, 제동 시스템, 주행 모드 전환 및 안전 기능을 담당합니다.

| Module | Description | Repository |
|---|---|---|
| Motor Control | 종방향 구동 모터 제어 | [BAKU-Motor-Control](https://github.com/sjh0130s/BAKU-Motor-Control) |
| Steering Control | 횡방향 조향 모터 제어 | [f429zi_baqu](https://github.com/planta223/f429zi_baqu) |
| Brake Control | 제동 액추에이터 제어 | [bakunet](https://github.com/jeyun6267/bakunet) |
| ASMS | 주행 모드 전환 및 안전 관리 | [ASMS_Firmware](https://github.com/taeeunindaeyo/ASMS_Firmware) |

### 2.2 Perception & Planning — 인지판단팀

LiDAR, Camera, GPS 및 IMU 등의 센서 데이터를 기반으로 차량의 위치와 주변 환경을 인식하고, 주행 경로 및 차량 제어 명령을 생성합니다.

| Module | Description | Repository |
|---|---|---|
| Traffic Light Recognition | 교통 신호 인식 및 현시 정보 처리 | [traffic-light-recognition](https://github.com/JaeeunChong/traffic-light-recognition) |
| Brake Test | 라이다 기반 제동 검차 | [BAQU4-Brake-Test](https://github.com/joosung631-ops/BAQU4-Brake-Test/tree/main/stop_test) |
| Control Manager | 주행 판단 및 경로 추종 제어 | [control_manager](https://github.com/planta223/control_manager) |

---

## 3. Documentation & Resources

### 3.1 Competition Documents

대회 규정, 경기 진행 시나리오, 신호 현시 정보 및 K-City 지도 등 대회 운영과 관련된 공식 자료는 비공개로 관리합니다.

### 3.2 Driving Data

제동검차, 예선 및 본선 과정에서 수집한 주행 로그와 지도 데이터를 정리합니다.

**[Google Drive — BAQU4 Driving Data](https://drive.google.com/drive/folders/11jBqeTpvgn3spmiP_2gE9azIPyaHj95M?usp=sharing)**

| File / Directory | Description |
|---|---|
| `brake_log/` | 제동검차 주행 로그 |
| `preliminary_1030/` | 예선 주행 로그 (2026-10-30) |
| `final_1031/` | 본선 주행 로그 (2026-10-31) |
| `MAP_preliminary_v3.json` | 예선 주행 지도 데이터 |
| `MAP_final_v4.json` | 본선 주행 지도 데이터 |

> All driving logs and map files are available through the Google Drive link above.

---

## 4. License

This repository is licensed under the [MIT License](LICENSE).

This license applies only to original materials contained in this repository.

Each linked project repository maintains its own license and copyright.

Competition regulations, official documents, and third-party materials are not covered by this license.
