# 릴리스 노트 자동 생성

이 스킬은 Git 커밋 히스토리를 분석하여 릴리스 노트를 자동으로 생성합니다.

## 작업 내용

1. 지정된 태그/커밋 범위의 변경사항 수집
2. 커밋 메시지 분석 및 분류:
   - ✨ Features (새로운 기능)
   - 🐛 Bug Fixes (버그 수정)
   - 📝 Documentation (문서)
   - 🎨 Refactoring (리팩토링)
   - ⚡️ Performance (성능 개선)
   - 🔒 Security (보안)
   - ⚠️ Breaking Changes (호환성 변경)
3. 릴리스 노트 생성:
   - 사용자 친화적인 설명
   - 영향받는 컴포넌트/기능
   - 마이그레이션 가이드 (필요시)

## 출력 형식

마크다운 형식으로 출력:
- 버전 번호
- 릴리스 날짜
- 주요 하이라이트
- 카테고리별 상세 변경사항
- 기여자 목록

## 사용 방법

최근 태그 이후 변경사항:

```
/release-notes
```

특정 범위:

```
/release-notes v1.0.0..v2.0.0
```

파일로 저장:

```
/release-notes --output CHANGELOG.md
```
