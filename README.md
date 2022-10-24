


![logo](https://user-images.githubusercontent.com/103496262/197355772-f4df931e-10fb-43e5-843f-04d33a04df64.JPG)


# 모각코, 함께 코딩하고 교류하는 커뮤니티

혼자 코딩하느라 지치시지는 않으신가요?
다양한 사람들과 함께 코딩하면서 교류해보세요!
<br><br>
## [🚀MoCo 접속하기](https://moco.site)
<br>

# 📖 목차 
 - [소개](#소개) 
 - [개발 환경](#개발-환경)
 - [사용 기술](#사용-기술)
 - [아키텍처](#시스템-아키텍처) 
 - [E-R 다이어그램](#e-r-다이어그램)
 - [Api 명세서](#-api-명세서)
 - [프로젝트 목적](#프로젝트-목적)
 - [화면 구성](#화면-구성)
 -  [핵심 기능](#핵심-기능)
    - [로그인](#로그인)
    - [Toast Ui editor](#toast-ui-editor)
    - [게시글 CRUD](#게시글-crud)
    - [댓글과 대댓글 구현](#댓글과-대댓글-구현)
    - [에러 처리](#에러처리)
    - [페이징 처리](#페이징-처리)   
    - [스마트 컨트랙트 호출](#스마트-컨트랙트-호출)
 - [CI/CD](#cicd)
 - [도메인 https 적용](#도메인-https-적용)
 - [Dev History](#dev-history)
	 -  [ISSUE](#issue)
	 -  [ERROR](#error) 
	 -  [UI/UX](#uiux-reference)


## 📃소개
**MoCo**는 개발자및 다양한 사람들과 소통할수 있는 플랫폼으로, 다양한 사람들간의 IT 생태계를 교류할수 있도록 도와줍니다.
<br>
참여율을 높이기위해 하루에 한번씩 모각코인을 받을수 있습니다. 받은 모각코인으로 도트맵을 구매할수 있습니다. 


## 개발 환경

![IntelliJ](https://img.shields.io/badge/macOS-M1-black?style=flat&logo=macos)&nbsp;![IntelliJ](https://img.shields.io/badge/intellJ-ffa4c4?style=flat&logo=IntelliJIDEA)&nbsp;![IntelliJ](https://img.shields.io/badge/github-606060?style=fat&logo=github)&nbsp;![IntelliJ](https://img.shields.io/badge/vscode-blue?style=flat&logo=VisualStudioCode)&nbsp;![IntelliJ](https://img.shields.io/badge/Docker-ADD8E6?style=flat&logo=docker)&nbsp;![IntelliJ](https://img.shields.io/badge/DBeaver-blue?style=flat)

 - MacOS M1
 - IntelliJ 
 - Visual Studio Code
 - GitHub
 - Docker
 - DBeaver

## 사용 기술 

![java](https://img.shields.io/badge/Java-11-DEB887?style=flat)&nbsp;![springboot](https://img.shields.io/badge/SpringBoot-2.7.2-3CB371?style=flat&logo=springboot)&nbsp;![spriongsecurity](https://img.shields.io/badge/SpringSecurity-5-3CB371?style=flat&logo=springsecurity)&nbsp;![spriongsecurity](https://img.shields.io/badge/Solidity-^0.8.0-c5ac00?style=flat&logo=solidity)

![spriongsecurity](https://img.shields.io/badge/Html5-C0C0C0?style=flat&logo=HTML5)&nbsp; ![spriongsecurity](https://img.shields.io/badge/CSS3-blue?style=flat&logo=css3)&nbsp; ![spriongsecurity](https://img.shields.io/badge/Thymeleaf-green?style=flat&logo=thymeleaf)&nbsp; ![spriongsecurity](https://img.shields.io/badge/BootStrap5-purple?style=flat&logo=Bootstrap)

![gradle](https://img.shields.io/badge/Gradle-7.5-skyblue?style=flat&logo=gradle)

![mysql](https://img.shields.io/badge/MySQL-8.0.28-FFA07A?style=flat&logo=mysql)

![ec2](https://img.shields.io/badge/AWS-ec2-FF8C00?style=flat&logo=amazonec2)&nbsp;![s3](https://img.shields.io/badge/AWS-s3-FF8C00?style=flat&logo=amazons3)&nbsp;![alb](https://img.shields.io/badge/AWS-alb-FF8C00?style=flat&logo=JFrogBintray)&nbsp;![route53](https://img.shields.io/badge/AWS-RDS-FF8C00?style=flat&logo=amazonrds)&nbsp;![rds](https://img.shields.io/badge/AWS-Route53-FF8C00?style=flat&logo=ray)

**백엔드**
  - Java 11 openjdk
  - SpringBoot 2.7.2
  - Spring Security5
  - Spring Data JPA 
  - Lombok

**프론트엔드**
 -   Html5/css3
 -   Javascript
 -   Thymeleaf
 -   Bootstrap 5
 
**빌드 툴**
 - Gradle 7.5

**데이터베이스**

 - Mysql

**인프라** 
-   AWS EC2
-   AWS S3
-   AWS Route53
-   AWS RDS
-   AWS ALB
-   Github Actions
-  Docker
-  DockerHub

**블록체인**
- goerli network
- solidity
- Meta Mask

**라이브러리**

 - [web3.js](https://web3js.readthedocs.io/en/v1.8.0/getting-started.html)
 - [openzeppelin-ERC20](https://docs.openzeppelin.com/contracts/4.x/erc20)
 - [tippy.js](https://atomiks.github.io/tippyjs/v6/getting-started/)
 - [toastui-editor](https://ui.toast.com/tui-editor)
 - [tagify](https://yaireo.github.io/tagify/)
 - [xeicon](http://xpressengine.github.io/XEIcon/started.html)
 - [fabric](http://fabricjs.com/docs/)
 - [copy-down](https://github.com/furstenheim/copy-down)

## 시스템 아키텍처
![시스템 아키텍처](https://user-images.githubusercontent.com/103496262/197354146-c861abe0-3f00-4f33-b276-66bd97903e7b.jpg)



## Server 아키텍처 
![아키텍처](https://user-images.githubusercontent.com/103496262/197343496-40279a8a-7ee3-4360-b1e5-679379bacd90.JPG)


## E-R 다이어그램
![ERD](https://user-images.githubusercontent.com/103496262/197354994-eefbbe74-47a7-4188-a3f9-1c240f11ff17.png)


## 📑 Api 명세서
### [Api 명세서 보기](https://moco.site/swagger-ui/index.html)


## 프로젝트 목적
실서비스 가능한 웹 애플리케이션을 만들어 보고 싶었습니다. 
나아가 이론보다는 직접 개발을 해나가며 배우는 것이 많다고 생각하기 때문에 시작했습니다.

팀프로젝트가 아닌 처음해보는 개인 프로젝트로 배포까지 해보는 것이 목표였으며,

웹 개발자로 진로를 잡은 시점에서 배포 가능한 웹 애플리케이션의 전 과정에 대해 한번쯤은 경험해 보고 싶었습니다. 

단순히 포트폴리오를 위한 프로젝트로 남는것이 아닌 프로덕트 단계까지, 사용자들의 피드백을 받으며 유지보수 까지 가능한 웹 애플리케이션을 만들어 보기로 결정했습니다.



## 화면 구성💻
|![첫페이지](https://user-images.githubusercontent.com/103496262/197594246-1b8f38d6-5629-452f-9e0d-65cdc6f2165d.JPG)|![메인페이지](https://user-images.githubusercontent.com/103496262/197594248-86b5fbc9-758e-4dd3-9928-47fc6267bbc8.JPG)| ![로그인](https://user-images.githubusercontent.com/103496262/197594244-12bcb35c-7aac-44dd-a429-d37be4129cd8.JPG) | ![회원가입](https://user-images.githubusercontent.com/103496262/197594262-c83cf72d-7681-4ee8-9b3d-6bf75f1a8e2e.JPG) |
| :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: |
|                                                      첫 페이지                                                      |                                                       메인 페이지                                                        |                                                      로그인                                                       |                                                     회원가입                                                      |

| ![글작성](https://user-images.githubusercontent.com/103496262/197594251-a6cb939c-5610-4f34-8fea-665866e2b1a4.JPG) | ![게시글 보기](https://user-images.githubusercontent.com/103496262/197594254-9aa7b7eb-e282-445b-a82b-a7645fdc8c0a.JPG) | ![출석체크보상 토큰받기](https://user-images.githubusercontent.com/103496262/197594242-c692895c-90f2-47cb-b3e3-30ddc58d100a.JPG) | ![설정페이지](https://user-images.githubusercontent.com/103496262/197594859-ead2455a-d3b1-4ec0-8ef4-19f1dff163b4.JPG) |
| :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: |
|                                                      글작성 페이지                                                      |                                                       게시글 보기                                                        |                                                      출석체크 보상                                                        |                                                     설정 페이지                                                      |

<br>

| ![도트맵](https://user-images.githubusercontent.com/103496262/197594258-1ed03775-c6ca-4b0d-bac4-0f1d4fe41abd.png) | ![땅구매 모달창](https://user-images.githubusercontent.com/103496262/197594259-241a9d1b-5463-40cb-8de2-1ad91b2ebe87.JPG) | ![구매된 땅 표시](https://user-images.githubusercontent.com/103496262/197594231-cd4a6cf7-40a4-468f-852f-75c7e0275a00.png) |
| :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------: |
|                                                     도트맵 페이지                                                      |                                                       땅구매 모달창                                                        |                                                      구매된 땅 표시                                                      |

<br>

## 핵심 기능⭐
### 🌠로그인
 - 소셜 로그인
   - 소셜 로그인 구현을 위해 스프링 시큐리티와, OAuth2 인증방식을 사용했으며, 엑세스 토큰으로 받아오는 유저 정보를 커스텀하여 사용하기 위해 Oauth2UserService 인터페이스를 상속받아 CustomOauth2UserService 클래스를 구현하였습니다. <br> [CustomOauth2UserService](https://github.com/JaeJinByun/MoCo/blob/986566e2fe78b7bab74394fa0f3650f85186adc2/src/main/java/com/board/board/service/user/CustomOAuth2UserService.java#L25)
 - 일반 로그인   
   -  자체 로그인 방식으로는 회원가입시 입력한 비밀번호를 해시 암호화 알고리즘을 적용하여 나온 해시값을 DB에 저장합니다. 
   - 로그인시 사용한 해시 알고리즘을 찾아 비밀번호의 정합성을 검증합니다. <br> [UserService](https://github.com/JaeJinByun/MoCo/blob/986566e2fe78b7bab74394fa0f3650f85186adc2/src/main/java/com/board/board/service/user/UserService.java#L38)
  
### 🌠Toast Ui editor

&ensp;&ensp;**이미지 저장**
 - 게시글 작성은 NHN에서 개발한 오픈소스로, 마크다운과 위지윅 방식을 지원하는 생산성있는 라이브러리를 이용했습니다. 
 - 게시글 작성시 이미지 삽입은 base64형식의 단점을 보완한 hooks 옵션을 사용했습니다. 
 - 이미지의 base64 인코딩의 단점은 해상도에 따라 글자수가 기하급수적으로 올라가기 때문에 DB저장시 문제가 발생합니다. 
 - 따라서 이미지의 저장된 주소값인 url을 저장하도록 했습니다. 
 
 1. 이미지 삽입시 hooks 옵션으로 blob 객체를 인터셉터합니다.
 2. Ajax로 blob 객체를 백엔드 서버로 저장 요청을 보냅니다.
 3. 백엔드 서버에서 blob 객체를 multipart로 받아 aws s3 버킷에 저장 요청을 보냅니다.
 4. 저장에 성공시 업로드된 url을 반환합니다. 
 
[이미지 업로드 요청](https://github.com/JaeJinByun/MoCo/blob/fc6398cb0ac90d1c976368061d1f1119985bce45/minify%20%EC%A0%81%EC%9A%A9%EC%A0%84%20JS%20%ED%8C%8C%EC%9D%BC/js/board/write.js#L11)

[이미지 업로드 처리](https://github.com/JaeJinByun/MoCo/blob/986566e2fe78b7bab74394fa0f3650f85186adc2/src/main/java/com/board/board/controller/AwsS3Controller.java#L21)


### 🌠게시글 CRUD
&ensp;&ensp;**글작성**
- Toast Ui editor로 작성한 마크다운 문법을 html 로 파싱하여 저장하였습니다. 
- 게시글 저장시 각 항목에 대한 유효성을 검사합니다. 에러 발생시 작성했던 내용들은 유지하면서 에러 내용또한 반환하도록 했습니다. 
  - [게시글 저장](https://github.com/JaeJinByun/MoCo/blob/fc6398cb0ac90d1c976368061d1f1119985bce45/src/main/java/com/board/board/controller/BoardController.java#L207) 
- tagify 라이브러리를 이용하여 태그를 작성할수 있습니다.  태그들은 Json 포맷으로 받아오며 ArrayList 자료구조로 파싱하여 한개의 태그당 한개의 컬럼으로 DB에 저장합니다. 
  - [태그 저장](https://github.com/JaeJinByun/MoCo/blob/fc6398cb0ac90d1c976368061d1f1119985bce45/src/main/java/com/board/board/controller/BoardController.java#L225) 
 
&ensp;&ensp;**글 수정**
 - 게시글 본문의 내용을 DB에 저장시 마크다운으로 저장해야 할지, Html태그로 변환후 저장해야 할지 고민이 많았습니다. 해당 이슈는 아래 링크에서 확인하실수 있습니다.
   -  [게시글 수정시 Toast editor에 Html 코드가 나오는 이슈](https://zinzae.notion.site/Html-daf08a98466842f1a7cc36929a0cc80a)
 - 게시글 수정은 빈번하게 발생하는 작업이 아니기 때문에 html 태그로 저장후 게시글 수정시에 마크다운 문법으로 파싱하도록 구현하였습니다. 
   - [Html -> MarkDown](https://github.com/JaeJinByun/MoCo/blob/fc6398cb0ac90d1c976368061d1f1119985bce45/src/main/java/com/board/board/controller/BoardController.java#L180) 
-  태그 수정시 삭제된 태그, 추가된 태그를 구분하기 위해 hashSet 자료구조의 차집합을 구할수 있는 removeAll() 메소드를 사용하였습니다.
   -   [태그 수정](https://github.com/JaeJinByun/MoCo/blob/762a33a28dfa570ffbad86c4778efd070586a1d3/src/main/java/com/board/board/controller/BoardController.java#L274) 

&ensp;&ensp;**글 삭제**
- [자신이 작성한 게시글만 삭제 가능하도록 세션을 이용해 검증하였습니다. ](https://github.com/JaeJinByun/MoCo/blob/fc6398cb0ac90d1c976368061d1f1119985bce45/src/main/java/com/board/board/controller/BoardController.java#L308)

&ensp;&ensp;**게시글 읽기**
- [조회수 중복 방지를 위해 쿠키를 사용하여 조회수 증가를 방지했습니다.](https://github.com/JaeJinByun/MoCo/blob/fc6398cb0ac90d1c976368061d1f1119985bce45/src/main/java/com/board/board/controller/BoardController.java#L89)

### 🌠댓글과 대댓글 구현

 대댓글의 경우 엔티티 구조안에서 셀프조인을 참조하여 계층을 가지도록 구현했습니다. 
   - [대댓글 계층정렬](https://github.com/JaeJinByun/MoCo/blob/fc6398cb0ac90d1c976368061d1f1119985bce45/src/main/java/com/board/board/service/board/CommentService.java#L88)

### 🌠에러처리

로그인, 회원가입시 에러가 나는경우 이를 처리하기위해 커스텀 클래스를 구현했으며,
로그인 관련 에러와 회원가입시 에러에 맞게 처리하였습니다. 
발생한 에러들은 추적이 가능하도록 Log를 남겨 CloudWatch 모니터링 시스템을 이용하여 실시간으로 확인 가능하도록 처리했습니다. 

[CustomAuthFailureHandler](https://github.com/JaeJinByun/MoCo/blob/c93bdc6252c5580679b9a58b3bd5f5a4c2789990/src/main/java/com/board/board/config/auth/CustomAuthFailureHandler.java#L23)

### 🌠페이징 처리
- ajax를 이용한 무한스크롤
  - 편한 스크롤링으로 콘텐츠가 로드되는 방식으로 특히 모바일 환경에서 더 나은 사용자 경험을 주며,콘텐츠의 노출을 쉽게 접할수 있도록 일반적인 페이지네이션을 두고 무한스크롤을 구현했습니다.
  - [자바스크립트 무한스크롤](https://github.com/JaeJinByun/MoCo/blob/c93bdc6252c5580679b9a58b3bd5f5a4c2789990/minify%20%EC%A0%81%EC%9A%A9%EC%A0%84%20JS%20%ED%8C%8C%EC%9D%BC/js/board/list.js#L1) 
  
 - 스크롤 위치와 데이터 유지
   - 무한 스크롤의 단점인 렌더링된 게시글들과 스크롤링 했던 위치로 돌아올수 있도록 세션스토리지를 이용하였습니다. 
   - 게시글 리스트페이지를 벗어날때 세션스토리지에 스크롤의 위치와 렌더링 정보를 저장후 해당 페이지에 돌아왔을때 세션 스토리지에 저장된 값을 렌더링하며 이전 스크롤의 위치로 이동하도록 구현했습니다.
   -  [렌더링, 스크롤 위치기억하기](https://github.com/JaeJinByun/MoCo/blob/c93bdc6252c5580679b9a58b3bd5f5a4c2789990/minify%20%EC%A0%81%EC%9A%A9%EC%A0%84%20JS%20%ED%8C%8C%EC%9D%BC/js/board/list.js#L169)
 
 ### 🌠스마트 컨트랙트 호출
 - openzeppelin 라이브러리를 이용하여 웹 애플리케이션에서 사용할수 있는 ERC-20 기반 토큰을 만들었습니다. 
 [스마트 컨트랙트](https://github.com/JaeJinByun/MoCo/blob/762a33a28dfa570ffbad86c4778efd070586a1d3/MyToken.sol#L5)
 
 - Web3.js 라이브러리를 이용하여 배포한 컨트랙트를 호출하여 토큰을 받을 수 있습니다. 
[자바스크립트 컨트랙트 호출](https://github.com/JaeJinByun/MoCo/blob/762a33a28dfa570ffbad86c4778efd070586a1d3/minify%20%EC%A0%81%EC%9A%A9%EC%A0%84%20JS%20%ED%8C%8C%EC%9D%BC/js/web3js/web3js.js#L533)
 


### CI/CD 
반복적인 프로세스 덜고 유지보수의 편리함을 위해  지속적 통합과 지속적 배포 파이프라인을 구축하였습니다.

깃 허브액션이 master 브랜치로 push된 code를 감지하여 생성한 스크립트 설정파일에 따라 jar 파일로 빌드후 도커 이미지화 시킵니다. 

도커 이미지화된 도커파일은 도커 이미지 저장소인 도커 허브로 push 됩니다.

push가 완료되면 ec2 인스턴스가 해당 도커 파일을 pull 하게 되며 실행중이었던 스프링부트 도커파일을 
정지 -> 컨테이너 삭제 -> 새로 내려받은 도커파일 실행 순으로 작업을 진행합니다. 

### 도메인 https 적용
브라우저의 안전한 접속과 , 브라우저 사이의 민감한 정보를 주고받을때를 대비해 aws ACM인증서를 받아 SSL 을 적용하였습니다. 
가비아에서 구매한 도메인과 aws Route53을 이용해 도메인을 연결하였습니다.


## Dev History
개발과정에서 발생한 이슈나 에러를 해결했던 기록을 남겼습니다. 

### ISSUE
- [SNS 회원가입시 name 중복으로 인한 게시글작성 실패](https://zinzae.notion.site/SNS-name-e6c937600ce54eab990ccbe6883ad762)
- [댓글 가져올수 없음 (생성자 레퍼런스 사용불가)](https://zinzae.notion.site/0123aac67d984ca0811d06271a759608)
- [무한스크롤구현과 뒤로가기 버튼으로 인한 DATA 초기화로 인한 스크롤 유지 불가](https://zinzae.notion.site/DATA-1894ace4bb1c47eeb2f6bf447b6cc428)
- [AJAX를 이용한 별명중복 체크시 응답에러](https://zinzae.notion.site/AJAX-74e289e5a81343f4ad2dd54679f4b921)
- [썸네일 존재 여부에 따른 로드 오류](https://zinzae.notion.site/c7ec41ef950c4faba8dc7c75a438befa)
- [이메일 인증을 하지 않은 아이디일 경우 그에 맞는 에러 리턴하기](https://zinzae.notion.site/1fc6b580456947ce89d224de3c6eb6db)
- [게시글 수정시 마크다운 편집기에 Html 코드가 나오는 이슈](https://zinzae.notion.site/Html-daf08a98466842f1a7cc36929a0cc80a)
- [해시태그 저장시(JPA) save VS saveAll 성능 고려](https://zinzae.notion.site/JPA-save-VS-saveAll-943e6fbe6e5f43809aafc9c8b3deb1bd)
- [스마트 컨트랙트 Java 래퍼 클래스로 변환시키기-Web3.js→Web3j](https://zinzae.notion.site/Java-Web3-js-Web3j-ecd95728c722487cac224df83f5f043d)
- [대댓글이 2번 중복되어 파싱되는 이슈](https://zinzae.notion.site/2-661fe5d8636c43b4b5930a3a2848e568)
- [해시태그 수정시 처리할 로직에 대해서](https://zinzae.notion.site/94ad8292ae3748d896c3ee1987732a56)
- [게시글 목록 조회시 N+1 문제](https://zinzae.notion.site/N-1-703279ae09ce4d1192f523f03b79e5d9)
- [게시글 조회시 실행되는 쿼리문 최적화 필요성](https://zinzae.notion.site/a8027faca93a4127960f973ade85eb13)
- [모집 마감 버튼 클릭시 확인창을 무시하며 ajax 호출](https://zinzae.notion.site/ajax-ac3ca0e056ec4ec8bef531fd5df45555)
- [회원 별명 변경시 게시글작성자명은 바뀌지 않는 이슈](https://zinzae.notion.site/42b9154079ef47ef97244652ce3c7843)
- [JQuery 부분 새로고침 `<div>` 중복 생성 문제, 부분 새로고침으로 인한 엘리먼트 참조문제]()

### Error 
- [WebSecurityConfigurerAdapter is deprecated](https://zinzae.notion.site/WebSecurityConfigurerAdapter-is-deprecated-6510f7fd802d48d59339e48a7894c556)
- [AnnotationException: @OneToOne or @ManyToOne …](https://zinzae.notion.site/AnnotationException-OneToOne-or-ManyToOne-eee7a9a6eb1f466ca3fae5305555fc35)
- […ClientRegistrationRepository' that could not be found.](https://zinzae.notion.site/ClientRegistrationRepository-that-could-not-be-found-50667daca0924e68acc7c872ed27600c)
- [Naver 로그인시 java.lang.IllegalArgumentException: Missing attribute 'id' in attributes](https://zinzae.notion.site/Naver-java-lang-IllegalArgumentException-Missing-attribute-id-in-attributes-105f718cdc044720bf8bca6e11e86fa4)
- [An internal error occurred while trying to authenticate the user.](https://zinzae.notion.site/An-internal-error-occurred-while-trying-to-authenticate-the-user-a499090aac4e4716a1a3ae31b4993692)
- [TemplateInputException](https://zinzae.notion.site/TemplateInputException-26c19d75c4894d96b2ad7445aa37b0fd)
- [method call attempted to call method size() on null context object](https://zinzae.notion.site/method-call-attempted-to-call-method-size-on-null-context-object-8ba389ebddeb4880b0b1eda5aaee4ea3)
- [Cannot call sendRedirect() after the response has been committed](https://zinzae.notion.site/Cannot-call-sendRedirect-after-the-response-has-been-committed-d437a190ac0045c8ab2a25c75cc4948a)
- [Uncaught ReferenceError: saveComment is not defined at HTMLButtonElement.onclick](https://zinzae.notion.site/Uncaught-ReferenceError-saveComment-is-not-defined-at-HTMLButtonElement-onclick-f5fc4a6c6363438fac4642478885062d)
- [nested exception is org.hibernate.loader.MultipleBagFetchException: cannot simultaneously fetch multiple bags](https://zinzae.notion.site/nested-exception-is-org-hibernate-loader-MultipleBagFetchException-cannot-simultaneously-fetch-mult-ff83fa5bbdb449b2b834473956f5821c)
- [Error executing DDL "create table like … engine=InnoDB" via JDBC Statemen](https://zinzae.notion.site/Error-executing-DDL-create-table-like-engine-InnoDB-via-JDBC-Statemen-c20b371936524816b5ea8372ce4d3783)
- [failed to lazily initialize a collection of role:com.board.board.domain.Comment.childList, could not initialize proxy - no Session](https://zinzae.notion.site/failed-to-lazily-initialize-a-collection-of-role-com-board-board-domain-Comment-childList-could-not-8a6bbe24d57248b5ac6b003823782c1c)
- [com.amazonaws.SdkClientException: Failed to connect to service endpoint](https://zinzae.notion.site/com-amazonaws-SdkClientException-Failed-to-connect-to-service-endpoint-adda112fdff847ddae4344c16ad2dd99)
- [TypeError: replace is not a function in JavaScript](https://zinzae.notion.site/TypeError-replace-is-not-a-function-in-JavaScript-3e0445f01ab046218fafaab3916b0a32)

---
### UI/UX Reference

- [좋아요 버튼](https://codepen.io/aaroniker/pen/BaZJMjv)
- [슬라이드 효과](https://swiperjs.com/swiper-api)
- [로그인 효과](https://codepen.io/karlovidek/pen/aNYWKE)
- [소셜 로그인 아이콘](https://codepen.io/RajRajeshDn/pen/qXeJOG)
- [구매된 도트의 모달창](https://codepen.io/lamchang/pen/PQGQyR)

 
## 느낀점 
팀 프로젝트가 아닌 1인 프로젝트로 진행하다 보니 개발 과정에서 발생하는 에러나, 이슈를 혼자 해결해 나가면서 더 나은 방법은 없는지 최선의 방법인지 피드백을 받을 수 있는 방법을 찾기 위해 많은 고민을 했습니다. 

공식문서, 여러 IT 커뮤니티 ,개발자 오픈채팅방 등을 통하여 현업에 계신 분들의 많은 도움을 많이 받았습니다.

프로젝트를 진행 할수록 부족함이 많다는 것을 느꼈으며, 원리를 이해하고 쓰는것과 모르고 쓰는 것의 중요함을 한번더 알게된것 같습니다. 깨닫고 배울수록 배워야할 지식의 곁가지가 늘어남을 체감하고 있습니다. 

이번 프로젝트로 인해 개발을 바라보는 자세가 많이 바뀐 계기가 된 것 같습니다. 
개발은 단순히 기능을 구현하기 위해 코딩하는 것이 아닌 문제를 바라보고 해결해 나가기 위한 과정이라는 것을 크게 느끼게 된 경험이었습니다.

