아무래도 CS 공부가 좀 필요할거같다.
꾸준히 하는게 목표이니, 천천히 공부해보자

# Protocol
프로토콜은 '약속', '규약', '협약' 등을 의미하는 단어로, 네트워크 분야 외에도 
여러 분야에서 통용된다고 한다.
상호간 원활한 교류, 소통, 통신을 위해 서로 동일하게 어떠한 설정/규칙을 
정한다는 뜻이다

비슷한 느낌으론 전화 통화 시 '여보세요'로 전화를 받으면서 시작하는 것이 
사회적 협약인 것과 같다.

컴퓨터 네트워크 환경 내 모든 기기가 서로 통시하며 데이터를 주고 받으려면, 각 
기기에는 사전 협의된 통신 협약/규약이 필요하다, 이 규약을 '네트워크 
프로토콜' 이라 하는데, 현존하는 네트워크 프로토콜은 수 십 여종이 존재한다.

인터넷을 사용하며 자주 접하는 건 몇 가지 안되는데, 요즘 같은 '인터넷 시대', 
'클라우드 시대'에 간단히 알아두면 유용하리라

![](https://velog.velcdn.com/images/minthug94_/post/42131085-197c-4cdc-93c5-00ce087f335e/image.png)
(출처=Agilent Technololgy)

## 인터넷 접속을 위한 기본 프로토콜 - TCP/IP
컴퓨터 네트워크에서 TCP/IP 프로토콜은 인터넷 연결에 있어 핵심이면서 대단히 
중요한 역할을 한다.
가끔 인터넷을 하다보면 본듯한 기억이 있다
'TCP/IP'는 TCP프로토콜의 특성과 IP 프로토콜의 특성을 합친 것이다.
즉, IP주소 체계(IP 프로토콜의 특성)을 통해, 신뢰성 높은 데이터 
송수신(TCP프로토콜의 특성)을 보장한다.

![](https://velog.velcdn.com/images/minthug94_/post/faa8d920-e4d9-48ea-917f-b10b4b358084/image.png)

맥북에 네트워크를 확인해보면, Internet Protocol Version 4 (TCP/IPv4) 와 
Internet Protocol Version 6 (TCP/IPv6) 옵션이 있을거다.
사용자가 사용하는 TCP/IP 버전이 'v4'이다

TCP/IPv6는 현행 v4의 IP주소 구조를 확장해, IP주소 고갈/부족 문제를 해결할 수 
잇따.
다만 대중적으로 확산되기 까진 시간이 좀 더 필요하다고 한다

IP주소, 서브넷마스크, 게이트웨이 주소, DNS 서버 주소 등을 통해 인테넷 
웹사이트에 접근하려면, 해당 웹사이트 서버와 사용자 PC는 모두 TCP/IP 
프로토콜을 사용한다는 규약이 적용돼 있어야 한다.

# 홈페이지를 제대로 출력하기 위한 프로토콜 - HTTP

일반적로 웹브라우저로 특정 홈페이지를 여는 건 '인터넷 접속'의 한 방식
인터넷 홈페이지 / 웹페이지는 기본적으로 '하이퍼 텍스트(Hyper-text)' 라는 
프로그래밍 언어(HTML)로 제작되는데, 이 하이퍼 텍스트 웹페이지를 제공, 
제어하는 프로토콜 HTTP(Hyper Text Transfer Protocol)이다.

웹브라우저 주소창에 'http://~' 라 입력하는 건, HTTP 프로토콜을 통해 HTML로 
제작된 웹페이지에 연결하겠다는 의미이다.
즉, 여기서 'http' 대신 다른 프로토콜을 입력하면 다른 방식으로 해당 사이트에 
접속하게 된다.

> 요즘엔 웹브라우저 주소창에 'http'를 따로 입력하지 않아도, http가 자동 
포함된 것으로 간주된다.
아울러 'http' 가 아닌 'https' 프로토콜도 많이 사용되는데, 이는 http와 
동일하지만 보안(Secure) 기능을 추가한 것이다.
https 프로토콜은 서버와 PC 간 송수신되는 데이터를 암호화하는데, 대게 
홈페이지 로그인이나 회원가입, 온라인 결제 등에 자동 적용된다.

## 빠른 파일 송수신을 위한 프로토콜 - FTP
화려하게 꾸며진 홈페이지 형식이 아닌, 파일 송수신 만을 위한 최소환의 환경만 
제공해 다른 프로토콜보다 파일 송수신 속도가 빠르다.
HTTP 프로토콜도 파일 송수신(업로드/다운로드)은 가능하지만, 많은 파일을 
처리하기에 적합하지 않다.
이에 FTP(File Transfer Protocol)는 대량의 파일을 빠르게 송수신할 수 있는 
프로토콜이다

특정 사이트가 ftp 서비스를 제공한다면, 앞선 'http://~' 주소창에 'http' 대신 
'ftp://~' 형식으로 FTP 서비스에 접속할 수 있다.
즉, 인터넷 주소가 같아도 http 로 접속하는 사이트와 ftp로 접속하는 사이트는 
서로 다르다.

일반 웹브라우저나 Finder(윈도우 탐색기) ftp 사이트에 접속할 수 있지만, 
아무래도 FTP 전용 프로그램을 사용하는게 여러 모로 편리하다.
'알드라이브(구.알FTP) || FileZilla' 같은 무료 프로그램이 있다고한다.
이 프로그램들은 사용자 PC를 FTP 서버로도 운영할 수 있는 서버 기능도 
제공한다.

## 이메일을 보내고 받을 수 있는 프로토콜 - SMTP && POP

인터넷으로 이메일을 보내고 받을 때도, 서버와 사용자간 상호 규약이 필요하다
메일을 보낼 땐 SMTP 프로토콜, 받을 땐 POP 프로토콜을 사용한다
(SMTP : Simple Mail Transfer Protocol / POP : Post Office Protocol)

대부분 이메일은 네이버, 구글 등의 이메일 서비스를 사용하기때문에 굳이 알 
필요는 없다 
이미 모두 설정되어있기 때문에

![](https://velog.velcdn.com/images/minthug94_/post/dbd0b2c4-8c49-48be-bf8e-e4fce1118ba2/image.png)


다만 메일 송수신 전용 프로그램을 사용하려면, 해당 포털의 메일 서버의 SMTP 
설정과 POP 설정을 직접 입력해야 한다
이를 설정하면 해당 포털의 메일 홈페이지에 접속하지 않아도, 메일 프로그램을 
통해 바로 메일 송수신이 가능하다.
포털 사이트가 아닌, 자체 메일 서버를 구축, 운영 중인 기업/기관 내 사용자는 
알아두면 좋은 지식이다

> 메일 수신 프로토콜로 POP 외 'IMAP(Internet Messaging Access Protocol)' 
이라는 프로토콜도 자주 사용된다, 몇 가지 특징이 있지만 기본적으로 POP와 
동일한 역할을 한다고 한다.

## 인터넷 주소를 자동 할당, 설정하는 프로토콜 - DHCP

[DHCP 프로토콜](https://velog.io/@minthug94_/DHCP)
IP주소 + 서브넷마스크 + 게이트웨이 주소 + DNS 서버 주소 등의 인터넷 주소 
세트를 자동으로 할당 받아 설정하는 프로토콜이다.
즉, DHCP 서버의 자동 할당 설정에 따라. 사용자 PC도 DHCP 서비스를 실행해 
인터넷 주소를 자동 할당 받는다.

----------------------------
참고 url
https://it.donga.com/31842/
