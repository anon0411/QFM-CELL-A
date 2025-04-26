
# 실험군 QFM-CELL-A: 기능적 세포 회로 실험
# Experiment Group QFM-CELL-A: Functional Cell Circuit Experiment

---

## 실험 목적
## Objective

이 실험은 양자 회로 내에서 구조가 단순히 반복되거나 유지되는 것을 넘어, **조건에 따라 스스로 변형하거나 다른 구조를 생성하는 기능성**을 가질 수 있는지를 탐색한다. 이를 통해 피드백 기반 회로가 구조적 '물질'을 넘어, 정보 기반의 '기능적 세포'로 해석될 수 있는지를 검토한다.

This experiment investigates whether quantum circuits with feedback structures can not only preserve but also transform themselves under specific conditions, thereby exhibiting behaviors analogous to functional cells rather than static materials.

---

## 실험 회로 설계
## Circuit Design

### 📐 실험 진행 단계
### Experimental Phases

1. **기본 구조 반복**  
   **Baseline Structure Repetition**  
   피드백 조건 없이 초기 회로를 반복 실행하여 안정된 출력 분포를 관찰함.  
   Repeatedly execute the initial circuit without branching to establish baseline structural stability.

2. **조건 분기 유도**  
   **Triggering Structural Divergence**  
   측정 결과가 '01' 또는 '10'일 경우, 회로가 변형된 피드백 구조로 전환되는지 관찰함.  
   Observe if outcomes '01' or '10' trigger transition to a different feedback path.

3. **분기 구조 반복 실행**  
   **Post-branch Feedback Repetition**  
   분기된 구조가 자기 유지 가능한지 확인하기 위해 연속 반복 수행.  
   Confirm whether the newly formed structure persists through repeated feedback.

4. **외부 자극 삽입 후 구조 반응**  
   **Response to External Stimulus**  
   RX(π) 삽입 후 구조가 원래 경로로 회복되는지 또는 새로운 상태로 분화되는지 평가.  
   Evaluate whether RX(π) causes structural recovery or leads to irreversible differentiation.


- **회로 구성**: 측정 결과에 따라 두 가지 상이한 피드백 회로 중 하나를 선택하여 다음 구조를 구성
  
  **Circuit Logic**: Based on the dominant measurement outcome, one of two distinct feedback subcircuits is selected to build the next structure

- **기본 회로**: H(0) → CX(0, 1) → RY(θ)

- **피드백 조건 분기**:
  - 결과가 '00' 또는 '11'인 경우: strong feedback → X-gate on all 1s
  - 결과가 '01' 또는 '10'인 경우: mutative feedback → RX(π/2) on even-indexed qubits

- **구조 변화 조건 삽입**: 외부 자극 RX(π)를 마지막 사이클에 삽입하여 다음 구조가 기존 구조에서 파생되는지를 측정

---

## 측정 방식
## Measurement Strategy

- 각 사이클에서 회로 결과의 변화 추적 (구조 유사도 + 분기 결정 로그)
- 구조 변화 여부 판단: 피드백 경로 변경 여부, 최종 회로 형상 비교

- Track similarity across cycles, and log whether structure transitions from one feedback logic to another occur.

---

## 기대되는 결과
## Expected Results

- 일부 사이클에서 피드백 분기 조건을 충족하면, 회로 구조가 다음 단계에서 **형태적으로 변화**할 것으로 기대됨
- 이러한 변화는 단순 반복을 넘어선 **자기 생성 또는 자기 전환**의 형태로 간주될 수 있음

---

## 분석 포인트
## Analysis Points

- 회로 구조의 변화 발생 시점과 조건 기록
- 구조 간 전환의 반복성 또는 비결정성 판단
- 외부 자극(RX(π)) 삽입 후 전환 구조가 **되돌림 가능한지(회복성)** 또는 **새로운 경로로 고정되는지(분화성)** 평가

---

## 실험 시각자료 및 로그
(추가 예정)

