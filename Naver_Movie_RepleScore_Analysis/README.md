# <네이버 영화 평점 및 댓글 분석하기>

## 1. 데이터 크롤링

### [결과 : 영화코드값으로 모든영화 Reple 가져오기](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_final.ipynb)
  - url 영화 코드값 사용
  - 속도문제해결 위해 : ThreadPoll 사용
  - 정규화 사용 데이터 타겟팅 및 정제

### 과정 
1. [현재상영작 영화 Reple 1페이지 가져오기](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_0827.ipynb)
 
2. [특정영화 영화 Reple 1페이지 크롤링](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_0828.ipynb)
 
3. [현재 상영작 모든 영화 Reple 가져오기(동적 크롤링)](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_0828_02.ipynb)
 
4. [영화 평점 랭킹에서 Reple 가져오기(영화 코드값 활용)](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_0830.ipynb)

## 2. 데이터 병합
  - 영화별로 크롤링된 데이터 하나의 csv파일로 병합
  - 영화제목(movie), 댓글내용(contents), 평점(score)를 제외한 컬럼 제거
  - 댓글내용(contents)에서 한글을 제외한 값들 제거
  
1. [CSV 데이터 병합하기](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/merge_csv_data.ipynb)
2. [데이터 정제 : 불필요 컬럼 제거](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/refine_csv.ipynb)
3. [데이터 정제 : contents 컬럼 내부 정제](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/refine_contents.ipynb)

## 3. 신경망 입력 데이터 만들기
1. 전체 댓글의 단어별 빈도수를 기준으로 정렬한 데이터 만들기
      - [Word2idx - Step01](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/make_word2idx_step01.ipynb)
      - [Word2idx - Step02](https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/make_word2idx_step02.ipynb)
