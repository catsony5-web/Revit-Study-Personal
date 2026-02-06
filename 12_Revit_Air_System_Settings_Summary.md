# 12. 📊 Revit Energy Analysis Data Inventory Summary

이 문서는 `11_Revit_Air_System_Settings.md copy.md`의 방대한 항목을 **빠르게 파악하기 위한 요약본**입니다.

---

## 1) 문서 목적

- Revit 에너지 해석 결과에서 추출되는 **연간/월간 지표**의 의미를 빠르게 이해
- **IP → SI 단위** 변환 해석을 지원
- **LEED / G-SEED** 인증 활용 포인트를 한눈에 정리

---

## 2) 컬럼 읽는 법

- **대분류**: 결과가 속한 리포트 섹션
- **항목명 (Eng/Kor)**: 리포트에서 실제 표시되는 항목명
- **현재값 (IP)**: 미국식 단위 결과값
- **변환값 (SI 예측)**: 국내 보고서용 참고값
- **데이터 의미**: 해당 값이 의미하는 지표
- **LEED/G-SEED 활용**: 인증 평가에 쓰이는 범위

---

## 3) 핵심 섹션 요약

### ✅ Annual Overview / 연간 개요

- 연간 에너지 소비를 **유형별(난방/냉방/조명/팬/펌프 등)**로 집계
- 연간 총량 기준의 **에너지 성능 비교**에 사용
- LEED: EAp2, EAc1 주요 근거
- G-SEED: EPI 및 단위면적당 1차에너지 산정에 활용
- 예시 데이터:
  - Heating - Consumption (kBtu) / 난방 - 소비: 109,160 kBtu (SI 예측: 31,992 kWh)
  - Cooling - Consumption (kBtu) / 냉방 - 소비: 12,976 kBtu (SI 예측: 3,803 kWh)

### ✅ Monthly Overview / 월간 개요

- 월별 부하/소비 변화를 확인
- **냉난방 성능의 계절별 패턴** 분석에 적합
- 부하 저감 성능, 피크 추이 분석에 활용
- 예시 데이터:
  - Cooling - Jul / 냉방 - Jul: 448.3 (SI 예측: 448.3 kWh)
  - Fans - Aug / 송풍기 - Aug: 390.26 (SI 예측: 390.26 kWh)

### ✅ Detailed Report / 상세 리포트

- 시스템/장비 단위의 세부 항목 제공
- 설비 용량 산정, 운영 전략 검토에 유용
- 예시 데이터:
  - Total Site Energy - Total Energy [kBtu]: 131,804.73 kBtu (SI 예측: 38,628 kWh)
  - Total Source Energy - Total Energy [kBtu]: 227,055.89 kBtu (SI 예측: 66,543 kWh)

### ✅ Measure Warnings / 경고 항목

- 입력값 누락, 비현실적 설정 등 **주의 항목** 확인
- 리포트 해석 전 **우선 점검 리스트**로 활용
- 예시 데이터:
  - (예) Unmet Hours 경고
  - (예) 시스템 스케줄 미설정

---

## 4) 실무 활용 체크리스트

- **연간 개요**로 전체 에너지 성능을 빠르게 비교
- **월간 개요**로 계절별 과부하 원인 파악
- **Detailed Report**로 설비 용량 및 운전 전략 점검
- **Measure Warnings**에서 모델 품질 이슈를 선제 조치

---

원본 데이터 전체는 `11_Revit_Air_System_Settings.md copy.md`에서 확인하세요.
