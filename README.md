# Projects in the Real World (ORDER BY END_DATE DESC)
[1] 연구 중심 병원 플랫폼 개발
>테크 스택: React.js, Typescript, Vue.js, Node.js, PostgreSQL, DynamoDB
프로젝트 기간: 2020.01~Present
Serverless package를 이용해서 API Gateway, Lambda를 개발함으로써 서버리스 아키텍쳐를 구현했습니다.
이 밖에 Cognito(회원 인증 서비스)와 SES(이메일 서비스), S3(웹사이트 호스팅/이미지 저장), Cloudfront(Cache), Route 53(DNS) 등의 서비스들을 사용했습니다.
프로젝트들을 필터링하거나 정렬할때는 PostgreSQL을 사용했고 프로젝트의 상세내용의 대한 정보는 DynamoDB를 이용해서 보여줍니다.
MobX와 Context API를 사용해서 여러 컴포넌트들에서 State를 관리하도록 개발했습니다.
이 서비스는 대중성을 위한 웹사이트가 아닌 협약을 한 병원들만 사용할 수 있으며 현재는 세종 병원과 분당 서울대 병원이 협약을 했습니다. 그렇기 때문에 포트폴리오로 공개하기가 힘든 제약 사항이 있습니다.
아주대학교 의료 원장님 앞에서 직접 저 본인이 웹어플리케이션 사용 시연을 할 정도로 꽤 스케일이 큰 프로젝트입니다.



[2] Covid19 Research Platform (코로나 연구 분석 플랫폼 개발)
>건강보험심사평가원의 빅데이터를 개방하여 여러 나라에서도 심평원의 데이터를 기반으로 연구 및 분석을 할 수 있게 해주고 코로나19 국제협력 연구에 발전을 위해 만들어진 플랫폼입니다.
보건복지부도 연관되어 있고 기사도 여러개 날 만큼 꽤 큰 이벤트 였습니다.
4일이라는 짧은 기간안에 플랫폼을 개발해야해서 [1]에서 개발한 프로젝트를 클론받아서 수정해서 배포했습니다.
 
[3] OHDSI Korea International Symposium (AWS DevOps)
>포트폴리오는 없고 뉴스 기사만 있어서 링크를 걸었습니다.
OHDSI (Observational Health Data Sciences and Informatics)는 국제 의료 정보 협회라고 보시면 되고 이 협회에서는 의료 정보 분석을 쉽게 할 수 있도록 Open Source 분석 도구 웹사이트 (Atlas, Achilles, Athena)를 제공합니다.
2019년 12월 12일부터 14일간의 행사를 진행했었고 약 한 달반 정도의 기간 동안 준비를 했었습니다. 이 행사에서는 분석 도구를 어떻게 돌리는지 데모를 하고 여러 나라에서 온 참가자들이 직접 한 번씩 분석 도구를 돌려보는 세션들이 있었습니다.
여기서 제가 맡은 의무는 Open Source 분석도구인 Atlas를 github에 제공되어 있는 CloudFormation (Terraform과 비슷한) 파일을 이용해서 웹서버 배포를 하고 아주대학교 데이터를 AWS OLAP DB인 Redshift라는 DB에 넣었습니다. 그리고, 다른 연구원들에게 부탁해서 같이 Stress Test를 하면서 컴퓨팅 파워 스펙과 Redshift의 노드수를 Optimizing 했습니다.
다행히 행사는 무사히 마무리 되었습니다. 이 행사에서 제가 보여준 활약으로 수습기간이였던 제가 아주대학교에서 계속 일할 수 있게 되었습니다.
 
[4] Smart Exhibition (전시회 웹사이트 개발)
>테크 스택: React.js, Node.js, MongoDB
프로젝트 기간: 2019.06~2019.10
Redux를 사용해서 여러 Component들 사이에서 State를 관리함
API 서버는 AWS ECS (Elastic Container Service)에서 호스팅
Authentication은 MiddleWare에 JWT 토큰을 검증하는 방식
Real Time Notification (Socket.io) 알림 서비스를 개발해서 새로운 회원이 생길때 실시간으로 어드민에서 확인할 수 있게 만듬
MongoDB의 스토리지는 EFS (Elastic File System)에 Mounting해서 3개의 가용 영역에서 사용할 수 있게함
 
[5] Meiyan Project (화장품 E-Commerce 플랫폼 개발)
>테크 스택: Vue.js, Node.js, DynamoDB
프로젝트 기간: 2018.12~2019.04
AWS 신기술인 aws-amplify/cli 이용해서 서비스 개발
AllPay PG사를 이용한 중국 결제시스템 연동 (알리페이, 위챗페이 연동)
python web scraping (BeautifulSoup)를 이용한 연관된 화장품 이름, 가격을 한눈에 볼수있게 도와주는 back-office software 개발

# Projects for Portfolio (ORDER BY END_DATE DESC)

[1] PHP (Restful API)
>Capstone project로 진행한 과제입니다. 저희 팀의 클라이언트가 도자기 공방을 하고 사람들을 가르치는 일을하시는데, 제가 맡은 임무는 Customer Booking Integration으로 (클라이언트의) 고객이 Occasion 이라는 다른 외부 웹사이트 API를 통해서 결제를하고 테이블을 부킹하면 Wordpress로 운영된 저희 고객사이트에 가입이 되어있지않으면 가입을 시키고 Vend라는 매출관리하는 사이트에 고객 정보를 입력하고 주문번호를 입력해서 클라이언트가 한 달에 얼마나 벌었는지 어떤 고객이 제일 많이 소비를 했는지를 알려줍니다.    
데모 영상: https://www.youtube.com/watch?v=sN0Y4nAWcyM
클라이언트 사이트: https://colourmypot.com/ 

[2] Blockchain - Language/IDE/Server: Solidity/Remix/Ganache Cli. 
>이더리움을 이용한 블록체인은 개인적으로 제가 최근에 관심을 가지게된 분야입니다. 방학때 유튜브로 영상만 찾아보다가 저도 직접 한 번 만들어보고 싶어서 stackoverflow랑 각종 references 등을 보고 solidity, web3.js, Ganache Cli를 이용해서 Dapp_ex1이랑 Dapp_ex2를 저 혼자만의 색깔로 만들었습니다. Dapp_ex1은 부동산 거래내역등을 기록할때 함부로 누가 바꾸지 못하도록 블록체인이 적용되었으면 하는 바람에 만들었고 Dapp_ex2는 오는 2021년은 굳이 밖에 나가지않고 집에서 대통령 선거를 하는 마음에 만들었습니다. ERC20는 실제로 Main Ethereum Network에는 발행하지못했지만 Rinkeby testnet에 발행해봤습니다. 
데모 영상: https://www.youtube.com/watch?v=r791oYxf3dg

[3] Java - Framework/IDE/Server: Spring Framework/Eclipse EE Oxygen/Apache Tomcat 9. 
>이 프로젝트는 서울에 집값이 비싸서 주머니 사정이 안좋은 사람들을 위해서 쉐어메이트를 찾게만들어주면 좋을것같아서 방학때 혼자 독학으로 만든 웹어플리케이션입니다. 물론 학교에서 자바를 가르쳐주기는 했지만, 프레임워크에 대해서는 전혀 가르쳐주지않아서 혼자 독학으로 Spring Framework랑 JSP 등을 공부해서 MyBatis로 MySQL을 매핑시킨 웹어플리케이션입니다. 기존의 다른 쉐어메이트 사이트의 차별화를 둔 부분은: 
유저가 거리 범위에 따라서 필터링을 할 수 있습니다. (예를 들어 5km 범위내의 서울특별시 이태원)
구글맵을 통해서 하우스의 위치 확인을 하고 원하면 자세한 정보를 볼수있습니다 (가격순 거리순으로도 정렬 및 확인 가능함). 
Lat, Lng을 이용해서 만들었기때문에 일본, 미국 등 다른 나라도 쉐어메이트를 찾을수있게 만들었습니다.
데모 영상: https://www.youtube.com/watch?v=FmyxsrNaN50

[4] FunCook
 >FunCook은 restful API를 이용해서 flickr API를 이용해서 아시안 음식사진을 가져와서 food AI API로 음식사진을 인식해서 음식의 이름을 따내서 edamam API를 이용해서 연관된 레시피를 검색해서 일상 생활 음식에 질린 서양인들이 새로운 음식을 경험할 수 있게 도와주는 웹어플리케이션입니다. 이 웹어플리케이션의 조금 특별한 점이 있다면 만약에 유저가 두개 이상의 이름을 가진 음식을 찾을때 (Keropok, Krupuk - 인도네시아 음식), Keropok라고 레시피를 찾았는데 검색결과가 없으면 Wikipedia API를 이용해서 제일 연관된 컨텐츠의 (Krupuk) 이름을 찾아서 다시 검색을 해줍니다. 
데모 영상: https://www.youtube.com/watch?v=hC_E5ZqqCfE
[5] Twiffy
>Twiffy는 Data Science의 기초라고 할수있는 Twitter Sentiment Analysis입니다. 예를 들어 트럼프를 검색하면 실시간으로 트럼프의 대한 댓글들을 통해서 얼마나 많은 사람들이 좋아하는지 아님 싫어하는지를 파이차트와 라인그래프를 이용해서 유저에게 쉽게 알려줍니다. 기존의 다른 아주 많은 Twitter Sentiment Analysis와 다른 점이있다면:
Flexibility - 웹소켓을 자유자재로 일시정지시키고 다시 시작할수있고 굳이 페이지를 다시 리프레시하지 않아도 새로운 검색을 할수있습니다.
Persistence - 두 명또는 그보다 많은 사용자가 똑같은 검색을 하면, 똑같은 검색결과를 얻을수있습니다. 
개인적으로 아쉬운 점이 있다면 MongoDB와 같은 NoSQL을 새로 공부해서 연결하고 싶었지만, 시간이 많이 없어서 제가 그나마 가장 잘알고있는 MySQL로 연결했습니다. 지금 AWS 계정을 없애서 MySQL 에러가 뜰것이지만, 그래도 테스트 하고싶으시면 스키마랑 테이블을 따로 만드시면 작동될것입니다. 그리고, 아마 프로그램을 실행시키다보면 Twitter API Limit Exceeded - 420 Status Code 라는 것이 뜰것인데 이것은 Load Balancer가 있어야 사라지는 문제입니다. 
데모 영상: https://www.youtube.com/watch?v=shBqxzgzguM

[6] [Go Lang / 카카오챗봇 / Android / IOS](https://drive.google.com/drive/folders/16B64InkkKJfca28p1NeDFAuiRsssXw4C?usp=sharing) - 이 프로젝트들은 그냥 심심할때 만든거라서 동영상 촬영을 안했습니다. 
> Go Lang: Go 언어를 상징하는 캐릭터가 재밌게 생겨서 한번 배워보고 싶어서 front-end (vue.js, vuetify, element.ui, axios), back-end (gorilla/mux, mgo/mongodb)를 이용해서 간단한 CRUD web app을 구현했고 pagination 처리까지 했습니다. docker-compose로 작성했기 때문에 별도로 mongodb, vue.js, go lang 설치없이 docker만 설치되어있으면 docker-compose up -d 커맨드를 제 프로젝트 루트 디렉토리에서 실행시키면 작동이 됩니다. 


[7] [카카오챗봇](https://drive.google.com/drive/folders/16B64InkkKJfca28p1NeDFAuiRsssXw4C?usp=sharing)
> 카카오챗봇은 aws educate ec2로 올렸기 때문에 19년 8월까지 작동할것입니다. 플러스친구에서 funjhy 아이디 검색하셔서 추가하시면 찾을수있고 버튼은 4가지로 구분됩니다. 1. OpenWeatherMap API를 이용한 날씨 검색  2. Google Calendar API를 이용한 날짜 예약하기 3. 이번달 (스케줄 확인) 4. 일주일내 (스케줄 확인) / 예약된 날짜가 없으면 request timeout error가 뜹니다. 프로젝트 폴더에 보안이슈로 accesskey 및 토큰은 제거했습니다. 


[8] [Android - Language/IDE: Java/Android Studio](https://drive.google.com/drive/folders/16B64InkkKJfca28p1NeDFAuiRsssXw4C?usp=sharing)
>Train_Timetable(왼쪽) 앱은 제가 살던 지역이 Runcorn이라는 곳이였는데 기차가 30분에 한 번씩 와서 매번 기차를 기다리기 싫어서 Translink 사이트에서 기차 타임테이블 정보를 가져와서 regex으로 스케쥴을 따내서 간편하게 앱을 열면 볼수있도록 만들었습니다. 그리고, 타이머를 이용해서 1초에 한 번씩 렌더링을 하도록 했습니다.
Military_Calendar(오른쪽) 앱은 친구가 군대갈때 만들어준 군대계산기앱입니다. 



[9] [iOS - Language/IDE: Swift, Object C/Xcode](https://drive.google.com/drive/folders/16B64InkkKJfca28p1NeDFAuiRsssXw4C?usp=sharing)
>Rilakuma_RPG는 리라쿠마라는 일본 캐릭터를 바탕으로 만든 RPG 게임입니다. 쉽게 설명하면 박주영 키우기라는 게임이랑 비슷한 형태입니다. SQLite를 이용해서 허기수치, 감정상태, 지나간 날짜, 가지고 있는 돈을 저장합니다. 기존에 제가 만든 다른 프로젝트를 복사 붙여넣기 하고 프로그래밍했기때문에 프로젝트 이름이 다를 수 있습니다. 


