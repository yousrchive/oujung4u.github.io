# oujung4u.github.io

## 목차
- [Final_Project](#Final_Project)


## Final_Project

모델 사용 영역

- 여행지 추천

- 챗봇 응답 (날씨, 관광지 정보, 교통)

1) 날씨

API or Crawling

크롤링 : https://www.weather.go.kr/w/weather/now.do

2) 관광지 정보 : 크롤링 (네이버)

3) 교통

[RESTAPI](#RESTAPI)


- 동행자 추천

데이터 소스

1) https://cafe.naver.com/momonme
(가입, 로그인 필요)

2) https://tripsoda.com/
(여행일정, 여행소개, 날짜, 나이, 인원 정보 모두 있음)

-> 제목, 날짜, 콘텐츠, 하이퍼링크 끌어오기
-> (input: 위치, 날짜, 성별, 나이) 제목/내용에서 유사도 검사 후 하이퍼링크 연결



### API, 모듈, 라이브러리

### RESTAPI

1. 공부 배경
VISITJEJU 제주도 공식 관광정보 포털에서 관광지 QnA 용도로 지식IN을 사용하고 있음 
https://www.visitjeju.net/kr/


2. 용도

1) 지식IN 

- 관광지 정보 - 관광지별로 하단에 노출

- 챗봇 교육에 사용 (**날씨**, 관광지 정보, 교통 별로 다른 API 사용)

3) 카페 - 동행자 구하기

→ 각각 다른 API를 사용하기 위해 궁금한 정보 미리 선택하게 하는 게 좋음

우려되는 점

1. 관광지와 유사도는 어떻게 파악?
2. 몇개 노출할 것?
3. 챗봇에서 미리 여행지를 설정하게 하고 물을 것?
4. 관광지가 구체화된 뒤 지식인을 사용해야 할 듯.
5. 충분한 질문들이 없었을 경우 html ?


4. 코드
[naver](C:\Users\Playdata\Desktop\수업\개인 공부\git\oujung4u.github.io\naver.ipynb) 


### 축제 정보

대한민국 전역 축제 정보 크롤링 사이트
1) 관광지 탭
2) 홈페이지 메인화면에 노출

https://www.mcst.go.kr/kor/s_culture/festival/festivalList.jsp

위치, 사진, 제목, 내용, 기간, 장소, 문의, 하이퍼링크, 요금 등
(컬럼: 개최지역, 개최기간, 축제성격, 관련누리집, 축제장소, 요금, 주최기관, 문의, 내용)
-> 위치별로 지도에 표시


### Receipt OCR

영수증에서 총 합계 찍어 올리면 날짜,시간 / 가게명 / 메뉴 / 총 금액 산출
(단순 n빵 or 메뉴별 n빵 다름)

레퍼런스:
https://learn.microsoft.com/ko-kr/azure/ai-services/computer-vision/overview-ocr
카카오 비전, 네이버 비전 있으나 유료
-> 전이학습 딥러닝 모델로 변경


