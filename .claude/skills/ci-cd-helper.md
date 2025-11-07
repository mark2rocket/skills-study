# CI/CD 헬퍼

이 스킬은 CI/CD 파이프라인 설정과 문제 해결을 도와줍니다.

## 작업 내용

1. CI/CD 설정 파일 생성 및 관리:
   - GitHub Actions
   - GitLab CI
   - CircleCI
   - Jenkins
2. 빌드 실패 분석 및 해결
3. 배포 자동화 설정
4. 환경 변수 관리
5. 테스트 자동화 통합

## 지원하는 워크플로우

### 기본 CI 파이프라인
- Lint 검사
- 테스트 실행
- 빌드 검증
- 코드 커버리지

### CD 파이프라인
- 자동 배포
- 환경별 설정
- 롤백 전략
- 알림 설정

### 보안 검사
- 의존성 취약점 스캔
- 코드 보안 분석
- 시크릿 검사

## 사용 방법

새 CI/CD 설정 생성:

```
/ci-cd-helper --setup github-actions
```

빌드 실패 분석:

```
/ci-cd-helper --analyze-failure
```

특정 플랫폼 설정:

```
/ci-cd-helper --platform gitlab
```
