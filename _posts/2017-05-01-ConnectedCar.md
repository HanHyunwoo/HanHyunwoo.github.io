---
layout: post
title: "커넥티드카 시스템 구축 및 운전습관 분석"
featured-img: ConnectedCar #emile-perron-190221
date_format: "2018.05 ~ 2018.06 (1개월)"
summary: "- Spring MVC <br> - Embedded (Arduino, LattePanda CAN통신) <br> - 빅데이터 시스템 구축 (Hadoop)<br> &nbsp;&nbsp;(데이터 적재, 분석, 저장 자동화 구현) <br> - 데이터 시각화 (Highchart, Nwagon, Zing) <br> - HTTP, TCP, FTP 프로토콜 사용"
---

# Intro
<!-- <dt style="font-size:20;font-weight:bold">&nbsp;&nbsp;4차 산업혁명 선도인력 과정을 통해 배운 Web, Spring, Java, Database, Hadoop, Android, R, Embedded CAN통신을 모두 이용하여 빅데이터를 이용한 운전습관 분석 프로젝트입니다.</dt><br><br> -->
<img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/intro.JPG"/><br><br>


## 시연 전체 구조
<img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/entire.JPG"/><br><br>


# Flow
<!-- <dt style="word-break:keep-all">① Arduino Sensor에서 발생하는 데이터를 LattePanda로 전송한다. (CAN통신)</dt>
<dt style="word-break:keep-all">② LattePanda는 받은 데이터를 차량용 Android로 보낸다. (TCP통신)</dt>
<dt style="word-break:keep-all">③ 차량용 Android는 받은 데이터를 WebServer로 보낸다. (HTTP통신)</dt>
<dt style="word-break:keep-all">④ WebServer는 받은 데이터를 LogFile로 Log를 남긴다. (Log4j)</dt>
<dt style="word-break:keep-all">⑤ 생성된 LogFile은 주기적으로 Hadoop시스템으로 전송한다. (FTP, Timer)</dt>
<dt style="word-break:keep-all">⑥ 받은 LogFile을 주기적으로 Hadoop에 적재한다. (ShellScript, Crontab)</dt>
<dt style="word-break:keep-all">⑦ R에서 필요한 Hadoop Data만 추출하고 분석한다.</dt>
<dt style="word-break:keep-all">⑧ 분석된 데이터는 WebServer로 보내고, WebServer는 Oracle에 저장한다.</dt>
<dt style="word-break:keep-all">⑨ 차량용 Android에서 OracleDB를 기반으로 만들어진 WebPage가 보여진다.</dt> -->

 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/flow.JPG"/><br><br>
# TF
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/TF.JPG"/>
### 소스 Github 주소 : <a href="https://github.com/HanHyunwoo/Connected_CAR" target="_blank">https://github.com/HanHyunwoo/Connected_CAR</a><br><br>

 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide1.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide2.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide3.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide4.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide5.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide6.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide7.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide8.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide9.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide10.JPG"/><br><br>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide11.JPG"/><br><br>


<dt style="word-break:keep-all;">&nbsp;&nbsp;커넥티드카를 이용하는 모든 운전자의 데이터와 자신의 데이터를 분석하여, 운전지표 및 효율이 보여진다.</dt>
 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide12.JPG"/><br><br>

 <img src="http://hanhyunwoo.github.io/assets/img/posts/ConnectedCar/slide13.JPG"/><br><br>


# 시연 영상
&nbsp;&nbsp;Sensor를 조작하면 LattePanda와 태블릿화면에 표시되는 것과 WebServer에 로그가 생기는 것을 볼 수 있다.
 <div style="position: relative; max-width: 100%; padding-bottom: 75%; height: 0;">
 <iframe width="4" height="3" src="https://www.youtube.com/embed/WkWnvN9F0Bg" frameborder="0" allowfullscreen="true" style="position: absolute; position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
 </div>
<br>

&nbsp;&nbsp;태블릿에 Sensor를 제어하는 버튼을 누르면 Sensor가 제어된다.
 <div style="position: relative; max-width: 100%; padding-bottom: 75%; height: 0;">
 <iframe width="4" height="3" src="https://www.youtube.com/embed/4jD98kKyrcc" frameborder="0" allowfullscreen="true" style="position: absolute; position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
 </div>
