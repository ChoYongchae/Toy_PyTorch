PyTorch 연습장
=========

+ 연구실 생활(2018~2020)동안에는 주로 tensorflow 1.x 버젼을 사용했는데, 졸업할때 즈음에는 많은 논문들의 공식 배포 코드가 pytorch로 구현된 것을 느낌
+ 논문에서는 자세히 서술되지 않은 내용들을 살펴보기 위해서는 공식 배포 코드를 보는 것이 제일 편한데, 이를 위해 PyTorch에 더 익숙해지고 싶음
+ 많은 연구자들이 pytorch로 연구하는 이유를 직접 느껴보고 나도 이를 활용하여 재밌는 프로젝트들을 진행해보고 싶음


하드웨어 환경
============
+ AMD Ryzen 5 3600
+ NVIDIA Geforce GTX1660 Super
+ RAM 16G(8+8)
+ HDD

환경 설치(Windows 10)
============
+ https://www.anaconda.com/products/individual   
    - tensorflow, pytorch 등의 여러 개발 환경들을 번갈아 사용하기 위해서 패키지/의존성 관리를 도와주는 anaconda를 사용
    + anaconda prompt 입력 명령어
        <pre>
        <code>

        // 원하는 경로로 이동
        (base)D:
        (base)cd study


        // 개발 환경 생성
        (base)conda create -n pytorch python=3.7 // y

        // 생성한 개발 환경으로 들어가기
        (base)conda activate pytorch

        // https://pytorch.org 에서 설치 명령어 확인 가능
        (pytorch)conda install pytorch torchvision cudatoolkit=10.2 -c pytorch // y

        // 그래프, 그림을 그려주는 라이브러리 설치
        (pytorch) conda install matplotlib // y

        // 웹기반 인터랙티브 실행환경 설치
        (pytorch) conda install jupyter notebook // y

        // 쥬피터 노트북 실행
        jupyter notebook
        </code>


1_DCGAN
===============
+ https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html
+ 제일 재밌어 보이는 DCGAN 기반 얼굴 생성 예제를 첫 연습으로 선정



utils
===============
+ crawling.py, chromedriver.exe: 구글 이미지 검색을 통해서 데이터셋 수집


기타 참조
==============
+ 마크다운 작성
    - https://gist.github.com/ihoneymon/652be052a0727ad59601
+ VSCode로 마크다운 미리보면서 작성하기
    - https://m.blog.naver.com/PostView.nhn?blogId=ndb796&logNo=221420270061&proxyReferer=https:%2F%2Fwww.google.com%2F