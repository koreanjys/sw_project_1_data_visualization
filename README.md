# `데이터 시각화 프로젝트`
- 개요: 데이터프레임을 그래프 등으로 시각화하는 프로젝트
- 기간: 2023-02-15 ~ 2023-03-09

## `주제: 뉴스 헤드라인과 주가의 상관관계 분석`

## `PASS 조`

- 조장 : 신주용 : 주가, 뉴스 헤드라인 크롤링 및 전처리
- 조원 : 송재원 : 뉴스 헤드라인 워드클라우드, 주가 데이터 시각화
- 허우영 : 주가 데이터 시각화
- 윤지현 : 주가 데이터 크롤링

## `주제 선정`

- 뉴스 헤드라인에 따른 주가 변동이 궁금했다. 다른 데이터는 제외하고 순수 헤드라인과 주가와 비교를 해봤다.

## `프로젝트 단계`

1. 주제 선정
2. 주가, 뉴스 헤드라인 크롤링
3. 데이터 전처리
4. 그래프와 워드클라우드 시각화
5. 시각화 비교분석

## `크롤링`

- 사용한 라이브러리 : requests, bs4, selenium
- 크롤링 한 url : 네이버, 구글

## `전처리`

- pandas로 크롤링 한 데이터들의 양식을 하나로 통일

## `시각화`

- 주가 데이터 시각화 : PowerBI
- 뉴스 헤드라인 시각화 : WordCloud

## `시각화 분석 결과`

- 워드클라우드만으로는 헤드라인이 주가 변동에 영향을 얼마나 미치는지 직관적으로 보기 어려웠다.

## `시행착오`

1. 구글 크롤링을 하다가 reCAPTCHA가 걸렸다. 해결 방법으로는 User-agent를 추가해서 식별 정보를 줘야했다.
2. 워드클라우드 로딩 렉. 원인은 전처리를 제대로 하지 않아 너무 많은 데이터를 읽다가 멈췄다.
3. 워드클라우드만으로는 비교 분석이 어려워서 자연어 처리로 헤드라인 내용을 점수화 하고 그래프로 시각화를 시도해 보았지만, 아직 배워보지 못했던 기술을 억지로 쓰다보니, 전혀 효과가 없었다.
