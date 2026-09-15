# mumul-legal

무물 수능의 이용약관과 개인정보처리방침을 관리하는 GitHub Pages 저장소입니다.

## 공개 URL

- 이용약관: `https://legal.justanswer.algorize-edu.com/terms/`
- 개인정보처리방침: `https://legal.justanswer.algorize-edu.com/privacy/`
- 개인정보 국외이전: `https://legal.justanswer.algorize-edu.com/privacy/#cross-border-transfer`
- 계정 및 데이터 삭제: `https://legal.justanswer.algorize-edu.com/privacy/#account-deletion`
- 문서 목록: `https://legal.justanswer.algorize-edu.com/versions/`
- 이용약관 사본: `https://legal.justanswer.algorize-edu.com/versions/2026-09-14/terms/`
- 개인정보처리방침 사본: `https://legal.justanswer.algorize-edu.com/versions/2026-09-14/privacy/`

## 현재 문서 상태

문서 식별자는 `2026-09-14`로 통일한다. 사용자 요청에 따라 시행일은 `2026-09-16`로 지정했다. 공고일은 사용자 요청에 따라 `2026-09-16`으로 지정했으며 현재 본문은 검토 중인 개정안이다. 시행일 지정은 최종 확정, 해당 날짜의 공고·배포 또는 이용자 동의가 완료되었다는 뜻이 아니다.

사용자 확인에 따라 배포 테스트용 과거 문서와 중복 초안은 정리했다. 과거 게시본은 Git 커밋 `bef2daf`에 보존돼 있다. 현재 페이지와 식별자별 사본은 permalink를 제외한 본문과 메타데이터가 같아야 한다.

공개 본문에 문서 식별자를 별도로 표시할 필요는 없다. `policy_version`과 서버 동의 기록의 버전은 별개로 관리하며, 이 저장소의 변경만으로 서버 데이터가 갱신되지는 않는다.

## 공개 전 남은 작업

- 두 문서에서 내부 검토 메모와 코드 설정 설명을 분리하고 이용자용 문장으로 정리한다.
- 실제 AI 제공사와 광고 계약·계정·파트너 설정을 확인해 수령자, 국가, 항목, 목적, 보유기간, 거부 절차와 법적 근거를 확정한다. 미확정 사실을 단순 삭제하거나 추정값으로 대체하지 않는다.
- 삭제 경로, 보관·파기 정책, 연령 조건을 실제 출시 구성과 대조한다.
- 이번 문서는 사용자 결정에 따라 광고 포함 초안으로 유지한다. 확정된 광고 정보 비수집·학습 정보 미전달·Google 공개 보유 기준은 반영하고, 미확정 광고 처리 항목은 남겨둔다. 광고 플랫폼은 Google AdMob만 사용하고 추가 미디에이션·Firebase Analytics는 사용하지 않기로 했다. 보상형 광고는 시청 조건 완료 시 보상을 제공한다고 안내하며, 약관에 보상의 종류·수량이나 보상 미정 문구를 넣지 않는다. 구체적인 보상과 조건은 실제 광고 표시 전 앱에서 안내해야 한다. 공고일은 `2026-09-16`, 시행일은 `2026-09-16`로 지정했다. 본문 확정 후 공개 화면의 개정안 안내를 정리하며, 지정일을 실제 배포·동의 완료의 증거로 취급하지 않는다.
- 서버 필수 약관 버전과 문서 URL, 앱의 동의 안내를 일치시킨다. 기존 동의 기록을 일괄 덮어쓰지 않는다.
- 메인 페이지, 문서 목록, 두 본문과 사본, 국외이전·삭제 anchor, 모바일 표와 키보드 포커스를 확인한다.

## 배포

GitHub Pages의 **Deploy from a branch** 방식으로 `main` 브랜치의 저장소 루트를 게시한다. Pages가 지원하는 Jekyll로 Markdown을 HTML로 변환한다. README는 `_config.yml`의 exclude 설정으로 사이트 게시 대상에서 제외한다. 공개 Git 저장소 자체에서 README 접근을 차단하는 설정은 아니다.

미시행 문서를 시행본으로 확정하지 않은 상태에서 버전 정리만으로 배포 완료라고 판단하지 않는다. 실제 배포 후 current URL, 사본 URL, 두 anchor와 HTTPS를 확인한다.
