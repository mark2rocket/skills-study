# Claude Skills 워크플로우 자동화 학습 프로젝트

이 프로젝트는 Claude 스킬을 사용하여 개발 워크플로우를 자동화하는 방법을 학습하고 실습하기 위한 레포지토리입니다.

## 📁 프로젝트 구조

```
skills-study/
├── .claude/
│   └── skills/           # Claude 스킬 디렉토리
│       ├── README.md     # 스킬 사용 가이드
│       ├── code-review.md
│       ├── test-runner.md
│       ├── release-notes.md
│       ├── docs-generator.md
│       ├── issue-handler.md
│       └── ci-cd-helper.md
└── README.md
```

## 🎯 프로젝트 목적

Claude 스킬을 활용하여 다음과 같은 개발 워크플로우를 자동화하는 방법을 학습합니다:

- ✅ 자동 코드 리뷰
- ✅ 테스트 자동 실행 및 분석
- ✅ 릴리스 노트 자동 생성
- ✅ 문서 자동 생성
- ✅ 이슈 자동 처리
- ✅ CI/CD 파이프라인 관리

## 🚀 빠른 시작

### 1. 스킬 사용하기

Claude와 대화하면서 다음과 같이 스킬을 실행할 수 있습니다:

```
/code-review
/test-runner
/release-notes
```

### 2. 스킬 커스터마이징

`.claude/skills/` 디렉토리의 마크다운 파일을 수정하여 스킬을 커스터마이징할 수 있습니다.

### 3. 새로운 스킬 추가

`.claude/skills/` 디렉토리에 새 마크다운 파일을 추가하여 자신만의 스킬을 만들 수 있습니다.

## 📚 포함된 스킬

| 스킬 | 설명 | 사용법 |
|------|------|--------|
| **code-review** | 코드 변경사항 자동 리뷰 | `/code-review` |
| **test-runner** | 테스트 실행 및 분석 | `/test-runner` |
| **release-notes** | 릴리스 노트 생성 | `/release-notes` |
| **docs-generator** | 문서 자동 생성 | `/docs-generator` |
| **issue-handler** | 이슈 자동 처리 | `/issue-handler #123` |
| **ci-cd-helper** | CI/CD 설정 및 관리 | `/ci-cd-helper` |

## 📖 상세 가이드

각 스킬에 대한 자세한 사용 방법은 [.claude/skills/README.md](.claude/skills/README.md)를 참조하세요.

## 💡 학습 리소스

- [Claude Code 공식 문서](https://docs.claude.com/en/docs/claude-code)
- [스킬 작성 가이드](https://docs.claude.com/en/docs/claude-code/skills)

## 🔧 실습 예제

### 예제 1: 코드 리뷰 워크플로우

1. 코드 변경 후 `/code-review` 실행
2. 피드백 검토 및 수정
3. `/test-runner`로 테스트 확인

### 예제 2: 릴리스 준비

1. `/release-notes`로 변경사항 정리
2. `/docs-generator`로 문서 업데이트
3. `/ci-cd-helper`로 배포 파이프라인 확인

## 🤝 기여 방법

1. 새로운 스킬 아이디어가 있다면 추가해보세요
2. 기존 스킬을 개선해보세요
3. 유용한 워크플로우 예제를 공유해보세요

## 📝 노트

이 프로젝트는 학습 목적으로 만들어졌습니다. 실제 프로젝트에 적용하기 전에 각 스킬을 충분히 테스트하고 커스터마이징하세요.

---

**Happy Coding! 🎉**
