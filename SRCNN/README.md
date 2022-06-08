# SRCNN 학습 진행

## 0. 사전준비
- Database 다운로드: DB.zip ([링크](https://drive.google.com/file/d/1b5XSQaOu2ku-MCC9Si6q0RyAk1RLxcP1/view?usp=sharing))
```bash
SRCNN
└── DB
    ├── train
    │   ├── hr
    │   └── lr
    └── test
        └── lr
``` 
- https://github.com/gymlab/ai_intro 에서 코드를 다운로드 (SRCNN 폴더의 train.ipynb, eval.ipynb를 업로드할 준비)
- Google Drive에 `SRCNN` 폴더 만들기
- 다운로드 받은 `train.ipynb`, `eval.ipynb`, `DB.zip` 파일을 `SRCNN` 폴더 안에 업로드 (압축 해제 코드는 train.ipynb에 있음)

## 1. Colab을 사용하여 train.ipynb 실행
- `수정 > 노트 설정` 에서 하드웨어 가속기를 GPU로 설정 후 저장
- 우측 상단에서 연결을 클릭
- 첫번째 셀은 Google Drive를 마운트 하는 코드
- 두번쨰 셀은 DB.zip의 압축을 해제하는 코드. 이 코드는 최초에 압축 해제시에만 사용하고, 압축해제 이후에는 사용하지 않으므로 주석(#)을 사용하여 비활성화 함.
- 각 셀을 수행하여 학습 진행 (모두 실행 단축키는 `Ctrl + F9`)
- 제공된 코드를 기반으로 프로젝트를 수정하여 새로운 모델을 학습 (구조, 하이퍼 파라미터 등 다양하게 변경)

## [참고] 제공된 코드의 Validation 성능: PSNR 27.4

# SRCNN 테스트 진행
## 1. Colab을 사용하여 eval.ipynb 실행
- `수정 > 노트 설정` 에서 하드웨어 가속기를 GPU로 설정 후 저장
- 우측 상단에서 연결을 클릭
- 첫번째 셀은 Google Drive를 마운트 하는 코드
- 각 셀을 수행하여 테스트 진행 (모두 실행 단축키는 `Ctrl + F9`)
- SRCNN의 results 폴더에 테스트 영상이 생성 (총 685장)
- results 폴더를 다운로드 받아서 압축하고 `학번_이름.zip`으로 압축 파일명 변경하여 제출
- 제출 (swkim@pknu.ac.kr)