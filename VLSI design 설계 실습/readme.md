# AIoT 반도체 설계 과정 - VLSI Design 설계 실습 과목 개요

**VLSI Design 설계 실습** 과목은 반도체 집적회로 설계의 전 과정을 실습 중심으로 학습하는 고급 설계 과목입니다. Verilog HDL을 이용한 회로 설계부터, 시뮬레이션, 물리적 레이아웃 작성, 배치/배선, DRC/LVS 검증까지 전체 VLSI 설계 플로우를 수행합니다.

## 주요 교육 내용

| 교육 영역              | 세부 내용 |
|----------------------|----------|
| **디지털 시스템 설계 기초** | 조합 회로, 순차 회로, FSM 설계 및 최적화 |
| **Verilog HDL 활용**   | RTL 설계, 모듈 계층화, 파이프라이닝, 파라미터화 설계 |
| **논리합성(Synthesis)** | RTL → Gate-level 변환, Synopsys Design Compiler 실습 |
| **배치 및 배선(PnR)**   | 셀 배치, 시계망 삽입, 라우팅 (Cadence Innovus 또는 OpenROAD) |
| **물리 설계(Layout)**   | GDSII 생성, 레이아웃 에디터를 이용한 수동/자동 배치 |
| **검증(DRC/LVS)**     | Design Rule Check, Layout vs Schematic 검증 |
| **타이밍 분석**         | STA(Static Timing Analysis), 타이밍 여유 분석 |
| **파워 분석 및 최적화** | 소비 전력 예측, 저전력 설계 기법 적용 (클럭 게이팅 등) |
| **FPGA 비교 실습**     | RTL을 FPGA와 ASIC 양쪽에 구현해보고 차이 비교 분석 |
| **최종 Tape-out 프로젝트** | SoC 또는 서브 블록을 완성하여 GDSII 파일로 Tape-out 시뮬레이션 |

## 교육 목표

- **VLSI 설계 플로우 전반에 대한 실습 역량 강화**
- **EDA 툴을 활용한 반도체 설계, 검증, 레이아웃 능력 습득**
- **산업 현장의 반도체 설계 엔지니어 실무에 대한 적응력 배양**

## 수업 특징

- RTL 설계 → Gate-level → Layout → GDSII 생성까지 전 과정 수행
- 실습 중심의 프로젝트 기반 학습(PBL)
- 타 과목(SoC 설계, ARM 실무, EDA 실습 등)과 연계한 종합 설계 수행

## 활용 툴 및 환경

- **EDA 툴**: Cadence (Virtuoso, Innovus), Synopsys (Design Compiler, IC Compiler), Mentor Graphics
- **설계 언어**: Verilog HDL, SystemVerilog
- **검증 툴**: ModelSim, Calibre (DRC/LVS)
- **오픈소스 옵션**: OpenROAD, Magic VLSI, KLayout


