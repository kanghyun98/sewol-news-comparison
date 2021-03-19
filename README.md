# 세월호 참사 신문사별 보도 방식 비교 분석



## 1. 소개

대표적인 진보, 보수 성향을 띄는 두 신문사의 4월 16일부터 4월 30일까지의 2주간 기사 본문을 분석, 비교하여 두 신문사의 세월호 관련 기사 보도 특성에 대해 비교 분석하였습니다.





## 2. 목적

- 선행된 연구에 따르면 신문사별로 세월호 기사 보도방식에 차이가 존재한다합니다. 해당 신문사별 기사 본문들을 이용하여 본문 내 명사들을 추출, 시각화 후 성향 차이를 직접 확인했습니다.

- 숭실대학교 정보통계보험수리학과 주관 빅데이터 경진대회 참여 및 전산통계 강의 내용 응용을 목적으로 하였습니다.





## 3. 방법

방법은 아래와 같습니다.

- 4월 16일부터 4월 30일을 기간으로 <세월호>를 검색했을 때 나오는 조선일보 기사 846개, 한겨레 기사 892개 기사를 사용

- R을 통해 링크 안의 기사 본문들을 크롤링 및 전처리하여 목적에 맞게 데이터 파일들을 생성
- 위 데이터 파일들을 이용해 각 신문사의 단어 출현빈도(4/16~20)와 주요 선별 단어들의 출현빈도(4/16~30)를 날짜별 비교와 전체 비교를 실시 (총 4개). 
- 추가적으로 각 신문사의 2주간 모든 단어 출현빈도를 종합 후 연관성 분석 실시

*자세한 내용은 위의 <u>Sewol.R</u>과 <u>세월호참사뉴스비교분석.hwp</u>을 참고 부탁드립니다.*





## 4. 결론

한겨레와 조선일보 간에는 명확한 성향 차이가 보였습니다. 5일간의 흐름은, 5일간 구조상황에 맞춰 자세한 내용이 매일 보도가 됐으며, 구조 -> 사고중점보도 -> 진상규명(한겨레) or 기타관련이슈(조선일보, e.g. 연예계) 흐름을 보였습니다.

*자세한 내용은 위의 <u>세월호참사뉴스비교분석.hwp</u>을 참고 부탁드립니다.*





## 5. 어려움

- 두 신문사의 보도방식의 차이를 볼 수 있는 기사 수를 선정하는 데에 있어서 분석자의 주관이 들어갔다는 한계가 있었습니다. 또한 5일간의 흐름 분석에서 보다 명확한 흐름을 보이지 못했다는 아쉬움이 있고, 워드클라우드를 이용한 시각화에서는 신문사 별의 보도방식 차이를 명확히 보이지 못했단 아쉬웠습니다.

- 단어사전을 사용할 때, 분석자들이 단어를 사전에 미리 추가하는 부분 또한 주관과 부족함이 있었t습니다. 더불어 한글을 텍스트마이닝할 때 형태소를 정확히 분석하여 명사와 어조사를 분리할 필요가 있고, 관련 함수인 SimplePos09, SimplePOS22 등의 사용법이 있었으나 구현해내지 못했습니다. 





## 6. 빅데이터 분석 경진대회 결과

2020년 12월 18일 Zoom 회의를 통해 빅데이터 분석 경진대회가 진행되었으며, *정보통계보험수리학과 17학번 김민우*와 함께 참가하여 우수상을 수상하였다.