# Claude Skills - 워크플로우 자동화 가이드

이 디렉토리에는 개발 및 마케팅 워크플로우를 자동화하기 위한 Claude 스킬들이 포함되어 있습니다.

## 📚 스킬 목록

### 🧑‍💻 개발자용 스킬

#### 1. 코드 리뷰 (`code-review.md`)
자동으로 코드 변경사항을 리뷰하고 피드백을 제공합니다.
- 코드 품질 검사
- 보안 취약점 탐지
- 성능 이슈 식별
- 개선 제안 제공

**사용법:** `/code-review` 또는 `/code-review [파일경로]`

#### 2. 테스트 자동 실행 (`test-runner.md`)
프로젝트의 테스트를 실행하고 결과를 분석합니다.
- 자동 테스트 실행
- 실패 원인 분석
- 자동 수정 옵션

**사용법:** `/test-runner` 또는 `/test-runner --fix`

#### 3. 릴리스 노트 생성 (`release-notes.md`)
Git 커밋 히스토리를 분석하여 릴리스 노트를 자동 생성합니다.
- 커밋 분류 (기능, 버그 수정, 문서 등)
- 마크다운 형식 출력
- CHANGELOG 파일 생성

**사용법:** `/release-notes` 또는 `/release-notes v1.0.0..v2.0.0`

#### 4. 문서 자동 생성 (`docs-generator.md`)
코드베이스를 분석하여 자동으로 문서를 생성합니다.
- API 문서
- 컴포넌트 문서
- 개발자 가이드

**사용법:** `/docs-generator` 또는 `/docs-generator --type api`

#### 5. 이슈 처리 (`issue-handler.md`)
GitHub 이슈를 분석하고 자동으로 처리합니다.
- 버그 재현 및 분석
- 기능 요청 구현 계획
- 자동 수정

**사용법:** `/issue-handler #123` 또는 `/issue-handler #123 --fix`

#### 6. CI/CD 헬퍼 (`ci-cd-helper.md`)
CI/CD 파이프라인 설정과 문제 해결을 도와줍니다.
- CI/CD 설정 생성
- 빌드 실패 분석
- 보안 검사

**사용법:** `/ci-cd-helper --setup github-actions`

---

### 📱 마케터용 스킬

#### 1. 콘텐츠 생성기 (`content-creator.md`)
다양한 마케팅 콘텐츠를 자동으로 생성합니다.
- 블로그 포스트, 소셜 미디어, 이메일
- 타겟 오디언스별 맞춤 콘텐츠
- A/B 테스트 버전 제공
- 해시태그 및 CTA 제안

**사용법:** `/content-creator` 또는 `"Instagram 포스트 3개 만들어줘"`

#### 2. SEO 최적화 (`seo-optimizer.md`)
콘텐츠의 SEO를 분석하고 최적화합니다.
- 키워드 리서치 및 분석
- 온페이지 SEO 최적화
- 경쟁사 키워드 분석
- 메타 태그 및 구조 개선

**사용법:** `/seo-optimizer` 또는 `/seo-optimizer --keyword-research`

#### 3. 소셜 미디어 매니저 (`social-media-manager.md`)
소셜 미디어 콘텐츠 기획 및 일정 관리를 도와줍니다.
- 월간/주간 콘텐츠 캘린더 생성
- 플랫폼별 최적화 (Instagram, LinkedIn, Twitter, Facebook 등)
- 해시태그 전략
- 최적 포스팅 시간 추천

**사용법:** `/social-media-manager` 또는 `"11월 콘텐츠 캘린더 만들어줘"`

#### 4. 마케팅 분석 (`marketing-analytics.md`)
마케팅 데이터를 분석하고 인사이트 기반 리포트를 생성합니다.
- 트래픽 및 전환율 분석
- 채널별 성과 분석
- ROI 및 ROAS 계산
- 액션 아이템 제시

**사용법:** `/marketing-analytics` 또는 `"지난 달 성과 리포트 작성해줘"`

#### 5. 카피라이터 (`copywriter.md`)
효과적인 마케팅 카피를 작성합니다.
- 광고 헤드라인, CTA, 제품 설명
- AIDA, PAS 등 카피라이팅 프레임워크
- 설득 기법 적용
- A/B 테스트 버전 제공

**사용법:** `/copywriter` 또는 `"랜딩 페이지 카피 작성해줘"`

#### 6. 경쟁사 분석 (`competitor-analyzer.md`)
경쟁사를 분석하여 마케팅 전략 수립을 지원합니다.
- 다차원 경쟁사 분석
- SWOT 분석
- 벤치마킹 및 비교
- 차별화 전략 제안

**사용법:** `/competitor-analyzer` 또는 `"주요 경쟁사 분석해줘"`

## 🚀 시작하기

### 스킬 사용 방법

1. **Slash 명령어로 실행**
   ```
   /[스킬이름]
   ```

2. **직접 참조**
   Claude에게 스킬 파일을 참조하도록 요청:
   ```
   "code-review.md 스킬을 사용해서 내 코드를 검토해줘"
   ```

### 스킬 커스터마이징

각 스킬은 마크다운 파일로 작성되어 있어 쉽게 수정할 수 있습니다:

1. `.claude/skills/[스킬이름].md` 파일 열기
2. 작업 내용, 출력 형식, 또는 사용 방법 수정
3. 저장 후 바로 사용 가능

## 💡 스킬 작성 가이드

### 기본 구조

```markdown
# 스킬 제목

스킬에 대한 간단한 설명

## 작업 내용

1. 수행할 작업 1
2. 수행할 작업 2
3. ...

## 출력 형식

결과를 어떤 형식으로 출력할지 설명

## 사용 방법

사용 예시 제공
```

### 좋은 스킬 작성 팁

1. **명확한 목적**: 스킬이 정확히 무엇을 하는지 명시
2. **구체적인 단계**: 수행할 작업을 단계별로 상세히 기술
3. **출력 형식 정의**: 결과물의 형식을 명확히 지정
4. **사용 예시**: 다양한 사용 시나리오 제공
5. **파라미터 설명**: 필요한 입력값과 옵션 설명

### 새로운 스킬 만들기

1. `.claude/skills/` 디렉토리에 새 마크다운 파일 생성
2. 위의 기본 구조를 따라 작성
3. Claude와 대화에서 바로 사용 가능

**예시:**
```bash
# .claude/skills/my-custom-skill.md 파일 생성
```

## 🔧 고급 기능

### 조건부 실행

스킬 내에서 조건을 지정할 수 있습니다:

```markdown
## 작업 내용

1. package.json 파일이 있는 경우:
   - npm 프로젝트로 처리
2. 그렇지 않은 경우:
   - Python 프로젝트로 처리
```

### 다른 스킬 참조

스킬 내에서 다른 스킬을 참조할 수 있습니다:

```markdown
## 작업 내용

1. 먼저 `/test-runner`를 실행하여 테스트 통과 확인
2. 테스트 통과 시 `/release-notes` 생성
```

### 외부 도구 통합

Bash 명령어나 다른 도구를 스킬에 통합:

```markdown
## 작업 내용

1. `npm run lint` 실행
2. `prettier --check .` 실행
3. 결과 분석 및 리포트 생성
```

## 📋 워크플로우 예시

### 🧑‍💻 개발 워크플로우

#### 배포 전 체크리스트

```bash
# 1. 코드 리뷰
/code-review

# 2. 테스트 실행
/test-runner

# 3. 문서 업데이트
/docs-generator

# 4. 릴리스 노트 생성
/release-notes --output CHANGELOG.md

# 5. CI/CD 설정 확인
/ci-cd-helper --analyze-failure
```

#### 버그 수정 워크플로우

```bash
# 1. 이슈 분석
/issue-handler #123

# 2. 수정 후 코드 리뷰
/code-review

# 3. 테스트 실행
/test-runner --fix
```

### 📱 마케팅 워크플로우

#### 콘텐츠 마케팅 캠페인

```bash
# 1. 경쟁사 분석
/competitor-analyzer

# 2. SEO 키워드 리서치
/seo-optimizer --keyword-research

# 3. 블로그 콘텐츠 생성
/content-creator

# 4. SEO 최적화
/seo-optimizer

# 5. 소셜 미디어 포스트 제작
/social-media-manager
```

#### 제품 런칭 캠페인

```bash
# 1. 랜딩 페이지 카피 작성
/copywriter

# 2. 소셜 미디어 캘린더 생성
/social-media-manager

# 3. 이메일 마케팅 콘텐츠
/content-creator

# 4. 성과 분석 대시보드 준비
/marketing-analytics
```

#### 월간 마케팅 리뷰

```bash
# 1. 성과 리포트 생성
/marketing-analytics

# 2. 경쟁사 벤치마킹
/competitor-analyzer --benchmark

# 3. SEO 순위 체크
/seo-optimizer

# 4. 다음 달 콘텐츠 계획
/social-media-manager
```

## 🤝 기여하기

새로운 스킬을 추가하거나 기존 스킬을 개선하려면:

1. 새 스킬 파일 생성 또는 기존 파일 수정
2. 이 README에 스킬 정보 추가
3. 변경사항 커밋 및 푸시

## 📖 추가 리소스

- [Claude Code 공식 문서](https://docs.claude.com/en/docs/claude-code)
- [스킬 작성 가이드](https://docs.claude.com/en/docs/claude-code/skills)

## 🎯 팁과 트릭

1. **스킬 체이닝**: 여러 스킬을 순차적으로 실행하여 복잡한 워크플로우 구성
2. **컨텍스트 제공**: 스킬 실행 시 구체적인 컨텍스트를 제공하면 더 정확한 결과
3. **반복 개선**: 스킬을 사용하면서 계속 개선하고 커스터마이징
4. **팀과 공유**: 팀원들과 유용한 스킬을 공유하여 생산성 향상

---

**질문이나 제안사항이 있으시면 언제든지 Claude에게 물어보세요!**
