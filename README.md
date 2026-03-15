# AI Quant Research — Asia Equity Factor Analysis

## Overview
Python 및 AI 도구(Claude, Cursor)를 활용하여
아시아 주요 종목을 대상으로 팩터 기반 투자 전략을 분석한 프로젝트.

## Projects

### 01. Multi-Factor Screening
- 모멘텀(12개월 수익률) + PBR을 결합한 종목 선별 모델
- 단일 팩터 대비 Multi-factor 방식의 유효성 검증
- 사용 기술: Python, pandas, yfinance, matplotlib

### 02. Earnings Surprise Momentum
- 실적 발표 전후 주가 반응 및 PEAD 패턴 분석
- Day-1 기준점 설정을 통한 측정 방법론 개선
- 발표 후 20일간 종목별 모멘텀 지속성 비교
- 사용 기술: Python, pandas, yfinance, seaborn

## Key Findings
- 가격 기반 팩터(모멘텀+PBR) 최하위 종목(TSMC)이
  실적 발표 후 Day+20 기준 최고 수익률(+9.25%) 달성
- Earnings Surprise 팩터 추가의 필요성 확인
- 발표 당일 강한 반응이 반드시 지속적 상승을 보장하지 않음

## Tools & Skills
- Python (pandas, yfinance, matplotlib, seaborn, scipy)
- Cursor AI — 코드 생성 및 자동화
- Claude — 분석 설계 및 리서치 워크플로우 구축
- Jupyter Notebook
