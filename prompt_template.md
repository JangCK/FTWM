FTWM Prompt Template (프롬프트 템플릿)

사용법: 아래 필드에 맞춰 입력하면 AI가 FTWM 워크플로우에 따라 설계를 생성합니다.

템플릿 필드:
- Purpose: (예: 설득형 에세이, 기술 문서, 소설 플롯)
- Adapter: (Core | Essay | Academic | NovelPlotting | Hybrid | Series)
- ReaderProfile:
  - Expertise: 1-5
  - Affinity: 1-5
  - Attention: 1-5
- TargetLength: 글자수 목표 (예: 3000)
- Constraints: (금지·필수 사항)
- Notes: 추가 맥락

요청 포맷(예시):
```
Purpose: 설득형 에세이
Adapter: Essay
ReaderProfile:
  Expertise: 3
  Affinity: 4
  Attention: 3
TargetLength: 3000
Constraints: 은유는 적절히 사용, 통계 1개 포함
Notes: 주제는 '원격 근무의 장단점'
```

AI 역할(간략):
1) ReaderProfile 검증 및 Width 코드 추천
2) 노드 트리(Mapping) 및 MECE 검증
3) Weight 맵(총합 100) 및 글자수 환산
4) Depth 목표(D1-D5)와 구체성 검증 규칙 적용
5) Peak 초안 2~3개([Draft] 태그 포함) 및 E4-COLLAB 표기
6) Texture 맵과 샘플 문장
7) Contour 요약(경사, 브릿지, 호흡점)
8) 간단한 Diagnostics 체크리스트 출력

출력 형식: Markdown 섹션으로 단계별 결과 제공
