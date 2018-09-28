# ch02
- 2018-08-17
- Junmo Kim
- [Convolutional Neural Network (CNN)]
    
    - 실습1 (SIIT_KAIST_CLS)
        - 실습자료 다운 : https://goo.gl/ccE8hG
        - 압축해제
        - 노트패드 다운
        - tab 크기 4->2로 변경
        - cmd창에서 SIIT_KAIST_CLS 폴더경로로 이동
        - 명령실행 : python main.py

    - 실습2 (SIIT_KAIST_GAN)    
        - cmd창에서 SIIT_KAIST_GAN 폴더경로로 이동
        - 명령실행 : python main.py
        - 학습과 동시에 vis 폴더에 학습결과가 이미징된다.
          점점 선명해진다.

    - 보고서 제출 >> Yekang Lee : askhow@kaist.ac.kr
    - 설문조사 : https://goo.gl/YTNcQk

- Gen 참고서적 : www.deeplearningbook.org

# ch03
- 2018-08-24
- 유창동 교수님
- [Recurrent Neural Network / Long Short-Term Memory]

    - 실습1
        - 실습자료 다운 : https://drive.google.com/file/d/17Nxx9NaDu_IxOpiJyfQqPumZlouSoOqS/view
        - 테스트 1
            INPUT_SIZE    = 9
            OUTPUT_SIZE   = 9
            HIDDEN_SIZE   = 100
            LEARNING_RATE = 0.005
            nEpoch 	      = 500

        - 테스트 2
            INPUT_SIZE    = 9
            OUTPUT_SIZE   = 9
            HIDDEN_SIZE   = 100
            LEARNING_RATE = 0.01
            nEpoch 	      = 500

        - 테스트 3
            INPUT_SIZE    = 9
            OUTPUT_SIZE   = 9
            HIDDEN_SIZE   = 200
            LEARNING_RATE = 0.01
            nEpoch 	      = 500
    - 보고서 제출 >> junyeong.kim@kaist.ac.kr


# ch04
- 2018-09-07
- 박현욱 교수님
- [Medical Imaging Systems]

    - Google's principles for developing AI
    - Be socially beneficial
    - Avoid creating or reinforcing unfair bias
    - Be built and tested for safety
    - Be accountable to people (interpretability)
    - Incorporate privacy design principles
    - Uphold high standards of scientific excellence
    - Be made available for uses that accord with these principles

    - positron ?

    - 실습
        - 실습자료 : http://35.229.152.185:5000/
        1. FCN(Fully Convolutional Network)
        - 간단하나 정밀도가 떨어짐
        
        2. U-Net
        - 레이어가 많고 정밀함

    - Keras Library
        - 모듈화
        - 최소주의
        - 쉬운 확장성
        - 파이썬 기반

# ch05
- 2018-09-14
- 김기응 교수님
- [Reinforcement Learning]
    - Machine Learning
        1. Supervised Learning
            - Object Detection
            - Object Localication
        2. Unsupervised Learning
            - GAN
                - nvidia celeba : 유명인들 이미지를 보고 가상인물 이미지 생성
        3. Reinforcement Learning
    - 실습 1
        - 실습자료 : https://github.com/KAIST-AILab/deeprl_practice
        - https://jupyter.nims.re.kr 접속
        - new > terminal > git clone https://github.com/KAIST-AILab/deeprl_practice
        - $ cd deeprl_practice
        - $ conda env create -f environment.yml : 실습에 필요한 모듈 설치(꽤 오래걸림)
        - $ source activate deeprl : 가상환경 활성화
        - $ python setup.py install : gym-maze 설치
        - $ cd baselines : baselines 설치
          $ pip install -e .
          $ cd ..
        - $ python -m ipykernel install --user --name deeprl --display-name deeprl : Jupyter notebook에 가상환경 커널 추가
        - https://jupyter.nims.re.kr > deeprl_practice폴더 > 1_Q-learning_maze.ipynb 실행
        - 메뉴에서 Kernel > Change kernel > deeprl 선택
        - 교재에 나온 Problem1,2,3 코딩 후 'learn_q_val()' 코드 실행하면 maze가 시각화되어서 출력됨
    - 실습 2
        - OpenAI : deeprl_practice/baselines/baselines
          >> 여기서 RL알고리즘을 골라서 사용하면 됨
        - 
    - 보고서 제출 : hvlee@ai.kaist.ac.kr        

# ch07
- 2018-09-28
- 김회린 교수님
- [음성인식]
    - 실습
        - 실습메뉴얼 : goo.gl/ZpeDU7
        - 실습파일 : kaist_kaldi_tutorial.ova (via goo.gl/g8xSDP or goo.gl/vVqiPe)
        - VitrtualBox(Ubuntu) + Kaldi
        - KALDI 
            - 대표적인 음성인식/화자인식용 오픈소스 툴킷
            - 대부분 Shell script, C++ (일부 python)    
            - 음성인식에 필요한 전처리/후처리에 필요한 여러 Lib를 갖추고 있음
            - 다양한 음성 데이터에 맞는 recipe/tutorial이 존재
            - http://kaldi-asr.org
            - https://github.com/kaldi-asr/kaldi
        - 그 외
            - CMU Sphinx : 2000년대 사용사던 오픈소스 툴킷 (C/Java/Python)            
            - HTK : 과거 주로 쓰였던 HMM 기반 음성인식 툴킷으로 라이센스 필요
        - Database
            - FSDD (Free Spoken Digit Dataset)
                - 음성인식을 위한 MNIST : Digit recognition task (0~9)
                - 사용할 샘플 : https://github.com/Jakobovski/free-spoken-digit-dataset
        - Ubuntu Login PW : 123450
            - $ cd kaldi/egs/fsdd
            - $ ./run.sh    
            
            
