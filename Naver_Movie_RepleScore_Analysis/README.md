# <네이버 영화 평점 및 댓글 분석하기>

## 1. 데이터 크롤링

### 결과 : 영화코드값으로 모든영화 Reple 가져오기
  - https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_final.ipynb
  - url 영화 코드값 사용
  - 속도문제해결 위해 : ThreadPoll 사용
  - 정규화 사용 데이터 타겟팅 및 정제

### 과정 
1. 현재상영작 영화 Reple 1페이지 가져오기
 - https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_0827.ipynb
 
2. 특정영화 영화 Reple 1페이지 크롤링
 - https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_0828.ipynb
 
3. 현재 상영작 모든 영화 Reple 가져오기(동적 크롤링)
 - https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_0828_02.ipynb
 
4. 영화 평점 랭킹에서 Reple 가져오기(영화 코드값 활용)
 - https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/movie_reple_crawling_0830.ipynb

## 2. 데이터 병합
1. CSV 데이터 병합하기
 - https://github.com/Yumai-K/MyProject/blob/master/Naver_Movie_RepleScore_Analysis/merge_csv_data.ipynb
