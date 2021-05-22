# Training Equipment

- 물체인식을 이용한 헬스 운동기구 매뉴얼 어플 -
<br>
<br>
<br>
<br>

## 설계 소개
 - 자세한 내용은 pdf를 확인하시면 됩니다.
<br>
<br>
<br>
<br>

## Getting Started / 어떻게 시작하나요?

1. 안드로이드, 머신러닝, PHP 폴더를 전부 다운로드 받아야 합니다.
2. 핸드폰과 컴퓨터를 연결한 후 안드로이드 스튜디오를 통해 Equipment.java 파일을 실행합니다.
3. (안드로이드) 핸드폰에 해당 어플이 다운로드되면 어플이 실행됩니다.
<br>
<br>
<br>
<br>

### Prerequisites / 선행 조건

아래 사항이 설치가 되어있어야합니다.

```
1. Ubuntu 18.04 버전을 서버로 가지고 있어야 합니다.

2. 해당 서버에 머신러닝 폴더와 PHP 폴더를 다운로드 합니다.

3. 추가적으로 경로는 /var/html/www/아래에 다운로드 한다.

4. Host Computer와 서버가 연결할 수 있게 네트워크를 설정해줘야합니다.
```
<br>
<br>
<br>
<br>

### Installing / 설치

아래 개발 환경이 설정 되어 있어야 실행할 수 있습니다.

```
Host Coumputer : Android Studio
Server(ubuntu 18.04) : Python, Tensorflow, MySQL, php, Apache2
```
<br>
<br>
<br>
<br>

## Running the tests / 테스트의 실행

1. Android Studio를 통해 Equipment.java 파일을 실행하면 어플이 실행되고 사용할 수 있습니다.
2. 그 전에 몇가지 설정해야할 사항을 아래 표시합니다.
<br>
<br>
<br>
<br>

### 코드 변경 사항

```
1. Host Computer와 Guest Computer(Server)를 준비합니다.

2. Host Computer를 HC, Guest Computer는 서버라고 적겠습니다.

3. HC는 Android Studio만 다운로드 해줍니다.

4. 서버는 ubuntu:18.04 버전으로 OS를 설치해야합니다.

5. 서버에 위에 필요한 개발 환경들을 전부 다운로드해줍니다.

6. Github에 등록된 PHP(/var/html/www/) 파일과 머신러닝(/var/www/html/uploads) 파일을 해당 경로에 저장해줍니다.

7. /var/www/html/name.txt 파일을 만들어줍니다. (권한은 chmod 777)

8. MySQL을 다운로드 받은 후 php 폴더 안에 있는 dbcon.php를 보고 db이름, 테이블명 등을 설정해줍니다.

9. 머신러닝 폴더안에서 확인해야 할 파일은 online_detection_preprocessing.py입니다.

10. 해당 파일은 remove.bg(유료 api)를 사용해 이미지의 백그라운드를 지운 후 물체 인식을 진행하기 때문에 remove.bg 사이트에 로그인해 api 키를 얻고 진행해야합니다.

11. online_detection_preprocessing.py 파일 안에 X-Api-key : ~~~ 부분에 remove.bg api 키만 넣어주시면 실행이 됩니다.

12. 요약하여 설명했기 때문에 해당 파일들을 전부 확인해보시고 실행하시면 공부에 좀 더 도움이 될 것입니다. 혹시나 모르는 부분은 코멘트 및 이메일 남겨주시면 답변 드리겠습니다.
```
<br>
<br>
<br>
<br>

### 테스트는 이런 식으로 작성하시면 됩니다

```
혹시 비슷한 방식으로 머신러닝을 통해 프로젝트를 진행하시고 싶은 분들은 retrain_inceptionv3.py만 수정해서 클래스를 추가하시면 운동기구 분류가 아닌 동물, 식물, 등 여러 클래스를 분류할 수 있게 됩니다.
```

