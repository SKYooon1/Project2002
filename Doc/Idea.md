# 트레이딩 시뮬레이터 (가칭)

###### 플레이어는 주식 트레이더로, HTS를 사용하여 주식 트레이딩하는 시뮬레이션 게임

-----

Base 	
- 20년 가량의 실제 주가 데이터를 통해서 주식 거래
- 게임 내 시간이 실제 시간보다 빠르게 흐름 (약 1분 - 게임 내 1시간)
- 실제 HTS와 (최대한) 비슷한 환경에서 트레이딩을 통해 자산 축적이 목적

Plus 	
- 게임적인 요소가 필요
- 게임 내에서 구매 가능한 아이템, 컨텐츠
- 검색기 기능, 함수 기능, 그래프 기능, 예약 거래 기능 잠금 -> 해금 (보류)
- 집, 차, 사업, 부채, 방 인테리어, 헤어/메이크업/코디 등 컨텐츠, 아이템

구현 내용, 게임의 토대, 게임의 기획 &rightarrow; 보충 필요

---


<a name="footnote_return">왜 이 게임이어야 할까?</a>

<br>

임금격차, 출생률 저하 등 경제적으로 악환경 때문에 추가 수입을 고민하며 주식에 관심이 높아졌다.<sup>[1](#footnote_1)</sup> <sup>[2](#footnote_2)</sup>

&rightarrow; 사람들의 가치관이 과거의 저축 위주에서 투자 위주의 가치관이 형성되는 듯한 경향을 보이는 듯 하다.<sup>[3](#footnote_3)</sup>

<br>

현재 HTS 상황은 아직도 액티브엑스, 논엑티브엑스 시절에서 벗어나지 않는다.<sup>[4](#footnote_4)</sup> <sup>[5](#footnote_5)</sup>

&rightarrow; VR/AR 장르의 주변기기나 투자도 꾸준히 생겨나고 관련 게임도 많아지는데 HTS가 가미된 게임을 만들면 좋을 것으로 사료된다.

<br>

경제상황 악화로 인해 투자에 유입되는 소위 '개미 계층'이 확대되는 경향이 보인다.<sup>[6](#footnote_6)</sup> <sup>[7](#footnote_7)</sup>

&rightarrow; 따라서 주식 투자 시작을 고려하는 사람들의 게임 유입 가능성이 높을 것으로 사료된다.

<br>

최근 비트코인과 같은 암호화폐도 법적으로 대책을 강구해야 한다는 시선이 많아졌다.<sup>[8](#footnote_8)</sup> <sup>[9](#footnote_9)</sup> <sup>[10](#footnote_10)</sup>

&rightarrow; 그럼 비트코인 HTS도 넣어야 하나? 고민의 여지가 있다.

------

업계에 이런 종류의 게임이 출시된 적이 있나?

&rightarrow; 비슷한 것들은 있었다.

<br>

**주식왕** : SyGames에서 제작한 안드로이드 주식 게임. 

게임 내에서 생성된 가상 주식 시장에서 모의투자 가능.

<br>

**Stock'er** : Mindknoll에서 제작한 안드로이드 주식 게임.

실제 데이터를 기반으로 게임 머니를 사용해 국내 주식(코스닥, 코스피)와 해외 주식(나스닥) 시장 모의투자 가능

<br>

**The Trading Game** - Bloomberg에서 제작한 웹 게임.

랜덤한 종목의 과거 주가 등락 데이터를 기반으로 짧은 시간에 수익을 내는 모의투자 게임, 다른 인원들의 통계 산출로 랭킹 기능이 탑재.

<br>

위 게임들을 직접 경험해보고

해당 게임에서 배울 점과 이점이 있을 개선 사항을 찾고

우리 게임만의 차별점을 세우는 것이 필요하다.

<br>

<a name="footnote_1">1</a>: 상장기업 성별 임금격차 더 벌어졌다…여성이 3600만원 덜받아 (한겨례)<sup>[return](#footnote_return)</sup><br>
https://www.hani.co.kr/arti/society/women/1057693.html<br>
<a name="footnote_2">2</a>: "가장 덜 나쁘다"…불안해도 美 증시에 몰리는 돈 (머니투데이)<sup>[return](#footnote_return)</sup><br>
https://news.mt.co.kr/mtview.php?no=2022090714124530851<br>
<a name="footnote_3">3</a>: 2030 투자자 수 2019년 이후 3배 증가… 채무액·개인파산도 가파르게 늘어 (부산일보)<sup>[return](#footnote_return)</sup><br>
http://www.busan.com/view/busan/view.php?code=2022091218515110108<br>
<a name="footnote_4">4</a>: 증권사 'HTS·MTS 장애' 5년새 16배↑…이용자 피해 268억원 (연합뉴스)<sup>[return](#footnote_return)</sup><br>
https://www.yna.co.kr/view/AKR20220906130100002<br>
<a name="footnote_5">5</a>: HTS·MTS 운용에 돈 아낀 증권사들···'연쇄 먹통' 이유 있었네(뉴스웨이)<sup>[return](#footnote_return)</sup><br>
https://www.newsway.co.kr/news/view?ud=2022090816203290196<br>
<a name="footnote_6">6</a>: 개미들 올해 주식 30조원 순매수… '급락장에 독박썼다' (서울와이어)<sup>[return](#footnote_return)</sup><br>
http://www.seoulwire.com/news/articleView.html?idxno=480374<br>
<a name="footnote_7">7</a>: 북클로징 다가온다…개미로 쏠리는 수급 (이코노믹 리뷰)<sup>[return](#footnote_return)</sup><br>
https://www.econovill.com/news/articleView.html?idxno=589099<br>
<a name="footnote_8">8</a>: SEC 위원장, “코인 등 가상자산들 금융당국 규제 받아야” (라디오코리아)<sup>[return](#footnote_return)</sup><br>
https://www.radiokorea.com/news/article.php?uid=396948<br>
<a name="footnote_9">9</a>: 국내 재진출 시동 건 해외 가상자산 거래소들 (디지털투데이)<sup>[return](#footnote_return)</sup><br>
https://www.digitaltoday.co.kr/news/articleView.html?idxno=460204<br>
<a name="footnote_10">10</a>: 접속차단 16개 코인 거래소...투자자 대응 방법과 조치할 것들 (블록미디어)<sup>[return](#footnote_return)</sup><br>
https://www.blockmedia.co.kr/archives/249974<br>