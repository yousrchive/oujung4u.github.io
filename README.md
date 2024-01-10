# oujung4u.github.io
a hub for storing self-developing history

## 목차
- [Final_Project](#Final_Project)


## Final_Project

### RESTAPI

1. 공부 배경
VISITJEJU 제주도 공식 관광정보 포털에서 관광지 QnA 용도로 지식IN을 사용하고 있음 
https://www.visitjeju.net/kr/



1) 관광지 정보 - 관광지별로 하단에 노출

2) 챗봇 교육에 사용 (**날씨**, 관광지 정보, 교통 별로 다른 API 사용)

3) 카페 - 동행자 구하기

→ 각각 다른 API를 사용하기 위해 궁금한 정보 미리 선택하게 하는 게 좋음

우려되는 점

1. 관광지와 유사도는 어떻게 파악?
2. 몇개 노출할 것?
3. 챗봇에서 미리 여행지를 설정하게 하고 물을 것?
4. 관광지가 구체화된 뒤 지식인을 사용해야 할 듯.
5. 충분한 질문들이 없었을 경우 html ?

→ 챗봇 서비스 이용 시 용도 구체화해두는 게 나을까


3) 동행자 구하기

https://cafe.naver.com/momonme
(가입, 로그인 필요)

https://tripsoda.com/
(여행일정, 여행소개, 날짜, 나이, 인원 정보 모두 있음)

-> 제목, 날짜, 콘텐츠, 하이퍼링크 끌어오기
-> (input: 위치, 날짜, 성별, 나이) 제목/내용에서 유사도 검사 후 노출


### 날씨API
날씨 정보 api:

(단위 설정)

https://doubled.tistory.com/20


- **웨더아이(유료)**

https://www.weatheri.co.kr/index.php

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/8ddf4b50-d1fc-4ff5-89a1-addcbdaf1465/dcc5db65-dfe9-4d6d-8586-1f5301b43d6b/Untitled.png)

https://topis.seoul.go.kr/refRoom/openRefRoom_4.do

- 오픈웨더맵 (무료, 해외 사잍)

https://openweathermap.org/api


### 크롤링

대한민국 전역 축제 정보 크롤링 사이트 → 관광지 탭 / 홈페이지 메인화면에 노출

https://www.mcst.go.kr/kor/s_culture/festival/festivalList.jsp




### Microsoft Azure AI vision

영수증에서 총 합계 찍어 올리면 날짜,시간 / 가게명 / 메뉴 / 총 금액 산출
(단순 n빵 or 메뉴별 n빵 다름)

레퍼런스:
https://learn.microsoft.com/ko-kr/azure/ai-services/computer-vision/overview-ocr