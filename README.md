# AI Quant Research — Asia Equity Factor Analysis

## Overview
Python 및 AI 도구(Claude, Cursor)를 활용하여
아시아 주요 종목을 대상으로 팩터 기반 투자 전략을 분석한 프로젝트.

## Projects

### 01. Multi-Factor Screening
- 모멘텀(12개월 수익률) + PBR을 결합한 종목 선별 모델
- 단일 팩터 대비 Multi-factor 방식의 유효성 검증
- 사용 기술: Python, pandas, yfinance, matplotlib

### 02. Earnings Announcement — Stock Price Reaction Analysis
- 실적 발표 후 주가 반응 분석
- Day-1 기준점 설정을 통한 측정 방법론 개선
- 발표 후 20일간 종목별 주가 반응 지속성 비교
- 사용 기술: Python, pandas, yfinance, seaborn

### 03. Asia Momentum Strategy Backtest
- 한국(KOSPI)·일본(Nikkei)·홍콩(HSI) 45개 종목 대상
  12개월 누적 수익률 기반 월별 리밸런싱 전략 백테스트
- 매월말 12개월 누적 수익률 상위 10개 종목을 동일비중으로 편입 후 익월 리밸런싱 반복
- Look-ahead bias 방지를 위해 모멘텀 팩터값 1개월 시차 적용
- 거래비용 미반영으로 실제 수익률과 차이 존재
- yfinance 기반 분석으로 현재 상장된 종목만 포함, Survivorship Bias 가능성 있음.

## Key Findings
- 가격 기반 팩터(모멘텀+PBR) 최하위 종목(TSMC)이
  실적 발표 후 Day+20 기준 최고 수익률(+9.25%) 달성
- EPS 컨센서스 데이터 기반 Earnings Surprise 팩터 추가 필요성 확인
- 발표 당일 강한 반응이 반드시 지속적 상승을 보장하지 않음
- 아시아 3개 시장 45개 종목 대상 12개월 모멘텀 전략 백테스트
  (2018-2025 누적수익률 3.64x, Sharpe 0.996, MDD -20.34% 단, 거래비용 미반영)

## Tools & Skills
- Python (pandas, yfinance, matplotlib, seaborn, scipy)
- Cursor AI/Chat GPT — 코드 생성 및 교차검증
- Claude — 코드생성 및 분석 보조
- Jupyter Notebook
