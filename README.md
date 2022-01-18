## ▶멜론99

<br>

# 전시어때 🖼

+ 웹개발종합반 5주차까지 듣고 복습할 겸 배운 기술들을 활용한 프로젝트를 계획
+ 멜론뮤직 탑100을 bs4와 requests를 이용해 스크래핑하여 제목과 가수, 순위를 추출하고, 그걸 가지고 셀레니움과 bs4를 가지고 유튜브 검색결과에서 썸네일, 유튜브 영상id번호, 플레이타임 등을 추출해서 들을 수 있는 사이트를 계획
+ 디자인은 원페이지로, cd플레이어를 재생하는 것처럼 줄을 당기면 플레이, 정지하고 리스트를 앨범처럼 볼 수 있고, 클릭하면 앨범을 클릭하면 해당 앨범 재생.
<br>

## ⏳프로젝트 기간
- 21년 12월 27일~31일

<br>


## 📺시연영상 링크

- 시연영상 링크
   <br> https://youtu.be/ZQfQkKi0pJk
   <br>


## 기술 스택

<br>

## 기능 소개
프로젝트를 진행하면서 시작하기 전에 api를 설계하고, 중요한 기능들이 안될까봐 기능 별로 조각내서 조각 코딩을 하고 합치는 방식으로 작업을 했음에도 불구하고, 계속 문제가 생겨서 구글링을 많이 했다. 예를 들어 유튜브 검색결과에서 첫번째 링크를 가져와서 노래를 재생시키려 했는데 1시간 연속재생이 있든가 해서 플레이타임이 10분이상이면 다음 링크를 가져온다든가, 또 재생목록을 불러왔을때 ajax가 비동기라 1~2초 정도 늦게 선언해둔 배열에 들어오길래, 페이지접속시 로딩화면을 만들어, 들어갔을 때 바로 불러온 상태로 보이게 한다든가 했다. 특히 비동기 문제랑 유튜브 api랑 겹쳐진 문제로, 이 부분에서 이틀을 잡아먹었다. 서버에 배포까지 하고싶었는데, 그건 또 로컬이 아닌 셀레니움을 우분투에서 크롤링하는 방법을 알아야해서 지금 막혔다. 우선은 크롤링이나 db, ajax통신 등을 연습했으니, 조별토이프로젝트를 진행해야겠다.
그리고 시간이 될 때 해놓은 코드에 주석을 달아봐야겠다.


----------------
사전팀프로젝트를 진행하면서, 로컬db의 콜렉션을 mongo compass를 이용해 json파일로 export하고, 그걸 파일질라를 이용해 ec2에 넣고 import해서 서버배포할 수 있단 걸 알게됨.
https://streamls.tistory.com/267   --- mongodb에서 json으로 export
https://webisfree.com/2017-07-30/mongodb-%EC%99%B8%EB%B6%80%ED%8C%8C%EC%9D%BC-import-export-%EB%B0%A9%EB%B2%95 -- json파일을 ec2로 mongodb에 import
https://www.jianshu.com/p/6fa450b356c8
이러면 우분투에서 셀레니움을 실행시킬 필요가 없다.
