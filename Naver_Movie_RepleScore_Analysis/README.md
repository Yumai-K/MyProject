# <네이버 영화 평점 및 댓글 분석하기>

## 결과 파일 다운 클라우드 
 - [학습완료 모델](https://drive.google.com/file/d/1Vm6r-F_0CRMHUrKLOzVDuUlgzF7Yg32j/view?usp=sharing)
 - [테스트 코드](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/model_test.ipynb)
 - [데이터 파일1 : test_set](https://drive.google.com/open?id=1BttX5LnNLX5tvHuM9q8imcb4pQB4c26g)
 - [데이터 파일2 : word2idx](https://drive.google.com/open?id=113X1nL58V8GWHVldBYCzUS_0bJrxR9QJ)
 - [크롤링 전체 데이터 : final_data_contents](https://drive.google.com/open?id=1zB1xwLnfzi5uUtMgCNGI8IIXznSc087j)
 
 
## 과정1. 데이터 클롤링 및 정제

 #### 크롤링 하기
  1)[영화코드값으로 영화 댓글 및 평점 가져오기](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_final.ipynb)
 #### 크롤링 데이터 병합 및 정제
  2)[코드값 별로 분류된 데이터 1개 csv파일로 병합](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/merge_csv_data.ipynb)
  
  3)[불필요 컬럼 제거](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/refine_csv.ipynb)
  
  4)[contents 내용 정제](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/refine_contents.ipynb)

  - url 영화 코드값 사용
  - 속도문제해결 위해 : ThreadPoll 사용
  - 정규 표현식 사용 데이터 타겟팅 및 정제


## 2. 입·출력 및 신경망 모델 생성

 #### Word2idx 생성하기
  1)전체 댓글의 단어별 빈도수를 기준으로 정렬한 데이터 만들기
      - [Word2idx - Step01](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/make_word2idx_step01.ipynb)
      - [Word2idx - Step02](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/make_word2idx_step02.ipynb)

  #### 학습 모델 생성 및 테스트
  2)[신경망 모델 만들기](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/create_model.ipynb)
  
  3)[모델 테스트](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/model_test.ipynb)
