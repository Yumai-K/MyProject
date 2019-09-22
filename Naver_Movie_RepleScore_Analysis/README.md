# <네이버 영화 평점 및 댓글 분석하기>

## 1. 데이터 클롤링 및 정제

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
  2)[신경망 모델 만들기(create_model)]()
  
  3)[모델 테스트(model_test)]()
