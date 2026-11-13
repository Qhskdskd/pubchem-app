# 약물 특성 조회 (PubChem)

PubChem 공식 API로 약물의 물리화학적 특성과 GHS 분류를 조회하는 단일 HTML 앱입니다.

- **PUG REST**: 이름 → CID, 분자식·분자량·XLogP·TPSA·SMILES 등
- **PUG View**: `GHS Classification` 섹션만 (출처 기관별 신호어, H/P 코드, 그림문자)
- 요청 간격 220ms 이상 → 초당 5회 제한 준수
- 각 섹션에 출처 API URL 표시

## 실행
`index.html`을 브라우저로 열거나:

```
python -m http.server 8000
```
→ http://localhost:8000

약물 이름은 영문으로 입력하세요 (예: ibuprofen).

## 데이터 출처
[PubChem](https://pubchem.ncbi.nlm.nih.gov/) (NCBI/NLM). GHS 정보는 ECHA, NITE 등 각 제공 기관의 자료입니다.
