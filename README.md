# 집중 실험실 (6호)

성인용 2분 집중 게임 세 가지를 선택하는 정적 PWA입니다.

- **색 vs 글자:** 글자 뜻을 무시하고 글씨 색을 고르기. 매 문제는 뜻과 색이 다릅니다.
- **가운데 화살표:** 반대 방향을 가리키는 주변 화살표를 무시하고 가운데 방향을 고르기.
- **규칙 전환:** 매 4문제마다 글씨 색 ↔ 글자 뜻 규칙 변경. 화면의 현재 규칙을 확인합니다.

모두 정답·오답·정확도를 기록하며 오답이면 같은 문제를 다시 풀고, 각 게임의 최고 기록은 분리합니다. 이전 단순 시각 탐색 기록은 `focus6.history.v1`에서 삭제하지 않고 새 최고 기록에서는 제외합니다. 기존 게임 코드/화면/테스트는 `archive/visual-search-v1/`에 보존합니다. 인지 기능의 진단 또는 향상을 입증하는 앱이 아닙니다.

첫 온라인 방문 후 오프라인 재실행 가능. iPhone Safari 공유→홈 화면에 추가, Android Chrome 메뉴→홈 화면에 추가. 완료 기록은 이 기기의 브라우저 localStorage에만 저장되며 다른 기기와 동기화되지 않습니다. 브라우저 데이터 삭제 시 기록도 없어집니다.

로컬 실행: `python -m http.server 8786` 후 `http://localhost:8786/`. 테스트: `npm ci && npm test`.

게임 원리 참고: [APA Stroop](https://www.apa.org/research-practice/conduct-research/stroop-effect), [NIH Toolbox Flanker](https://nihtoolbox.org/test/flanker-inhibitory-control-and-attention-test-age-12/), [NIH Toolbox DCCS](https://nihtoolbox.org/test/dimensional-change-card-sort-test/). 공식 검사를 재현하거나 검증된 평가 점수를 산출하지는 않습니다.
