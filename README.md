# 🤖 Agentic Economy - AI 경제 에이전트 시스템

**2026년 미래 경제를 분석하는 5개의 AI 에이전트 기반 경제 분석 플랫폼**

> 암호화폐, 주식, 주요 인물, 시장 동향을 자동으로 모니터링하고 예측하는 에이전트 시스템

---

## 📋 개요

**Agentic Economy**는 AI 에이전트를 활용한 혁신적인 경제 분석 시스템입니다. 
5개의 독립적인 에이전트가 협력하여 **실시간 시장 데이터 수집, 분석, 예측**을 자동화합니다.

### 🎯 핵심 목표
- ✅ 암호화폐 시장의 실시간 동향 파악
- ✅ 전통 주식 시장의 트렌드 분석
- ✅ 경제에 영향력 있는 주요 인물 모니터링
- ✅ 주식 시장 동향 기반 가격 예측
- ✅ 암호화폐 시장 동향 기반 가격 예측

---

## 🤖 5가지 핵심 에이전트

### 1️⃣ 암호화폐 동향 에이전트 (Crypto Trend Agent)
**실시간 암호화폐 시장 모니터링**

| 항목 | 설명 |
|------|------|
| 주요 기능 | BTC, ETH, Top 100 코인 시세, 거래량, 센티먼트 |
| API | CoinGecko, CoinMarketCap, CryptoPanic |
| 업데이트 | 1시간 또는 실시간 |
| 주요 지표 | 가격, 시가총액, 거래량, 24h 변동률 |

📊 **모니터링 지표**
- 가격 변동률 (1h, 24h, 7d, 30d)
- 시가총액 및 순위 변화
- 거래량 이상치 탐지
- 센티먼트 점수 (긍정/부정)
- 섹터별 분석 (DeFi, Layer2, AI 등)

---

### 2️⃣ 주식 시장 동향 에이전트 (Stock Market Trend Agent)
**전통 주식 시장의 포괄적 분석**

| 항목 | 설명 |
|------|------|
| 주요 기능 | S&P 500, NASDAQ, 개별 종목, 섹터 분석 |
| API | yfinance, Alpha Vantage, Polygon.io |
| 업데이트 | 장 중 실시간, 장 후 일일 정리 |
| 커버리지 | US Stock Market (NYSE, NASDAQ) |

📈 **분석 항목**
- 지수별 성과 (S&P 500, NASDAQ, Dow Jones)
- 기술적 지표 (MA, RSI, MACD, Bollinger Bands)
- 펀더멘탈 분석 (P/E, ROE, 배당 수익률)
- 거시 경제 지표 (금리, 실업률, GDP)
- 섹터 로테이션 분석
- VIX 공포 지수 모니터링

---

### 3️⃣ 주요 인물 팔로잉 에이전트 (Influencer Monitoring Agent)
**경제에 영향력 있는 주요 인물 모니터링**

| 항목 | 설명 |
|------|------|
| 주요 대상 | Elon Musk, Donald Trump, 기업 CEO, 경제 전문가 |
| API | Tavily Search, NewsAPI, X API (향후) |
| 업데이트 | 실시간 또는 1시간마다 |
| 형식 | X 포스트, 언론 인터뷰, 성명서 |

🎯 **팔로잉 대상 (Tier별)**
- **Tier 1**: Elon Musk, Donald Trump (최우선)
- **Tier 2**: Tech CEO (Apple, Microsoft, Google, Meta)
- **Tier 3**: 암호화폐 인물 (Vitalik Buterin, CZ 등)
- **Tier 4**: 경제 전문가 (Buffett, Dalio, Krugman)

---

### 4️⃣ 주식 시장 예측 에이전트 (Stock Prediction Agent)
**ML/DL 기반 주가 예측**

| 항목 | 설명 |
|------|------|
| 주요 기능 | 1일/1주/1개월 주가 예측 및 신호 생성 |
| 모델 | ARIMA, XGBoost, LightGBM, LSTM |
| 정확도 목표 | 60%+ (단기), 55%+ (중기) |
| 예측 대상 | S&P 500 지수, Top 100 개별 종목 |

🎲 **예측 모델**
- **ARIMA/Prophet**: 단기 트렌드 (1~5일)
- **XGBoost/LightGBM**: 중기 예측 (1~4주)
- **LSTM**: 장기 추세 (1개월+)
- **Ensemble**: 여러 모델의 투표 결합

---

### 5️⃣ 암호화폐 시장 예측 에이전트 (Crypto Prediction Agent)
**암호화폐 가격 예측 및 추세 분석**

| 항목 | 설명 |
|------|------|
| 주요 기능 | 4h/1d/1w/1m 암호화폐 가격 예측 |
| 모델 | Prophet, XGBoost, LSTM 앙상블 |
| 정확도 목표 | 65%+ (단기), 60%+ (중기) |
| 예측 대상 | BTC, ETH, Top 20 코인 |

🚀 **예측 특징**
- 4시간 단위 초단기 예측
- 1일 중기 예측
- 온체인 메트릭 분석
- 시장 감정 (Fear & Greed Index) 반영
- 거래 신호 및 위험도 평가

---

## 🛠️ 기술 스택

### API 서비스
```
암호화폐:
├── CoinGecko (월 10,000 크레딧)
├── CoinMarketCap (월 10,000 크레딧)
└── CryptoPanic (일 100회)

주식/경제:
├── yfinance (완전 무료)
├── Alpha Vantage (일 25회)
└── Polygon.io (실시간 - 유료)

뉴스/검색:
├── Tavily Search (월 1,000회)
└── NewsAPI (일 100회)

소셜:
└── X API (유료 - $200/월)
```

### 프로그래밍
```
Python 3.10+
├── pandas, numpy (데이터 처리)
├── scikit-learn, xgboost (머신러닝)
├── tensorflow/pytorch (딥러닝)
├── statsmodels, prophet (시계열 분석)
└── plotly, matplotlib (시각화)
```

### 데이터베이스 & 저장소
```
Primary:
├── PostgreSQL (시계열 데이터)
├── Redis (캐시)
└── Elasticsearch (전문 검색 - 향후)

Secondary:
└── CSV/Parquet (초기 단계)
```

---

## 💰 API 요금제

### Phase 1: 무료 플랜 (초기)
| 서비스 | 월 비용 | 제한사항 |
|--------|--------|---------|
| **합계** | **$0/월** | 모든 무료 플랜 사용 |

**포함 내용**
- ✅ CoinGecko: 월 10,000 크레딧
- ✅ CoinMarketCap: 월 10,000 크레딧
- ✅ CryptoPanic: 일 100회
- ✅ yfinance: 무제한
- ✅ Alpha Vantage: 일 25회
- ✅ Tavily Search: 월 1,000회
- ✅ NewsAPI: 일 100회

### Phase 2: 라이트 유료 (선택)
| 서비스 | 월 비용 |
|--------|--------|
| CoinGecko | $35/월 |
| Tavily Search | $30/월 |
| **합계** | **$65/월** |

### Phase 3: 풀 스택 유료 (스케일)
| 서비스 | 월 비용 |
|--------|--------|
| CoinGecko | $35 |
| CoinMarketCap | $29 |
| CryptoPanic | $29 |
| Alpha Vantage | $50 |
| Polygon.io | $29 |
| Tavily Search | $30 |
| NewsAPI | $40 |
| X API | $200 |
| **합계** | **$442/월** |

> 📌 더 자세한 내용은 [요금제 정리.md](요금제%20정리.md) 참고

---

## 📁 프로젝트 구조

```
agentic-economy/
├── README.md                          # 프로젝트 개요
├── 요금제 정리.md                      # API 요금제 정리
├── .github/
│   └── agents/
│       ├── 01_암호화폐동향에이전트.md      # Crypto Trend Agent
│       ├── 02_주식시장동향에이전트.md      # Stock Market Trend Agent
│       ├── 03_주요인물팔로잉에이전트.md    # Influencer Monitoring Agent
│       ├── 04_주식시장예측에이전트.md      # Stock Prediction Agent
│       └── 05_암호화폐시장예측에이전트.md  # Crypto Prediction Agent
│
├── agents/                            # 에이전트 코드
│   ├── __init__.py
│   ├── crypto_trend/                  # 암호화폐 동향 에이전트
│   ├── stock_market/                  # 주식 시장 동향 에이전트
│   ├── influencer_monitor/            # 주요 인물 팔로잉 에이전트
│   ├── stock_prediction/              # 주식 시장 예측 에이전트
│   └── crypto_prediction/             # 암호화폐 시장 예측 에이전트
│
├── data/                              # 데이터 저장소
│   ├── raw/                           # 원본 데이터
│   ├── processed/                     # 처리된 데이터
│   └── models/                        # 학습된 모델
│
├── config/                            # 설정 파일
│   ├── .env.example
│   ├── config.yaml
│   └── credentials.json
│
├── docs/                              # 문서
│   ├── development.md                 # 개발 가이드
│   ├── api-setup.md                   # API 설정
│   ├── database.md                    # 데이터베이스 구성
│   └── deployment.md                  # 배포 가이드
│
├── tests/                             # 테스트
│   ├── unit/
│   ├── integration/
│   └── fixtures/
│
├── requirements.txt                   # Python 패키지
├── Dockerfile                         # Docker 컨테이너
├── docker-compose.yml                 # Docker Compose
└── .gitignore
```

---

## 🚀 빠른 시작

### 사전 요구사항
- Python 3.10+
- PostgreSQL 13+
- Redis 6+
- pip (또는 conda)

### 1단계: 저장소 클론
```bash
git clone https://github.com/LimChanju/agentic-economy.git
cd agentic-economy
```

### 2단계: 가상 환경 설정
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
# 또는
venv\Scripts\activate  # Windows
```

### 3단계: 패키지 설치
```bash
pip install -r requirements.txt
```

### 4단계: 환경 변수 설정
```bash
cp config/.env.example config/.env
# .env 파일에 API 키 입력
```

### 5단계: 데이터베이스 초기화
```bash
python setup_db.py
```

### 6단계: 에이전트 실행
```bash
# 모든 에이전트 시작
python main.py

# 또는 개별 에이전트 실행
python agents/crypto_trend/agent.py
python agents/stock_market/agent.py
python agents/influencer_monitor/agent.py
python agents/stock_prediction/agent.py
python agents/crypto_prediction/agent.py
```

---

## 📊 에이전트별 사용 현황

### 활성 에이전트
```
✅ 암호화폐 동향 에이전트  - 데이터 수집 중
✅ 주식 시장 동향 에이전트 - 데이터 수집 중
✅ 주요 인물 팔로잉 에이전트 - 모니터링 중
🔄 주식 시장 예측 에이전트 - 개발 중
🔄 암호화폐 시장 예측 에이전트 - 개발 중
```

---

## 🔧 API 설정

### 필수 API 키
```
CoinGecko:      https://www.coingecko.com/en/api
CoinMarketCap:  https://coinmarketcap.com/api/
CryptoPanic:    https://cryptopanic.com/api
Alpha Vantage:  https://www.alphavantage.co/
Tavily Search:  https://tavily.com/
NewsAPI:        https://newsapi.org/
```

### .env 파일 예시
```env
# Crypto APIs
COINGECKO_API_KEY=your_coingecko_key
COINMARKETCAP_API_KEY=your_coinmarketcap_key
CRYPTOPANIC_API_KEY=your_cryptopanic_key

# Stock APIs
ALPHA_VANTAGE_API_KEY=your_alpha_vantage_key
POLYGON_API_KEY=your_polygon_key

# Search & News
TAVILY_API_KEY=your_tavily_key
NEWSAPI_API_KEY=your_newsapi_key

# Database
DATABASE_URL=postgresql://user:password@localhost:5432/agentic_economy
REDIS_URL=redis://localhost:6379/0

# X API (향후)
X_API_KEY=your_x_api_key
```

---

## 📈 성능 지표

### 목표 정확도
```
암호화폐 동향:     실시간 모니터링 (정확도 100%)
주식 시장 동향:    실시간 모니터링 (정확도 100%)
주요 인물 팔로잉:  실시간 감지 (응답 시간 < 5분)
주식 시장 예측:    60%+ 정확도 (단기)
암호화폐 예측:     65%+ 정확도 (단기)
```

---

## 📚 상세 문서

각 에이전트에 대한 상세한 설명은 아래를 참고하세요:

- 📌 [암호화폐 동향 에이전트](.github/agents/01_암호화폐동향에이전트.md)
- 📌 [주식 시장 동향 에이전트](.github/agents/02_주식시장동향에이전트.md)
- 📌 [주요 인물 팔로잉 에이전트](.github/agents/03_주요인물팔로잉에이전트.md)
- 📌 [주식 시장 예측 에이전트](.github/agents/04_주식시장예측에이전트.md)
- 📌 [암호화폐 시장 예측 에이전트](.github/agents/05_암호화폐시장예측에이전트.md)
- 💰 [API 요금제 정리](요금제%20정리.md)

---

## 🤝 기여 가이드

이 프로젝트에 기여하려면:

1. 저장소를 포크합니다
2. 기능 브랜치를 생성합니다 (`git checkout -b feature/amazing-feature`)
3. 변경사항을 커밋합니다 (`git commit -m 'Add amazing feature'`)
4. 브랜치에 푸시합니다 (`git push origin feature/amazing-feature`)
5. Pull Request를 생성합니다

---

## 📝 라이선스

이 프로젝트는 MIT 라이선스를 따릅니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참고하세요.

---

## 📞 지원

- 📧 이슈 제출: [GitHub Issues](https://github.com/LimChanju/agentic-economy/issues)
- 💬 토론: [GitHub Discussions](https://github.com/LimChanju/agentic-economy/discussions)
- 📌 프로젝트 보드: [GitHub Projects](https://github.com/LimChanju/agentic-economy/projects)

---

## 🔮 향후 계획 (Roadmap)

### Q1 2026
- ✅ 기본 에이전트 구조 설계
- ✅ API 통합 가이드 작성
- 🔄 초기 데이터 수집 시스템 구축

### Q2 2026
- 🔄 머신러닝 모델 개발
- 🔄 백테스트 시스템 구현
- 🔄 웹 대시보드 개발

### Q3 2026
- 🔄 실시간 예측 시스템 배포
- 🔄 포트폴리오 최적화 에이전트 추가
- 🔄 위험 관리 시스템 구현

### Q4 2026
- 🔄 고급 시각화 및 분석 도구
- 🔄 모바일 앱 개발
- 🔄 커뮤니티 피처 추가

---

## 👨‍💻 작성자

**임찬주 (Chanju Lim)**
- 🎓 경제 데이터 과학 연구자
- 🚀 AI 에이전트 개발자
- 📊 금융 시장 분석가

---

## 🙏 감사의 말

이 프로젝트는 다음의 멋진 서비스와 라이브러리들 덕분에 가능했습니다:

- CoinGecko, CoinMarketCap, Alpha Vantage 등 API 제공자
- pandas, scikit-learn, TensorFlow/PyTorch 등 오픈소스 커뮤니티
- GitHub 및 오픈소스 생태계

---

**마지막 업데이트**: 2026-03-06  
**상태**: 🟢 활발히 개발 중

⭐ 이 프로젝트가 유용하다면 Star를 눌러주세요!