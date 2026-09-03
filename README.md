# mumul-legal

무물 수능의 이용약관과 개인정보처리방침을 공개하는 GitHub Pages 저장소입니다.

## 공개 URL 계약

custom domain 연결 후 다음 URL을 사용합니다.

- 현재 이용약관: `https://legal.justanswer.algorize-edu.com/terms/`
- 현재 개인정보처리방침: `https://legal.justanswer.algorize-edu.com/privacy/`
- 개인정보 국외이전: `https://legal.justanswer.algorize-edu.com/privacy/#cross-border-transfer`
- 계정 및 데이터 삭제: `https://legal.justanswer.algorize-edu.com/privacy/#account-deletion`
- 버전 목록: `https://legal.justanswer.algorize-edu.com/versions/`
- 향후 버전별 이용약관: `https://legal.justanswer.algorize-edu.com/versions/<version>/terms/`
- 향후 버전별 개인정보처리방침: `https://legal.justanswer.algorize-edu.com/versions/<version>/privacy/`

`<version>`은 공고일과 시행일을 확정한 시행본의 변경되지 않는 식별자입니다. 현재의 `draft-2026-09-02`는 production required version으로 사용하지 않습니다.

## 배포

GitHub Pages의 **Deploy from a branch** 방식으로 `main` 브랜치의 저장소 루트를 게시합니다. 별도 GitHub Actions workflow나 JavaScript 빌드는 사용하지 않습니다. Pages가 지원하는 Jekyll로 Markdown을 정적 HTML로 변환합니다.

법률 문서는 Markdown을 source of truth로 관리합니다. current 페이지는 최신 시행본으로 갱신할 수 있지만, 이미 공개한 `versions/<version>/` 문서는 덮어쓰지 않습니다. 중요한 내용이 바뀌면 서버의 required version도 올리고 앱에서 재동의를 받아야 합니다.

## 출시 전 체크

- 문서의 production version, 공고일, 시행일 확정
- 시행본을 `versions/<version>/`에 고정 보관
- `draft: false`로 변경하고 초안 경고 문구 제거
- GitHub Pages custom domain과 HTTPS 강제 적용
- Route 53에서 `legal.justanswer.algorize-edu.com` CNAME 연결
- current URL, version URL, 두 anchor, 404, 모바일 표, 키보드 포커스 확인
- 앱과 스토어 콘솔에 canonical URL 반영
