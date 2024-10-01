# 🚦 Traffic Signal Controller Project

## 📌 프로젝트 개요
- **프로젝트명**: Traffic Signal Controller
- **주제**: 교통 신호 제어기 설계
- **설명**: 본 프로젝트는 수업시간에 배운 Verilog와 Bread Board를 이용하여 교차로의 교통 신호 제어기를 설계하고 구현한 과제입니다. 주요 도로(NS)와 보조 도로(EW) 간의 교차로에서 신호등이 정상적으로 작동하도록 상태 천이도, 진리표, Karnaugh Map을 활용하여 설계하였습니다.

## 🚦 교통 신호 제어기 설계
- **교차로 구성**: 남북(NS), 동서(EW) 방향의 교차로가 있는 교통 신호 제어기 디자인.
- **주도로 설정**: NS 도로가 교통 흐름이 많은 주도로 설정되어, EW 도로에 차량이 없을 시 항상 NS 도로에 녹색 신호를 유지.
- **신호 전환 조건**: EW 도로에 차량이 감지될 때 신호가 변경됨.
- **신호등 상태**: 녹색, 황색, 적색의 3가지 신호 상태를 제어.
- **신호 시간 설정**:
  - **NS 도로 신호 시간**: 녹색(6초) → 황색(2초) → 적색
  - **EW 도로 신호 시간**: 녹색(3초) → 황색(2초) → 적색
- **설계 방식**: **Moore** 또는 **Mealy** 상태 기계(State Machine) 설계를 활용하여 신호등을 제어.

## ✨ 주요 기능
1. **신호 제어 시스템 설계 및 구현**
   - 교차로의 주요 도로(NS)와 보조 도로(EW)에 대한 신호등 제어.
   - 특정 조건에 따라 NS 도로의 녹색 신호 유지, EW 도로의 교통량에 따른 신호 변경.

2. **상태 천이도(S.T.T) 설계**
   - Verilog를 이용하여 상태 천이도를 설계.
   - 주요 상태: 녹색(Green), 황색(Yellow), 적색(Red) 신호 제어.

3. **Mod-13 Counter 활용**
   - Verilog로 Mod-13 Counter를 설계하여 신호 주기를 제어.


## 🛠️ 기술 스택
언어: Verilog

설계 도구: LogicWorks

구현 환경: Bread Board, Verilog Simulation Tool

## 📂 폴더 구조 (Folder Structure)
```plaintext
Traffic_Signal_Controller/
├── Traffic_Signal_Controller.hwp           # 프로젝트 보고서 파일 (HWP)
├── Traffic_Signal_Controller.pdf           # 프로젝트 PDF 보고서
├── case1.tb.v                              # Test Bench for Case 1
├── case1.v                                  # Verilog Code for Case 1
├── case2.tb.v                              # Test Bench for Case 2
├── case2.v                                  # Verilog Code for Case 2
├── mod13.v                                  # Mod-13 Counter Design
├── 최종 회로.cct                           # 최종 회로 설계 파일
└── README.md                                # 프로젝트 설명 파일 (현재 파일)

