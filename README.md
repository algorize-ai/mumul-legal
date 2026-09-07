# mumul-legal

무물 수능의 이용약관과 개인정보처리방침을 공개하는 GitHub Pages 저장소입니다.

## 공개 URL 계약

다음 URL을 사용합니다.

- 현재 이용약관: `https://legal.justanswer.algorize-edu.com/terms/`
- 현재 개인정보처리방침: `https://legal.justanswer.algorize-edu.com/privacy/`
- 개인정보 국외이전: `https://legal.justanswer.algorize-edu.com/privacy/#cross-border-transfer`
- 계정 및 데이터 삭제: `https://legal.justanswer.algorize-edu.com/privacy/#account-deletion`
- 버전 목록: `https://legal.justanswer.algorize-edu.com/versions/`
- 첫 버전 이용약관: `https://legal.justanswer.algorize-edu.com/versions/2026-09-02/terms/`
- 첫 버전 개인정보처리방침: `https://legal.justanswer.algorize-edu.com/versions/2026-09-02/privacy/`

첫 production required version은 `2026-09-02`이며, 공고일과 시행일은 모두 `2026-09-07`입니다. 버전은 변경되지 않는 문서 식별자이며 공고일·시행일과 같을 필요는 없습니다.

현재 페이지와 해당 버전의 고정 페이지는 같은 본문과 날짜를 사용합니다. 각 페이지의 명시적 Jekyll `permalink`로 공개 경로를 고정합니다.

## 배포

GitHub Pages의 **Deploy from a branch** 방식으로 `main` 브랜치의 저장소 루트를 게시합니다. 별도 GitHub Actions workflow나 JavaScript 빌드는 사용하지 않습니다. Pages가 지원하는 Jekyll로 Markdown을 정적 HTML로 변환합니다.

법률 문서는 Markdown을 source of truth로 관리합니다. current 페이지는 최신 시행본으로 갱신할 수 있지만, 이미 공개한 `versions/<version>/` 문서는 덮어쓰지 않습니다. 중요한 내용이 바뀌면 서버의 required version도 올리고 앱에서 재동의를 받아야 합니다.

## 미확정 사항과 공개 확인

광고 국외이전의 수령자·국가·보유기간·법적 근거 등 기존 본문의 미확정 사항은 그대로 남아 있습니다. 문서 버전·공고일·시행일 확정이나 `draft: false`는 해당 사실관계 확인 또는 법률 검토 완료를 뜻하지 않습니다. 관련 안내를 공개 페이지에 유지합니다.

- 개인정보처리방침 제8조의 광고 계약·계정·파트너와 국외이전 미확정 사항 확인
- GitHub Pages custom domain과 HTTPS 강제 적용
- Route 53에서 `legal.justanswer.algorize-edu.com` CNAME 연결
- current URL, version URL, 두 anchor, 404, 모바일 표, 키보드 포커스 확인
- 앱과 스토어 콘솔에 canonical URL 반영
