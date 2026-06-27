# 쇼핑 리스트 앱

한국어 IME를 지원하는 간단한 쇼핑 리스트 웹 앱입니다.

## 기능

- **아이템 추가** — 입력 후 버튼 클릭 또는 Enter 키
- **체크 완료** — 체크박스 클릭으로 완료 표시 (취소선)
- **개별 삭제** — × 버튼으로 아이템 삭제
- **완료 항목 일괄 삭제** — 체크된 항목 한 번에 삭제
- **자동 저장** — localStorage로 새로고침 후에도 목록 유지

## 사용 방법

별도 설치 없이 `index.html` 파일을 브라우저에서 열면 바로 사용할 수 있습니다.

## 기술 스택

- HTML5
- CSS3 (Flexbox, Custom Properties)
- Vanilla JavaScript (ES6+)
- Web Storage API (localStorage)

## 특이사항

- 한국어 IME 조합 중 Enter 키 이벤트 이중 발생 문제 처리 (`e.isComposing`)
- 시크릿 모드 등 localStorage 접근 불가 환경 대응 (`try/catch`)
- 접근성 고려 — 실제 `<input type="checkbox">` 사용 및 `aria-label` 적용
