# VTuber 솔루션 개발 로드맵 V3.0 (전면 개정판)

> **버전**: 3.0
> **최종 수정**: 2025-11-17
> **변경 이력**: [ROADMAP_V2_ANALYSIS.md](./ROADMAP_V2_ANALYSIS.md) 참조
> **V2.1 업데이트**: Live2D 파트별 AI 생성 전략 추가
> **V2.2 업데이트**: 파트 조화 및 일관성 시스템 추가
> **V3.0 업데이트**: 15개 간과 영역 전면 통합, 운영/품질/MLOps 강화 ⭐⭐⭐

---

## 📋 V3.0 개정 요약

### 🎯 **V3.0의 핵심 철학**

> **"기술적 완벽성보다 운영 가능한 현실성"**
> **"사용자가 실패하지 않도록 돕는 시스템"**
> **"확장 가능하고 유지보수 가능한 아키텍처"**

### 🔥 **주요 변경사항**

#### ✅ **15개 간과 영역 전면 통합**
1. ✅ Live2D 파트 생성 현실 문제 해결 (얼굴 각도, 표정, 가림 처리)
2. ✅ 3D VRM 템플릿 전략 개선 (다양성 vs 비용 균형)
3. ✅ RVC 음성 품질 현실적 가이드 (5-10분 학습 데이터)
4. ✅ 립싱크 다국어 지원 (한국어, 일본어, 영어)
5. ✅ 데이터 생명주기 관리 체계 구축
6. ✅ 입력 전처리 및 품질 검증 강화
7. ✅ 보안 심층 방어 전략 (OWASP Top 10)
8. ✅ 캐싱 및 성능 최적화 상세화
9. ✅ 사용자 경험 (UX) 체계적 설계
10. ✅ 품질 보증 (QA) 완전 자동화
11. ✅ 확장성 및 부하 관리 전략
12. ✅ 비용 최적화 및 FinOps
13. ✅ 재해 복구 및 비즈니스 연속성
14. ✅ 국제화 및 현지화 전략
15. ✅ AI 모델 MLOps 체계

#### 🏗️ **구조적 변화**
- **Phase 수**: 20개 → **23개** (+3)
  - Phase 21: 운영 안정성 (Observability) ⭐ 신규
  - Phase 22: 품질 보증 (QA Strategy) ⭐ 신규
  - Phase 23: MLOps (Model Lifecycle) ⭐ 신규
- **총 단계**: 925개 → **~1,280개** (+355)
- **MVP 기간**: 6개월 → **7개월** (품질 강화)
- **전체 개발 기간**: 12개월 → **15개월** (운영 안정화 포함)

#### 📊 **Phase별 확장**
| Phase | V2.2 Steps | V3.0 Steps | 증가 | 주요 추가 사항 |
|-------|-----------|-----------|------|--------------|
| 0 | 30 | 50 | +20 | QA 전략, 테스트 자동화 |
| 1 | 95 | 125 | +30 | 데이터 생명주기, 보안 심층화 |
| 2 | 40 | 75 | +35 | 입력 품질 개선, 전처리 강화 |
| 3 | 50 | 50 | 0 | 유지 |
| 4 | 70 | 85 | +15 | 템플릿 다양화, 텍스처 품질 |
| 5 | 50 | 75 | +25 | 음성 품질 검증, 노이즈 제거 |
| 6 | 35 | 55 | +20 | 다국어 립싱크 |
| 7 | 55 | 60 | +5 | WebRTC 최적화 |
| 8 | 95 | 130 | +35 | UX 최적화, 온보딩, 접근성 |
| 9 | 30 | 35 | +5 | MVP 테스트 강화 |
| 10 | 90 | 115 | +25 | 파트 전처리, 조화 강화 |
| 11 | 25 | 30 | +5 | - |
| 12 | 35 | 80 | +45 | 캐싱, 비용 최적화, 확장성 |
| 13 | 35 | 40 | +5 | - |
| 14 | 35 | 55 | +20 | 재해 복구 상세화 |
| 15 | 30 | 35 | +5 | - |
| 16 | 30 | 35 | +5 | - |
| 17 | 20 | 40 | +20 | i18n/l10n 강화 |
| 18 | 20 | 25 | +5 | - |
| 19 | 25 | 30 | +5 | - |
| 20 | 35 | 40 | +5 | - |
| **21** | **0** | **45** | **+45** | **운영 안정성** ⭐ |
| **22** | **0** | **60** | **+60** | **품질 보증** ⭐ |
| **23** | **0** | **40** | **+40** | **MLOps** ⭐ |
| **합계** | **925** | **1,285** | **+360** | - |

---

## 🎯 프로젝트 개요

**프로젝트 명**: Koo Virtual Youtuber Manager
**목표**: 사진과 음성만으로 누구나 VTuber가 될 수 있는 **운영 가능한** 올인원 솔루션
**핵심 전략**: 빠른 MVP → 사용자 피드백 → 품질 강화 → 안정적 운영

### 🔑 **V3.0 핵심 가치**

1. **신뢰성** (Reliability): 99.9% 업타임, 자동 복구
2. **품질** (Quality): 저품질 입력도 처리, 실패율 <5%
3. **사용성** (Usability): 비전문가도 5분 내 아바타 생성
4. **확장성** (Scalability): 10명 → 10,000명 무중단 확장
5. **보안** (Security): OWASP Top 10 준수, 데이터 암호화
6. **비용 효율** (Cost Efficiency): 사용자당 월 $2 이하 운영

### 🛠️ **기술 스택**

#### 백엔드
- **웹 프레임워크**: FastAPI 0.100+
- **ORM**: SQLAlchemy 2.0 (async)
- **데이터베이스**: PostgreSQL 15+ (프로덕션), SQLite (로컬)
- **캐시**: Redis 7+ (세션, API 캐시, 작업 큐)
- **작업 큐**: Celery + RabbitMQ
- **WebSocket**: FastAPI WebSocket
- **인증**: JWT (python-jose), OAuth2 (Authlib)
- **보안**: slowapi (rate limiting), python-multipart, bcrypt

#### AI/ML
- **딥러닝**: PyTorch 2.0+, CUDA 11.8+
- **컴퓨터 비전**: OpenCV 4.8+, MediaPipe 0.10+
- **Face Parsing**: BiSeNet, face-parsing.PyTorch
- **음성 처리**: librosa, soundfile, sounddevice, RNNoise
- **음성 변환**: RVC (Retrieval-based Voice Conversion)
- **3D 생성**: DECA (얼굴), 템플릿 기반
- **이미지 생성**: Stable Diffusion 1.5/XL, ControlNet 1.1
- **이미지 품질 개선**: Real-ESRGAN, GFPGAN ⭐ (V3.0 신규)
- **색상 조화**: colorharmony, color-thief-py
- **이미지 블렌딩**: scikit-image (Poisson blending)
- **조명 정규화**: Retinex
- **배경 제거**: rembg (U2-Net)
- **립싱크**: Rhubarb Lip Sync (영어), 자체 구현 (한국어/일본어) ⭐

#### 프론트엔드
- **프레임워크**: React 18+
- **언어**: TypeScript 5+
- **빌드 도구**: Vite 4+
- **라우팅**: React Router 6+
- **상태 관리**: Zustand
- **UI 라이브러리**: shadcn/ui, Radix UI
- **스타일링**: Tailwind CSS 3+
- **3D 렌더링**: Three.js, @pixiv/three-vrm
- **2D 렌더링**: PixiJS 7+, Live2D Cubism SDK
- **API 클라이언트**: Axios, TanStack Query
- **폼**: React Hook Form
- **i18n**: react-i18next ⭐
- **온보딩**: Intro.js, Shepherd.js ⭐ (V3.0 신규)
- **테스트**: Vitest, React Testing Library, Playwright

#### 데스크톱
- **프레임워크**: Electron 25+
- **가상 카메라**: pyvirtualcam, v4l2loopback (Linux), OBS Virtual Cam

#### DevOps & 운영
- **컨테이너**: Docker, Docker Compose
- **CI/CD**: GitHub Actions
- **클라우드**: AWS / GCP / Azure (선택)
- **모니터링**: Prometheus, Grafana, Sentry ⭐
- **로그**: Loki, ELK Stack ⭐
- **추적**: OpenTelemetry, Jaeger ⭐ (V3.0 신규)
- **비용 관리**: CloudHealth, Kubecost ⭐ (V3.0 신규)
- **ML 관리**: MLflow, Weights & Biases ⭐ (V3.0 신규)

#### 품질 보증
- **단위 테스트**: pytest, Vitest
- **통합 테스트**: pytest + Testcontainers
- **E2E 테스트**: Playwright ⭐
- **성능 테스트**: Locust, k6 ⭐
- **보안 스캔**: OWASP ZAP, Snyk ⭐
- **코드 품질**: SonarQube ⭐ (V3.0 신규)

### 🎯 **MVP 핵심 기능** (7개월)

1. ✅ 웹캠 얼굴 트래킹 (MediaPipe)
2. ✅ 얼굴 사진 → 3D VRM 아바타 (템플릿 기반, 10+ 템플릿)
3. ✅ 실시간 아바타 애니메이션 (60fps, <300ms 레이턴시)
4. ✅ 음성 변환 (RVC, 5-10분 학습 데이터)
5. ✅ 다국어 립싱크 (한국어, 영어, 일본어)
6. ✅ OBS 가상 카메라 출력
7. ✅ 웹 인터페이스 (온보딩, UX 최적화)
8. ✅ **품질 보증** (자동화된 테스트, 에러 복구) ⭐
9. ✅ **운영 모니터링** (Observability) ⭐
10. ✅ **보안 강화** (OWASP Top 10 대응) ⭐

---

## 🏗️ 아키텍처 설계

### 전체 시스템 구조

```
┌─────────────────────────────────────────────────────────────────────┐
│                         Frontend Layer                              │
├─────────────────────────────────────────────────────────────────────┤
│  Web App (React + TS + Vite)                                        │
│  - UI Components (shadcn/ui)                                        │
│  - State Management (Zustand)                                       │
│  - WebSocket Client                                                 │
│  - 3D Renderer (Three.js + VRM)                                     │
│  - 2D Renderer (PixiJS + Live2D)                                    │
│  - Onboarding (Intro.js) ⭐                                         │
│  - i18n (react-i18next) ⭐                                          │
└─────────────────────────────────────────────────────────────────────┘
                            ↓ REST API / WebSocket / WebRTC
┌─────────────────────────────────────────────────────────────────────┐
│                    Backend API Layer                                │
├─────────────────────────────────────────────────────────────────────┤
│  FastAPI Server + WebSocket + Security Layer                       │
│  - Rate Limiting (Tiered) ⭐                                        │
│  - CORS (화이트리스트)                                              │
│  - Authentication (JWT + OAuth2)                                    │
│  - API Gateway                                                      │
│  - Feature Flags                                                    │
│  - Input Validation ⭐                                              │
└─────────────────────────────────────────────────────────────────────┘
                            ↓
┌─────────────────────────────────────────────────────────────────────┐
│                  Core Service Layer                                 │
├──────────────┬──────────────┬──────────────┬──────────────┬─────────┤
│ Voice        │ Avatar       │ Tracking     │ Streaming    │ Data    │
│ Service      │ Service      │ Service      │ Service      │ Mgmt ⭐ │
│ (RVC)        │ (VRM/L2D)    │ (MediaPipe)  │ (WebRTC/WS)  │         │
└──────────────┴──────────────┴──────────────┴──────────────┴─────────┘
                            ↓
┌─────────────────────────────────────────────────────────────────────┐
│                   AI/ML Engine Layer                                │
├──────────────┬──────────────┬──────────────┬──────────────┬─────────┤
│ RVC Engine   │ Face Mesh    │ Face Parsing │ SD + CN      │ Quality │
│ (PyTorch)    │ (MediaPipe)  │ (BiSeNet)    │ (Diffusion)  │ Enhance │
│              │              │              │              │ ⭐      │
└──────────────┴──────────────┴──────────────┴──────────────┴─────────┘
                            ↓
┌─────────────────────────────────────────────────────────────────────┐
│                Infrastructure Layer                                 │
├──────────────┬──────────────┬──────────────┬──────────────┬─────────┤
│ Database     │ Cache        │ Queue        │ Storage      │ Monitor │
│ (PostgreSQL) │ (Redis)      │ (Celery)     │ (S3/Local)   │ ⭐      │
│ + Replica ⭐ │ + Cluster ⭐ │ + Priority⭐ │ + CDN ⭐     │ (Prom)  │
└──────────────┴──────────────┴──────────────┴──────────────┴─────────┘
```

### 🔄 **데이터 흐름**

```
사용자 업로드 (얼굴 사진)
    ↓
입력 검증 및 전처리 ⭐
    ├─ 얼굴 감지 (MTCNN)
    ├─ 각도 검증 (±15도)
    ├─ 품질 검사 (해상도, 조명)
    ├─ 자동 개선 (업스케일, 노이즈 제거)
    └─ 배경 제거 (rembg)
    ↓
템플릿 매칭 또는 파트 생성
    ├─ VRM: 템플릿 선택 → 텍스처 매핑
    └─ Live2D: Face Parsing → 파트 생성 → 조화 처리
    ↓
아바타 저장 (DB + S3)
    ↓
실시간 트래킹 (MediaPipe)
    ↓
음성 변환 (RVC) + 립싱크
    ↓
렌더링 (Three.js / PixiJS)
    ↓
스트리밍 출력 (OBS / WebRTC)
```

---

# 🎯 MVP 개발 (Phase 0-9)

## Phase 0: 프로젝트 초기 설정 및 QA 기반 구축 (1-50) ⭐

> **목표**: 견고한 개발 환경, 자동화된 품질 보증, 포괄적 문서화
> **V3.0 핵심**: 테스트 자동화 및 CI/CD 파이프라인 완성

### Phase 0.1: 프로젝트 구조 및 환경 (1-10)
1. Git 저장소 초기화 및 .gitignore 설정
2. 프로젝트 루트 디렉토리 구조 설계
   ```
   /
   ├── backend/
   ├── frontend/
   ├── desktop/
   ├── docs/
   ├── tests/
   ├── scripts/
   └── .github/
   ```
3. 백엔드 디렉토리 구조 (`backend/`)
   ```
   backend/
   ├── app/
   │   ├── api/
   │   ├── core/
   │   ├── models/
   │   ├── services/
   │   ├── schemas/
   │   └── utils/
   ├── tests/
   ├── alembic/
   └── requirements.txt
   ```
4. 프론트엔드 디렉토리 구조 (`frontend/`)
5. Python 가상환경 및 requirements.txt
6. Node.js 프로젝트 초기화 (package.json)
7. Docker 환경 설정 (Dockerfile, docker-compose.yml)
8. 개발 환경 변수 관리 (.env.template)
9. 코드 포맷터 설정 (black, prettier, eslint)
10. pre-commit hooks 설정 (black, mypy, eslint)

### Phase 0.2: 개발 도구 및 품질 관리 (11-30) ⭐
11. **테스트 프레임워크 설정**: pytest (backend), Vitest (frontend)
12. **코드 커버리지 도구**: coverage.py, vitest coverage
    - 목표: >80% (핵심 로직 >90%)
13. **CI/CD 파이프라인 기본 설정** (GitHub Actions)
    ```yaml
    # .github/workflows/ci.yml
    on: [push, pull_request]
    jobs:
      lint:
        - black --check
        - pylint
        - eslint
      test:
        - pytest --cov=app --cov-report=xml
        - vitest run --coverage
      build:
        - docker build
    ```
14. **로깅 라이브러리 설정**: structlog (구조화된 JSON 로그)
15. **에러 트래킹 준비**: Sentry SDK 통합
16. **API 문서 자동화**: OpenAPI/Swagger 설정
17. **타입 체크 설정**: mypy (Python), TypeScript strict mode
18. **린터 설정**: pylint, ESLint
19. **개발 서버 실행 스크립트**: `make dev`
20. **Makefile / 태스크 러너** 설정
    ```makefile
    .PHONY: dev test lint format clean
    dev:
        docker-compose up -d
    test:
        pytest tests/
    lint:
        black --check app/
        pylint app/
    format:
        black app/
    clean:
        find . -type d -name __pycache__ -exec rm -rf {} +
    ```
21. **단위 테스트 샘플 작성** (pytest fixtures)
22. **통합 테스트 준비** (Docker Testcontainers)
23. **E2E 테스트 준비** (Playwright 설치 및 설정)
24. **성능 테스트 준비** (Locust 설치)
25. **보안 스캔 설정** (OWASP ZAP, Snyk)
26. **코드 품질 게이트** (SonarQube 또는 CodeClimate)
27. **의존성 업데이트 자동화** (Dependabot)
28. **Git Hooks 고급 설정** (commit message 규칙, branch naming)
29. **개발 환경 문서** (DEVELOPMENT.md)
30. **Phase 0.2 QA 체크리스트** 검증

### Phase 0.3: 문서화 (31-45)
31. **README.md** (프로젝트 소개, 설치 방법, 빠른 시작)
32. **CONTRIBUTING.md** (기여 가이드, 코드 스타일, PR 프로세스)
33. **ARCHITECTURE.md** (시스템 아키텍처, 데이터 흐름)
34. **API 명세 초안** (OpenAPI 3.0 스키마)
35. **데이터베이스 스키마 초안** (ERD 다이어그램)
36. **개발 로드맵** (현재 문서)
37. **라이선스 선택 및 LICENSE 파일** (MIT or Apache 2.0 권장)
38. **이슈 템플릿** (.github/ISSUE_TEMPLATE/)
    - Bug report
    - Feature request
    - Question
39. **PR 템플릿** (.github/PULL_REQUEST_TEMPLATE.md)
40. **보안 정책** (SECURITY.md, 취약점 보고 프로세스)
41. **코드 오브 컨덕트** (CODE_OF_CONDUCT.md)
42. **체인지로그** (CHANGELOG.md)
43. **FAQ 초안** (자주 묻는 질문)
44. **온보딩 가이드** (신규 개발자용)
45. **Phase 0.3 문서 검토 및 승인**

### Phase 0.4: 테스트 전략 수립 ⭐⭐⭐ (46-50)
46. **단위 테스트 전략 문서** (QA_STRATEGY.md)
    - 커버리지 목표: >80%
    - Mock/Stub 전략
    - Fixture 관리
47. **통합 테스트 전략**
    - DB 마이그레이션 테스트
    - API 엔드포인트 테스트
    - 서비스 간 통합 테스트
48. **E2E 테스트 시나리오 목록**
    - 사용자 회원가입 → 아바타 생성 → 스트리밍
    - 에러 처리 시나리오
49. **성능 테스트 기준선** (Baseline)
    - 목표 RPS (Requests Per Second)
    - 목표 레이턴시 (P50, P95, P99)
50. **테스트 자동화 검증** (모든 테스트 실행 및 통과 확인)

---

## Phase 1: 백엔드 인프라 구축 및 데이터 관리 (51-175) ⭐

> **목표**: 견고한 백엔드, 보안, 인증, 데이터 생명주기 관리
> **V3.0 핵심**: 데이터 관리 체계, 보안 심층화

### Phase 1.1: FastAPI 기본 설정 (51-65)
51. FastAPI 프로젝트 초기화
52. 설정 관리 모듈 (config.py, Pydantic BaseSettings)
53. 구조화된 로깅 시스템 (structlog + JSON)
    ```python
    import structlog
    logger = structlog.get_logger()
    logger.info("user_registered", user_id=123, email="user@example.com")
    ```
54. 전역 에러 핸들러
55. CORS 설정 (화이트리스트 기반)
56. 헬스체크 엔드포인트 (/health, /ready)
57. API 버저닝 구조 (/api/v1)
58. 요청/응답 모델 (Pydantic BaseModel)
59. API 문서 자동 생성 (Swagger UI, ReDoc)
60. 미들웨어 체인 설정
61. 요청 ID 추적 (X-Request-ID)
62. Feature Flags 시스템 (환경 변수 기반)
63. 환경별 설정 (dev, staging, prod)
64. 개발 서버 hot reload 설정
65. Phase 1.1 유닛 테스트

### Phase 1.2: 데이터베이스 설정 (66-85)
66. SQLAlchemy ORM 설정
67. 데이터베이스 연결 관리 (asyncpg)
68. 커넥션 풀 최적화 (pool_size=20, max_overflow=10)
69. Alembic 마이그레이션 설정
70. Base 모델 및 믹스인 (timestamps, soft delete)
    ```python
    class TimestampMixin:
        created_at = Column(DateTime, default=datetime.utcnow)
        updated_at = Column(DateTime, onupdate=datetime.utcnow)

    class SoftDeleteMixin:
        deleted_at = Column(DateTime, nullable=True)
    ```
71. **User 모델 정의**
    ```python
    class User(Base, TimestampMixin, SoftDeleteMixin):
        id = Column(UUID, primary_key=True)
        email = Column(String, unique=True, nullable=False)
        hashed_password = Column(String, nullable=False)
        display_name = Column(String)
        quota_gb = Column(Integer, default=1)  # 스토리지 할당량
    ```
72. **Project 모델 정의** (VTuber 프로젝트)
    ```python
    class Project(Base, TimestampMixin, SoftDeleteMixin):
        id = Column(UUID, primary_key=True)
        user_id = Column(UUID, ForeignKey('users.id'))
        name = Column(String, nullable=False)
        description = Column(Text)
        version = Column(Integer, default=1)  # 버전 관리
    ```
73. **Avatar 모델 정의** (VRM, Live2D 메타데이터)
74. **VoiceModel 모델 정의**
75. **Session 모델 정의** (트래킹 세션)
76. **FacePart 모델 정의** (파트 DB)
77. **FileMetadata 모델 정의** ⭐ (V3.0 신규)
    ```python
    class FileMetadata(Base, TimestampMixin):
        id = Column(UUID, primary_key=True)
        user_id = Column(UUID, ForeignKey('users.id'))
        file_path = Column(String, nullable=False)
        file_size = Column(BigInteger)  # bytes
        mime_type = Column(String)
        checksum = Column(String)  # SHA-256
        last_accessed = Column(DateTime)
    ```
78. **AuditLog 모델 정의** ⭐ (V3.0 신규 - 변경 이력)
    ```python
    class AuditLog(Base):
        id = Column(UUID, primary_key=True)
        user_id = Column(UUID)
        action = Column(String)  # 'create', 'update', 'delete'
        resource_type = Column(String)  # 'avatar', 'project'
        resource_id = Column(UUID)
        changes = Column(JSONB)  # {'field': {'old': ..., 'new': ...}}
        timestamp = Column(DateTime, default=datetime.utcnow)
    ```
79. 모델 관계 설정 (Foreign Keys, Relationships)
80. 인덱스 설계 및 추가
    ```python
    Index('ix_users_email', User.email)
    Index('ix_projects_user_id', Project.user_id)
    Index('ix_audit_logs_user_id_timestamp', AuditLog.user_id, AuditLog.timestamp)
    ```
81. 초기 마이그레이션 파일 생성
82. 데이터베이스 시딩 스크립트
83. Phase 1.2 DB 테스트
84. DB 마이그레이션 롤백 테스트
85. DB 성능 벤치마크 (쿼리 실행 시간)

### Phase 1.3: 인증 및 권한 (86-105)
86. JWT 토큰 생성/검증 (python-jose)
    - Access token: 15분 TTL
    - Refresh token: 7일 TTL
87. 패스워드 해싱 (bcrypt, cost factor 12)
88. 사용자 등록 API (/api/v1/auth/register)
    - 이메일 중복 검증
    - 패스워드 강도 검증 (최소 8자, 대소문자, 숫자, 특수문자)
89. 로그인 API (/api/v1/auth/login)
90. 토큰 갱신 API (/api/v1/auth/refresh)
91. 로그아웃 API (토큰 무효화 - Redis 블랙리스트)
92. 인증 미들웨어 (get_current_user)
93. 권한 검증 데코레이터 (require_permission)
94. OAuth2 준비 (Google, GitHub)
95. 패스워드 재설정 플로우
    - 이메일 발송 (토큰 포함)
    - 토큰 검증 및 패스워드 변경
96. 이메일 인증 (선택적)
97. API 키 생성 및 관리
98. 세션 관리 (Redis)
99. 2FA (Two-Factor Authentication) 준비 (선택적)
100. RBAC (Role-Based Access Control) 설계
     - Roles: admin, user, guest
     - Permissions: create_avatar, delete_project, etc.
101. Phase 1.3 인증 테스트
102. 인증 API 문서 업데이트
103. 보안 테스트 (Brute force 방어)
104. JWT 토큰 탈취 시나리오 테스트
105. OAuth2 통합 테스트

### Phase 1.4: 보안 시스템 심층 방어 ⭐⭐⭐ (106-140)

> **V3.0 핵심**: OWASP Top 10 완전 대응, 다층 방어

#### 1.4.1: 입력 검증 및 보호 (106-115)
106. **파일 타입 검증**
     - MIME type 체크 (magic number)
     - 확장자 화이트리스트
     ```python
     ALLOWED_EXTENSIONS = {'.jpg', '.png', '.wav', '.mp3'}
     ALLOWED_MIME_TYPES = {'image/jpeg', 'image/png', 'audio/wav'}

     def validate_file(file):
         # Magic number 체크
         file_type = magic.from_buffer(file.read(1024), mime=True)
         if file_type not in ALLOWED_MIME_TYPES:
             raise ValueError("Invalid file type")
     ```
107. **이미지 폭탄 방어** (Decompression bomb)
     ```python
     from PIL import Image
     Image.MAX_IMAGE_PIXELS = 100_000_000  # 100MP 제한
     ```
108. **ZIP 폭탄 방어**
     ```python
     MAX_ZIP_SIZE = 100 * 1024 * 1024  # 100MB
     MAX_UNCOMPRESSED_SIZE = 500 * 1024 * 1024  # 500MB
     ```
109. **SVG 인젝션 방어** (XXE 공격)
     - SVG 업로드 금지 또는 sanitization
110. **Path traversal 방어**
     ```python
     import os
     def safe_join(base_path, user_input):
         path = os.path.normpath(os.path.join(base_path, user_input))
         if not path.startswith(base_path):
             raise ValueError("Path traversal detected")
         return path
     ```
111. **SQL 인젝션 방어** (SQLAlchemy ORM 사용, raw query 금지)
112. **XSS 방어** (입력 sanitization, CSP 헤더)
     ```python
     from fastapi.middleware.cors import CORSMiddleware
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["https://yourdomain.com"],
         allow_credentials=True,
         allow_methods=["GET", "POST", "PUT", "DELETE"],
         allow_headers=["Authorization", "Content-Type"],
     )
     ```
113. **CSRF 방어** (SameSite 쿠키, CSRF 토큰)
114. **Command 인젝션 방어** (subprocess 사용 시 shell=False)
115. **Phase 1.4.1 보안 테스트** (OWASP ZAP 스캔)

#### 1.4.2: API 보안 상세화 (116-125)
116. **JWT 보안 강화**
     ```python
     # Access token: 15분
     # Refresh token: 7일, HTTP-only cookie
     # Token rotation: Refresh 시 새 토큰 발급

     def create_access_token(data: dict):
         to_encode = data.copy()
         expire = datetime.utcnow() + timedelta(minutes=15)
         to_encode.update({"exp": expire, "type": "access"})
         return jwt.encode(to_encode, SECRET_KEY, algorithm="HS256")

     def create_refresh_token(user_id: str):
         expire = datetime.utcnow() + timedelta(days=7)
         to_encode = {"sub": user_id, "exp": expire, "type": "refresh"}
         token = jwt.encode(to_encode, SECRET_KEY, algorithm="HS256")
         # Redis에 저장
         redis_client.setex(f"refresh_token:{user_id}", 7*24*3600, token)
         return token
     ```
117. **Token blacklist 구현** (로그아웃 시)
     ```python
     def revoke_token(token: str):
         redis_client.setex(f"blacklist:{token}", 15*60, "1")
     ```
118. **API Key 관리**
     - Hashed storage (SHA-256)
     - Rate limiting per API key
     - IP whitelist (옵션)
119. **CORS 정밀 설정**
     - Allowed origins 화이트리스트
     - Preflight request 처리
120. **HTTPS 강제** (TLS 1.3)
     ```python
     from fastapi.middleware.httpsredirect import HTTPSRedirectMiddleware
     app.add_middleware(HTTPSRedirectMiddleware)
     ```
121. **HSTS 헤더**
     ```python
     @app.middleware("http")
     async def add_security_headers(request, call_next):
         response = await call_next(request)
         response.headers["Strict-Transport-Security"] = "max-age=31536000; includeSubDomains"
         response.headers["X-Content-Type-Options"] = "nosniff"
         response.headers["X-Frame-Options"] = "DENY"
         response.headers["X-XSS-Protection"] = "1; mode=block"
         return response
     ```
122. **API 버전 관리 및 Deprecation 정책**
123. **API 문서 접근 제어** (프로덕션에서 /docs 비활성화 또는 인증)
124. **Phase 1.4.2 API 보안 테스트**
125. **침투 테스트 (Penetration Testing)** 준비

#### 1.4.3: Rate Limiting 및 DDoS 방어 (126-135)
126. **Tiered rate limiting 구현** ⭐
     ```python
     from slowapi import Limiter
     from slowapi.util import get_remote_address

     limiter = Limiter(key_func=get_remote_address)

     # 미인증: 10 req/min
     @app.get("/api/v1/public")
     @limiter.limit("10/minute")
     async def public_endpoint():
         pass

     # 무료 사용자: 100 req/min
     @app.get("/api/v1/user")
     @limiter.limit("100/minute")
     async def user_endpoint(current_user: User = Depends(get_current_user)):
         pass

     # 유료 사용자: 1000 req/min
     @app.get("/api/v1/premium")
     @limiter.limit("1000/minute")
     async def premium_endpoint(current_user: User = Depends(get_premium_user)):
         pass
     ```
127. **엔드포인트별 Rate Limiting**
     ```python
     # 아바타 생성: 1 req/min (리소스 집약적)
     @app.post("/api/v1/avatars")
     @limiter.limit("1/minute")
     async def create_avatar():
         pass

     # 음성 변환: 10 req/min
     @app.post("/api/v1/voice/convert")
     @limiter.limit("10/minute")
     async def convert_voice():
         pass

     # 조회 API: 100 req/min
     @app.get("/api/v1/avatars")
     @limiter.limit("100/minute")
     async def list_avatars():
         pass
     ```
128. **IP 기반 + 사용자 기반 조합**
     ```python
     def get_identifier(request: Request):
         if request.state.user:
             return f"user:{request.state.user.id}"
         return f"ip:{request.client.host}"

     limiter = Limiter(key_func=get_identifier)
     ```
129. **동적 Rate Limiting** (시스템 부하 기반)
     ```python
     def dynamic_limit():
         cpu_usage = psutil.cpu_percent()
         if cpu_usage > 80:
             return "10/minute"  # 부하 높을 때 제한 강화
         return "100/minute"

     @app.get("/api/v1/dynamic")
     @limiter.limit(dynamic_limit)
     async def dynamic_endpoint():
         pass
     ```
130. **Distributed Rate Limiting** (Redis 기반)
     ```python
     from slowapi.extensions import RateLimitStorage
     from redis import Redis

     redis_client = Redis(host='localhost', port=6379)
     limiter = Limiter(
         key_func=get_identifier,
         storage_uri="redis://localhost:6379"
     )
     ```
131. **DDoS 방어 - Application Layer (L7)**
     - Request validation
     - Captcha (hCaptcha, reCAPTCHA)
     - Bot detection
132. **DDoS 방어 - Network Layer (L3/L4)**
     - Cloudflare 또는 AWS Shield 통합
     - SYN flood protection
133. **Rate limit 초과 시 응답**
     ```python
     @app.exception_handler(RateLimitExceeded)
     async def rate_limit_handler(request: Request, exc: RateLimitExceeded):
         return JSONResponse(
             status_code=429,
             content={
                 "error": "Too many requests",
                 "retry_after": exc.detail,
                 "limit": exc.limit
             },
             headers={"Retry-After": str(exc.detail)}
         )
     ```
134. **Phase 1.4.3 Rate Limiting 테스트**
135. **DDoS 시뮬레이션 테스트** (Locust)

#### 1.4.4: 데이터 암호화 (136-140)
136. **전송 암호화 (TLS 1.3)**
     - Let's Encrypt 인증서
     - HSTS 헤더
137. **저장 암호화**
     - DB 암호화: PostgreSQL TDE (선택적)
     - 파일 암호화: 민감 데이터만 (KMS)
     - 패스워드: bcrypt (cost factor 12)
     - API Key: SHA-256 해싱
138. **키 관리 (KMS)**
     - AWS KMS, Google Cloud KMS, HashiCorp Vault
     - 키 로테이션: 90일마다
139. **민감 정보 마스킹** (로그, 에러 메시지)
     ```python
     def mask_email(email: str) -> str:
         local, domain = email.split('@')
         return f"{local[0]}***@{domain}"

     logger.info("user_login", email=mask_email(user.email))
     ```
140. **Phase 1.4 보안 통합 테스트 및 OWASP ZAP 전체 스캔**

### Phase 1.5: 데이터 생명주기 관리 ⭐⭐⭐ (141-160)

> **V3.0 신규 Phase**: 데이터 버전 관리, 백업, 정합성, 스토리지 최적화

#### 1.5.1: 버전 관리 및 히스토리 (141-148)
141. **아바타 버전 관리 구현**
     ```python
     class AvatarVersion(Base, TimestampMixin):
         id = Column(UUID, primary_key=True)
         avatar_id = Column(UUID, ForeignKey('avatars.id'))
         version = Column(Integer, nullable=False)
         changes = Column(JSONB)  # 변경 내용
         created_by = Column(UUID, ForeignKey('users.id'))

     # 사용 예시
     def update_avatar(avatar_id, changes):
         avatar = db.query(Avatar).get(avatar_id)
         avatar.version += 1

         # 버전 히스토리 저장
         version = AvatarVersion(
             avatar_id=avatar_id,
             version=avatar.version,
             changes=changes
         )
         db.add(version)
     ```
142. **설정 변경 히스토리 (AuditLog 활용)**
     ```python
     def log_change(user_id, action, resource_type, resource_id, old_value, new_value):
         audit = AuditLog(
             user_id=user_id,
             action=action,
             resource_type=resource_type,
             resource_id=resource_id,
             changes={'old': old_value, 'new': new_value}
         )
         db.add(audit)
     ```
143. **롤백 기능 구현**
     ```python
     def rollback_to_version(avatar_id, target_version):
         version = db.query(AvatarVersion).filter(
             AvatarVersion.avatar_id == avatar_id,
             AvatarVersion.version == target_version
         ).first()

         if not version:
             raise ValueError("Version not found")

         # 버전 데이터로 복원
         avatar = db.query(Avatar).get(avatar_id)
         avatar.apply_changes(version.changes)
         avatar.version = target_version
     ```
144. **Soft delete 구현** (deleted_at 플래그)
     ```python
     def soft_delete(model_id):
         model = db.query(Model).get(model_id)
         model.deleted_at = datetime.utcnow()
         db.commit()

     def restore(model_id):
         model = db.query(Model).get(model_id)
         model.deleted_at = None
         db.commit()

     # 쿼리 시 deleted_at IS NULL 조건 자동 추가
     db.query(Model).filter(Model.deleted_at.is_(None))
     ```
145. **변경 이력 조회 API** (/api/v1/audit-logs)
146. **버전 비교 기능** (diff)
147. **Phase 1.5.1 버전 관리 테스트**
148. **롤백 시나리오 테스트**

#### 1.5.2: 데이터 정합성 및 무결성 (149-153)
149. **Foreign Key 제약 조건 검증**
     - ON DELETE CASCADE 또는 RESTRICT 설정
150. **고아 레코드 탐지 및 정리**
     ```python
     def find_orphaned_files():
         # DB에는 있지만 파일 시스템에 없는 레코드
         files_in_db = db.query(FileMetadata.file_path).all()
         for file_path in files_in_db:
             if not os.path.exists(file_path):
                 logger.warning("orphaned_file_in_db", path=file_path)

         # 파일 시스템에는 있지만 DB에 없는 파일
         files_on_disk = glob.glob("uploads/**/*", recursive=True)
         for file_path in files_on_disk:
             if not db.query(FileMetadata).filter(
                 FileMetadata.file_path == file_path
             ).first():
                 logger.warning("orphaned_file_on_disk", path=file_path)
     ```
151. **파일과 DB 레코드 동기화 검증**
     ```python
     def verify_file_integrity():
         files = db.query(FileMetadata).all()
         for file in files:
             if not os.path.exists(file.file_path):
                 logger.error("file_missing", file_id=file.id, path=file.file_path)
                 continue

             # Checksum 검증
             actual_checksum = calculate_sha256(file.file_path)
             if actual_checksum != file.checksum:
                 logger.error("checksum_mismatch", file_id=file.id)
     ```
152. **정기 무결성 체크 (Cron job)**
     ```python
     # scripts/integrity_check.py
     # Cron: 매일 새벽 3시 실행
     from celery.schedules import crontab

     @celery.task
     def daily_integrity_check():
         verify_file_integrity()
         find_orphaned_files()
         check_foreign_keys()

     celery.conf.beat_schedule = {
         'integrity-check': {
             'task': 'tasks.daily_integrity_check',
             'schedule': crontab(hour=3, minute=0)
         }
     }
     ```
153. **Phase 1.5.2 무결성 테스트**

#### 1.5.3: 스토리지 관리 (154-160)
154. **파일 크기 제한 구현**
     ```python
     MAX_FILE_SIZE = {
         'image': 10 * 1024 * 1024,  # 10MB
         'vrm': 50 * 1024 * 1024,     # 50MB
         'audio': 100 * 1024 * 1024   # 100MB
     }

     @app.post("/api/v1/upload")
     async def upload_file(file: UploadFile):
         file_size = 0
         async for chunk in file.stream():
             file_size += len(chunk)
             if file_size > MAX_FILE_SIZE['image']:
                 raise HTTPException(413, "File too large")
     ```
155. **사용자별 할당량 (Quota) 구현**
     ```python
     def check_quota(user_id: UUID, file_size: int):
         user = db.query(User).get(user_id)
         used_space = db.query(func.sum(FileMetadata.file_size)).filter(
             FileMetadata.user_id == user_id
         ).scalar() or 0

         if used_space + file_size > user.quota_gb * 1024**3:
             raise HTTPException(507, "Quota exceeded")

     @app.post("/api/v1/upload")
     async def upload_file(file: UploadFile, user: User = Depends(get_current_user)):
         check_quota(user.id, file.size)
         # ...
     ```
156. **자동 압축 구현**
     ```python
     from PIL import Image

     def compress_image(input_path, output_path, quality=85):
         img = Image.open(input_path)
         # PNG → WebP 변환
         img.save(output_path, format='WebP', quality=quality, optimize=True)

         # 용량 비교
         original_size = os.path.getsize(input_path)
         compressed_size = os.path.getsize(output_path)
         savings = (1 - compressed_size / original_size) * 100
         logger.info("image_compressed", savings=f"{savings:.1f}%")
     ```
157. **오래된 임시 파일 자동 삭제**
     ```python
     @celery.task
     def cleanup_temp_files():
         temp_dir = "/tmp/uploads"
         cutoff = datetime.utcnow() - timedelta(days=7)

         for file_path in glob.glob(f"{temp_dir}/*"):
             file_time = datetime.fromtimestamp(os.path.getmtime(file_path))
             if file_time < cutoff:
                 os.remove(file_path)
                 logger.info("temp_file_deleted", path=file_path)
     ```
158. **CDN 캐시 무효화 API**
     ```python
     import boto3

     def invalidate_cdn_cache(file_paths: List[str]):
         client = boto3.client('cloudfront')
         response = client.create_invalidation(
             DistributionId='YOUR_DISTRIBUTION_ID',
             InvalidationBatch={
                 'Paths': {
                     'Quantity': len(file_paths),
                     'Items': file_paths
                 },
                 'CallerReference': str(datetime.utcnow().timestamp())
             }
         )
         return response
     ```
159. **스토리지 사용량 모니터링 대시보드**
160. **Phase 1.5.3 스토리지 관리 테스트**

### Phase 1.6: 백업 및 복구 전략 (161-175) ⭐
161. **자동 백업 스케줄 설정**
     ```bash
     # Cron: 매일 3시 (UTC)
     0 3 * * * /usr/bin/pg_dump -U postgres vtuber_db | gzip > /backups/daily/$(date +\%Y\%m\%d).sql.gz

     # 주간 백업: 매주 일요일
     0 3 * * 0 /usr/bin/pg_dump -U postgres vtuber_db | gzip > /backups/weekly/$(date +\%Y\%m\%d).sql.gz
     ```
162. **Full backup 구현** (pg_dump)
163. **Incremental backup 구현** (WAL archiving)
     ```ini
     # postgresql.conf
     wal_level = replica
     archive_mode = on
     archive_command = 'cp %p /backups/wal/%f'
     ```
164. **Transaction log backup** (PostgreSQL WAL)
165. **백업 보존 정책 구현**
     ```python
     RETENTION_POLICY = {
         'daily': timedelta(days=7),
         'weekly': timedelta(weeks=4),
         'monthly': timedelta(days=365)
     }

     def cleanup_old_backups():
         for backup_type, retention in RETENTION_POLICY.items():
             cutoff = datetime.utcnow() - retention
             backup_dir = f"/backups/{backup_type}"

             for backup_file in glob.glob(f"{backup_dir}/*.sql.gz"):
                 file_time = datetime.fromtimestamp(os.path.getmtime(backup_file))
                 if file_time < cutoff:
                     os.remove(backup_file)
     ```
166. **백업 테스트 (월 1회 복구 테스트)**
     ```python
     @celery.task
     def monthly_backup_test():
         # 랜덤 백업 선택
         backup_file = random.choice(glob.glob("/backups/daily/*.sql.gz"))

         # 테스트 DB에 복구
         subprocess.run([
             'gunzip', '-c', backup_file, '|',
             'psql', '-U', 'postgres', '-d', 'vtuber_test'
         ])

         # 무결성 검증
         result = verify_database_integrity('vtuber_test')
         if not result:
             alert_team("Backup test failed!")
     ```
167. **복구 시간 측정 (RTO)** - 목표: <4시간
168. **복구 지점 목표 (RPO)** - 목표: <1시간 데이터 손실
169. **지리적 복제 설정** (S3 Cross-Region Replication)
     ```python
     import boto3

     s3 = boto3.client('s3')
     s3.put_bucket_replication(
         Bucket='primary-bucket',
         ReplicationConfiguration={
             'Role': 'arn:aws:iam::...',
             'Rules': [{
                 'Status': 'Enabled',
                 'Destination': {
                     'Bucket': 'arn:aws:s3:::secondary-bucket',
                     'ReplicationTime': {'Status': 'Enabled', 'Time': {'Minutes': 15}}
                 }
             }]
         }
     )
     ```
170. **DB 복제 (Streaming Replication)**
     ```ini
     # Primary 서버
     wal_level = replica
     max_wal_senders = 5

     # Replica 서버
     hot_standby = on
     ```
171. **페일오버 절차 문서화** (Runbook)
172. **재해 복구 계획 (DRP) 문서**
173. **백업 암호화** (GPG)
     ```bash
     pg_dump vtuber_db | gzip | gpg --encrypt --recipient admin@example.com > backup.sql.gz.gpg
     ```
174. **Phase 1.6 백업 복구 통합 테스트**
175. **재해 시뮬레이션 (GameDay)** - DB 장애 대응 연습

---

## Phase 2: 파일 관리 및 입력 품질 개선 (176-250) ⭐⭐⭐

> **목표**: 저품질 입력도 처리 가능, 자동 개선, 품질 검증
> **V3.0 핵심**: 입력 전처리 대폭 강화, 사용자 실패율 최소화

### Phase 2.1: 파일 스토리지 기본 (176-190)
176. 로컬 파일 스토리지 구조 설계
     ```
     uploads/
     ├── users/
     │   └── {user_id}/
     │       ├── images/
     │       ├── audio/
     │       ├── avatars/
     │       └── temp/
     ```
177. 파일 업로드 API (/api/v1/upload)
178. 멀티파트 폼 데이터 처리
179. 파일 타입 검증 (Phase 1.4.1 재활용)
180. 파일 크기 제한 (Phase 1.5.3 재활용)
181. 파일 이름 sanitization
     ```python
     import re

     def sanitize_filename(filename: str) -> str:
         # 위험한 문자 제거
         filename = re.sub(r'[^\w\s.-]', '', filename)
         # 공백을 언더스코어로
         filename = filename.replace(' ', '_')
         # 연속된 점 제거
         filename = re.sub(r'\.+', '.', filename)
         return filename
     ```
182. UUID 기반 파일명 생성
     ```python
     import uuid
     from pathlib import Path

     def generate_unique_filename(original_filename: str) -> str:
         ext = Path(original_filename).suffix
         unique_id = uuid.uuid4()
         return f"{unique_id}{ext}"
     ```
183. 임시 파일 관리 및 정리 (Phase 1.5.3 Cron 활용)
184. 파일 삭제 API
185. S3 호환 스토리지 통합 (boto3) - 선택적
186. CDN 연동 준비 (CloudFront, Cloudflare)
187. 파일 메타데이터 저장 (FileMetadata 모델 활용)
188. 파일 다운로드 API (Presigned URL)
189. Phase 2.1 파일 스토리지 테스트
190. S3 업로드 성능 테스트

### Phase 2.2: 기본 이미지 처리 (191-200)
191. 이미지 리사이징 (Pillow)
     ```python
     from PIL import Image

     def resize_image(image_path, max_size=1024):
         img = Image.open(image_path)
         img.thumbnail((max_size, max_size), Image.Resampling.LANCZOS)
         img.save(image_path)
     ```
192. 썸네일 생성
193. EXIF 데이터 읽기 및 회전 보정
     ```python
     from PIL import Image, ExifTags

     def fix_orientation(image_path):
         img = Image.open(image_path)
         try:
             for orientation in ExifTags.TAGS.keys():
                 if ExifTags.TAGS[orientation] == 'Orientation':
                     break
             exif = img._getexif()
             if exif:
                 orientation_value = exif[orientation]
                 if orientation_value == 3:
                     img = img.rotate(180, expand=True)
                 elif orientation_value == 6:
                     img = img.rotate(270, expand=True)
                 elif orientation_value == 8:
                     img = img.rotate(90, expand=True)
         except:
             pass
         img.save(image_path)
     ```
194. 포맷 변환 (PNG → WebP)
195. 메타데이터 제거 (개인정보 보호)
196. 배경 제거 (rembg)
     ```python
     from rembg import remove

     def remove_background(input_path, output_path):
         with open(input_path, 'rb') as i:
             with open(output_path, 'wb') as o:
                 input_data = i.read()
                 output_data = remove(input_data)
                 o.write(output_data)
     ```
197. 이미지 검증 (손상된 이미지 감지)
     ```python
     from PIL import Image

     def verify_image(image_path):
         try:
             img = Image.open(image_path)
             img.verify()  # 이미지 검증
             return True
         except:
             return False
     ```
198. Phase 2.2 이미지 처리 테스트
199. 성능 벤치마크 (이미지당 처리 시간)
200. 메모리 사용량 모니터링

### Phase 2.3: 입력 품질 개선 및 전처리 ⭐⭐⭐ (201-235)

> **V3.0 핵심 신규 Sub-Phase**: 저품질 입력을 고품질로 자동 개선

#### 2.3.1: 이미지 품질 자동 개선 (201-215)
201. **저해상도 업스케일링 (Real-ESRGAN)** ⭐
     ```python
     from realesrgan import RealESRGAN

     def upscale_image(input_path, output_path, scale=2):
         model = RealESRGAN('RealESRGAN_x2plus')
         img = Image.open(input_path)
         result = model.predict(img)
         result.save(output_path)

         logger.info("image_upscaled",
                     original_size=img.size,
                     upscaled_size=result.size)
     ```
202. **얼굴 복원 (GFPGAN)** - 블러, 저품질 얼굴 개선 ⭐
     ```python
     from gfpgan import GFPGANer

     def restore_face(input_path, output_path):
         restorer = GFPGANer(
             model_path='GFPGANv1.3.pth',
             upscale=2,
             arch='clean',
             channel_multiplier=2
         )

         img = cv2.imread(input_path)
         _, _, restored_img = restorer.enhance(img)
         cv2.imwrite(output_path, restored_img)
     ```
203. **노이즈 제거 (Non-local means denoising)**
     ```python
     import cv2

     def denoise_image(image_path):
         img = cv2.imread(image_path)
         denoised = cv2.fastNlMeansDenoisingColored(img, None, 10, 10, 7, 21)
         cv2.imwrite(image_path, denoised)
     ```
204. **블러 제거 (Deblur GAN)** - 선택적
205. **저조도 보정 (EnlightenGAN)**
     ```python
     def enhance_low_light(input_path, output_path):
         # EnlightenGAN 모델 로드
         model = load_enlighten_gan()
         img = Image.open(input_path)
         enhanced = model.predict(img)
         enhanced.save(output_path)
     ```
206. **화이트 밸런스 자동 조정**
     ```python
     import cv2
     import numpy as np

     def auto_white_balance(image_path):
         img = cv2.imread(image_path)
         result = cv2.xphoto.createSimpleWB().balanceWhite(img)
         cv2.imwrite(image_path, result)
     ```
207. **샤프닝 (Unsharp mask)**
     ```python
     from PIL import ImageFilter

     def sharpen_image(image_path):
         img = Image.open(image_path)
         sharpened = img.filter(ImageFilter.UnsharpMask(radius=2, percent=150))
         sharpened.save(image_path)
     ```
208. **색상 보정 (Histogram equalization)**
     ```python
     import cv2

     def equalize_histogram(image_path):
         img = cv2.imread(image_path)
         img_yuv = cv2.cvtColor(img, cv2.COLOR_BGR2YUV)
         img_yuv[:,:,0] = cv2.equalizeHist(img_yuv[:,:,0])
         result = cv2.cvtColor(img_yuv, cv2.COLOR_YUV2BGR)
         cv2.imwrite(image_path, result)
     ```
209. **CLAHE (Contrast Limited Adaptive Histogram Equalization)**
     ```python
     def apply_clahe(image_path):
         img = cv2.imread(image_path)
         lab = cv2.cvtColor(img, cv2.COLOR_BGR2LAB)
         l, a, b = cv2.split(lab)

         clahe = cv2.createCLAHE(clipLimit=2.0, tileGridSize=(8,8))
         l = clahe.apply(l)

         lab = cv2.merge([l,a,b])
         result = cv2.cvtColor(lab, cv2.COLOR_LAB2BGR)
         cv2.imwrite(image_path, result)
     ```
210. **품질 개선 파이프라인 구성**
     ```python
     def enhance_image_quality(input_path, output_path):
         # 1. 노이즈 제거
         denoise_image(input_path)

         # 2. 저조도 개선 (필요 시)
         if is_low_light(input_path):
             enhance_low_light(input_path, input_path)

         # 3. 업스케일링 (해상도 < 512)
         if get_image_size(input_path)[0] < 512:
             upscale_image(input_path, input_path, scale=2)

         # 4. 얼굴 복원
         restore_face(input_path, input_path)

         # 5. 샤프닝
         sharpen_image(input_path)

         # 6. 최종 저장
         shutil.copy(input_path, output_path)
     ```
211. **품질 개선 전/후 비교 UI**
212. **사용자에게 개선 옵션 제공** ("자동 개선 적용" 체크박스)
213. **Phase 2.3.1 품질 개선 테스트**
214. **다양한 저품질 이미지 테스트셋** (100+ 이미지)
215. **품질 개선 성능 벤치마크** (처리 시간, GPU 사용률)

#### 2.3.2: 얼굴 감지 및 검증 (216-230)
216. **고정밀 얼굴 감지 (MTCNN 또는 RetinaFace)** ⭐
     ```python
     from mtcnn import MTCNN

     detector = MTCNN()

     def detect_faces(image_path):
         img = cv2.imread(image_path)
         faces = detector.detect_faces(img)

         if len(faces) == 0:
             raise ValueError("No face detected")
         elif len(faces) > 1:
             # 가장 큰 얼굴 선택
             faces = sorted(faces, key=lambda x: x['box'][2] * x['box'][3], reverse=True)

         return faces[0]
     ```
217. **얼굴 정렬 (Face alignment)** - 눈 수평 맞추기
     ```python
     import math

     def align_face(image_path, face_data):
         img = cv2.imread(image_path)
         keypoints = face_data['keypoints']

         # 두 눈 좌표
         left_eye = keypoints['left_eye']
         right_eye = keypoints['right_eye']

         # 각도 계산
         dY = right_eye[1] - left_eye[1]
         dX = right_eye[0] - left_eye[0]
         angle = math.degrees(math.atan2(dY, dX))

         # 회전
         center = ((left_eye[0] + right_eye[0]) // 2, (left_eye[1] + right_eye[1]) // 2)
         M = cv2.getRotationMatrix2D(center, angle, 1.0)
         aligned = cv2.warpAffine(img, M, (img.shape[1], img.shape[0]))

         cv2.imwrite(image_path, aligned)
     ```
218. **얼굴 자동 크롭** - 얼굴 중심으로 정사각형
     ```python
     def crop_face(image_path, face_data, padding=0.3):
         img = cv2.imread(image_path)
         x, y, w, h = face_data['box']

         # Padding 추가
         padding_w = int(w * padding)
         padding_h = int(h * padding)

         x1 = max(0, x - padding_w)
         y1 = max(0, y - padding_h)
         x2 = min(img.shape[1], x + w + padding_w)
         y2 = min(img.shape[0], y + h + padding_h)

         # 정사각형으로 만들기
         size = max(x2 - x1, y2 - y1)
         cx = (x1 + x2) // 2
         cy = (y1 + y2) // 2

         x1 = max(0, cx - size // 2)
         y1 = max(0, cy - size // 2)
         x2 = min(img.shape[1], x1 + size)
         y2 = min(img.shape[0], y1 + size)

         cropped = img[y1:y2, x1:x2]
         cv2.imwrite(image_path, cropped)
     ```
219. **얼굴 각도 추정 (Head pose estimation)** ⭐
     ```python
     import cv2
     import numpy as np

     def estimate_head_pose(image_path, face_landmarks):
         # 3D 모델 포인트
         model_points = np.array([
             (0.0, 0.0, 0.0),             # Nose tip
             (0.0, -330.0, -65.0),        # Chin
             (-225.0, 170.0, -135.0),     # Left eye left corner
             (225.0, 170.0, -135.0),      # Right eye right corner
             (-150.0, -150.0, -125.0),    # Left Mouth corner
             (150.0, -150.0, -125.0)      # Right mouth corner
         ])

         # 2D 이미지 포인트 (얼굴 랜드마크에서 추출)
         image_points = np.array([
             face_landmarks['nose_tip'],
             face_landmarks['chin'],
             face_landmarks['left_eye_left_corner'],
             face_landmarks['right_eye_right_corner'],
             face_landmarks['left_mouth_corner'],
             face_landmarks['right_mouth_corner']
         ], dtype="double")

         img = cv2.imread(image_path)
         size = img.shape
         focal_length = size[1]
         center = (size[1]/2, size[0]/2)
         camera_matrix = np.array([
             [focal_length, 0, center[0]],
             [0, focal_length, center[1]],
             [0, 0, 1]
         ], dtype="double")

         dist_coeffs = np.zeros((4,1))

         (success, rotation_vector, translation_vector) = cv2.solvePnP(
             model_points, image_points, camera_matrix, dist_coeffs
         )

         # Euler angles
         rotation_mat, _ = cv2.Rodrigues(rotation_vector)
         pose_mat = cv2.hconcat((rotation_mat, translation_vector))
         _, _, _, _, _, _, euler_angles = cv2.decomposeProjectionMatrix(pose_mat)

         pitch, yaw, roll = euler_angles.flatten()[:3]

         return {'pitch': pitch, 'yaw': yaw, 'roll': roll}
     ```
220. **얼굴 각도 검증** - Pitch/Yaw/Roll ±15도 이내 권장
     ```python
     def validate_head_pose(pose):
         MAX_ANGLE = 15  # degrees

         warnings = []
         if abs(pose['pitch']) > MAX_ANGLE:
             warnings.append(f"얼굴이 너무 {'위' if pose['pitch'] > 0 else '아래'}를 보고 있습니다 ({pose['pitch']:.1f}°)")

         if abs(pose['yaw']) > MAX_ANGLE:
             warnings.append(f"얼굴이 너무 {'왼쪽' if pose['yaw'] < 0 else '오른쪽'}으로 돌아가 있습니다 ({pose['yaw']:.1f}°)")

         if abs(pose['roll']) > 5:  # Roll은 더 엄격
             warnings.append(f"얼굴이 기울어져 있습니다 ({pose['roll']:.1f}°)")

         return warnings
     ```
221. **다중 얼굴 처리 UI** - "여러 얼굴이 감지되었습니다. 사용할 얼굴을 선택하세요"
222. **얼굴 미감지 처리** - "얼굴을 찾을 수 없습니다. 정면 사진을 업로드해주세요"
223. **얼굴 크기 검증** - 이미지의 최소 20% 차지해야 함
     ```python
     def validate_face_size(image_path, face_box):
         img = cv2.imread(image_path)
         img_area = img.shape[0] * img.shape[1]
         face_area = face_box[2] * face_box[3]

         face_ratio = face_area / img_area

         if face_ratio < 0.2:
             raise ValueError("얼굴이 너무 작습니다. 얼굴이 더 크게 보이도록 촬영해주세요")
         elif face_ratio > 0.9:
             raise ValueError("얼굴이 너무 큽니다. 약간 떨어져서 촬영해주세요")
     ```
224. **측면/후면 사진 거부** - Yaw > 30도
     ```python
     def reject_profile_photos(pose):
         if abs(pose['yaw']) > 30:
             raise ValueError("옆모습 사진은 사용할 수 없습니다. 정면 사진을 업로드해주세요")
     ```
225. **부적절한 이미지 필터링 (NSFW)** - 선택적
     ```python
     from nudenet import NudeDetector

     detector = NudeDetector()

     def check_nsfw(image_path):
         detections = detector.detect(image_path)
         for detection in detections:
             if detection['class'] in ['EXPOSED_GENITALIA', 'EXPOSED_BREAST']:
                 if detection['score'] > 0.6:
                     raise ValueError("부적절한 이미지입니다")
     ```
226. **Phase 2.3.2 얼굴 감지 테스트**
227. **Edge case 테스트** (안경, 마스크, 모자, 수염 등)
228. **다양한 인종/나이/성별 테스트**
229. **얼굴 감지 정확도 측정** (목표: >95%)
230. **실패 시 사용자 친화적 메시지 테스트**

#### 2.3.3: 음성 전처리 (231-235)
231. **음성 노이즈 제거 (RNNoise)**
     ```python
     import subprocess

     def remove_noise(input_path, output_path):
         subprocess.run([
             'rnnoise',
             input_path,
             output_path
         ])
     ```
232. **음량 정규화 (-23 LUFS)** - EBU R128 표준
     ```python
     import pyloudnorm as pyln

     def normalize_loudness(audio_path, target_loudness=-23.0):
         data, rate = sf.read(audio_path)

         # 현재 loudness 측정
         meter = pyln.Meter(rate)
         loudness = meter.integrated_loudness(data)

         # 정규화
         normalized = pyln.normalize.loudness(data, loudness, target_loudness)

         sf.write(audio_path, normalized, rate)
     ```
233. **클리핑 제거 및 soft clipping**
     ```python
     import numpy as np

     def remove_clipping(audio_data, threshold=0.95):
         # 클리핑 감지
         clipped = np.abs(audio_data) > threshold

         if clipped.any():
             # Soft clipping 적용
             audio_data = np.tanh(audio_data)

         return audio_data
     ```
234. **침묵 제거 (VAD - Voice Activity Detection)**
     ```python
     from webrtcvad import Vad

     def remove_silence(audio_path, aggressiveness=3):
         vad = Vad(aggressiveness)  # 0-3, 3이 가장 공격적

         data, rate = sf.read(audio_path)
         # VAD 적용하여 음성 구간만 추출
         # ... (구현 생략)
     ```
235. **Phase 2.3.3 음성 전처리 테스트**

### Phase 2.4: 입력 검증 종합 (236-250)
236. **이미지 검증 API** (/api/v1/validate/image)
     ```python
     @app.post("/api/v1/validate/image")
     async def validate_image(file: UploadFile):
         warnings = []
         errors = []

         # 1. 파일 타입 검증
         if not is_valid_image(file):
             errors.append("지원하지 않는 파일 형식입니다")

         # 2. 얼굴 감지
         try:
             faces = detect_faces(file)
             if len(faces) > 1:
                 warnings.append("여러 얼굴이 감지되었습니다")
         except ValueError as e:
             errors.append(str(e))

         # 3. 얼굴 각도 검증
         pose = estimate_head_pose(file, faces[0])
         pose_warnings = validate_head_pose(pose)
         warnings.extend(pose_warnings)

         # 4. 품질 체크
         quality_score = assess_image_quality(file)
         if quality_score < 0.5:
             warnings.append("이미지 품질이 낮습니다. 자동 개선을 권장합니다")

         return {
             "valid": len(errors) == 0,
             "errors": errors,
             "warnings": warnings,
             "suggestions": generate_suggestions(errors, warnings)
         }
     ```
237. **음성 검증 API** (/api/v1/validate/audio)
238. **검증 결과 UI 표시** (에러, 경고, 제안사항)
239. **자동 수정 제안**
     ```python
     def generate_suggestions(errors, warnings):
         suggestions = []

         if "얼굴을 찾을 수 없습니다" in errors:
             suggestions.append("밝은 곳에서 정면을 바라보고 촬영해주세요")
             suggestions.append("얼굴이 화면의 중앙에 오도록 해주세요")

         if any("각도" in w for w in warnings):
             suggestions.append("카메라를 눈높이에 맞춰주세요")
             suggestions.append("정면을 바라봐주세요")

         if "품질이 낮습니다" in warnings:
             suggestions.append("'자동 개선' 버튼을 클릭하세요")
             suggestions.append("더 밝은 환경에서 촬영해주세요")

         return suggestions
     ```
240. **실시간 검증 피드백** (업로드 중 미리보기)
241. **재촬영 가이드 UI**
     - 좋은 예시 사진 표시
     - 나쁜 예시 사진 표시
242. **검증 통과율 모니터링**
     ```python
     def track_validation_pass_rate():
         total = db.query(func.count(UploadAttempt.id)).scalar()
         passed = db.query(func.count(UploadAttempt.id)).filter(
             UploadAttempt.validation_passed == True
         ).scalar()

         pass_rate = passed / total if total > 0 else 0
         logger.info("validation_pass_rate", rate=pass_rate)
     ```
243. **실패 사유 분석**
     ```python
     def analyze_failure_reasons():
         failures = db.query(
             UploadAttempt.failure_reason,
             func.count(UploadAttempt.id).label('count')
         ).filter(
             UploadAttempt.validation_passed == False
         ).group_by(UploadAttempt.failure_reason).all()

         for reason, count in failures:
             logger.info("validation_failure", reason=reason, count=count)
     ```
244. **자동 개선 성공율 추적**
245. **Phase 2.4 검증 통합 테스트**
246. **1000+ 다양한 이미지 검증 테스트**
247. **사용자 경험 테스트** (실패 시 메시지 명확성)
248. **검증 성능 최적화** (처리 시간 <3초 목표)
249. **검증 API 문서화**
250. **Phase 2 전체 통합 테스트 및 문서화**

---

**(Part 1 계속...)**
