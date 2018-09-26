# KoNLPy 설치 (Windows+Anaconda)

설치 방법은 아래에 운영체제별로 설명되어 있습니다. <br>
http://konlpy.org/ko/latest/install/

윈도우+아나콘다 설치를 좀 더 상세하게 살펴봅니다.

## 파이썬 32비트, 64비트 구분 
명령라인에서 python을 입력합니다.
<img src="https://i.imgur.com/5Oy5SKj.png" >

설치되어 사용중인 파이썬이 32비트, 64비트 구분 합니다. 이후 설치 프로그램들의 선택이 달라집니다.


## 1) JDK 설치 (JDK-7 이상)
http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

<img src="https://i.imgur.com/qxKNrmo.png" >

JDK을 다운로드 하여 설치
* jdk-8u171-windows-i586.exe (32비트)
* jdk-8u171-windows-x64.exe (64비트)


## 2) 시스템 환경 변수 편집 (JAVA_HOME)
윈도우 키를 누르고 "시스템 환경 변수 편집"를 입력하여 시스템 환경 변수 JAVA_HOME 추가

<img src="https://i.imgur.com/ueg22oB.png" >

<img src="https://i.imgur.com/GwiMf4u.png" >


설정된 환경변수 확인

<img src="https://i.imgur.com/7kyJHl5.png" >


(확인) JAVA_HOME 환경변수 값은 다음과 같습니다.

```
C:\Program Files (x86)\Java\jdk1.8.0_171 (32비트 경우)
C:\Program Files\Java\jdk1.8.0_171 (64비트 경우)
```


## 3) jpype 설치
https://www.lfd.uci.edu/~gohlke/pythonlibs/#jpype

JPype1 다운로드 하여,
* JPype1‑0.6.3‑cp36‑cp36m‑win32.whl (32비트 경우)
* JPype1‑0.6.3‑cp36‑cp36m‑win_amd64.whl (64비트 경우)

다음과 같이 pip로 설치

```
C:\Users\Seung-June\Downloads>pip install JPype1‑0.6.3‑cp36‑cp36m‑win_amd64.whl
```

## 4) KoNLPy 확인


```python
from konlpy.tag import Kkma
engine = Kkma()
nouns = engine.nouns('NLP: 컴퓨터가 인강의 언어를 알아들을 수 있게 만드는 학문분야. 인공지능의 하위 분야로, 일반적인 인공지능을 만들려던 1960년대의 시도가 실패한 후, 인간의 언어를 분석하고 처리하는 인공지능이 세분화 되면서 생긴 학문 분야. 흔히 우리가 아는 말하는 컴퓨터 및 인간과 대화하는 컴퓨터 관련 기술이 이 쪽에 속한다.')
print(nouns)

```

```python
['컴퓨터', '강의', '언어', '수', '학문', '학문분야', '분야', '인공', '인공지능', '지능', '하위', '일반적', '1960', '1960년대', '년대', '시도', '실패', '후', '인간', '분석', '처리', '세분화', '우리', '말', '대화', '관련', '기술', '쪽']
```



<img src="https://i.imgur.com/kdhtRvG.png" >




#### 2018 FinanceData.KR
