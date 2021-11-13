# NH_competition
- Dacon에서 진행한 NH투자증권 제 1회 빅데이터 경진대회 ["AI야, 진짜 뉴스를 찾아줘!"](https://dacon.io/competitions/official/235658/overview/description) **수상**
- [League 1] 알고리즘 개발과 [League 2] 시각화 주제 중 `[League 1] 알고리즘 개발` 주제에 참가
- NH투자증권 본사에서의 결선 쇼케이스 발표 후 `League 2등 (리뽀 팀)`
- 대회 주제 : 뉴스 데이터 중 진짜 뉴스와 가짜 뉴스를 분류하는 Text Classification(딥러닝을 활용한 AI 뉴스 필터링 알고리즘 개발)

## Tutorial
1. About_NLP
2. Preprocessing
3. Vectorization
4. Word_Embedding
5. Modeling

## Data
- **NH투자증권이 제공한 데이터는 대회 종료 후 파기되었음**
- **한국어불용어.txt** : 여러 논문과 자료들을 참고하고 직접 수집하여 전처리한 불용어 데이터
- [GoogleNews-vectors-negative300.bin.gz](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit?resourcekey=0-wjGZdNAUop6WykTtMip30g) : Embedding Layer에 사용한 Google에서 제공한 Word Embedding 데이터
- [word-embeddings](https://drive.google.com/file/d/1yHGtccC2FV3_d6C6_Q4cozYSOgA7bG-e/view) : Fasttext, Glove, Word2vec, Swivel 데이터

## Submission
> 코드 순서
1. EDA
2. Preprocessing
3. Modeling
4. 확인용
5. 제출코드

## Trials
- AutoKeras
- TFBert
- GPT2
- SVM
- LightGBM 등

## 형태소 분석기 설치

1. KoNLPy == 0.5.2
- [KoNLPy](https://konlpy.org/ko/latest/install/) 공식 웹사이트 참고
```
$ python3 -m pip install --upgrade pip

$ python3 -m pip install konlpy
```
<br/>

2. MeCab(version : mecab of 0.996/ko-0.9.2)
```
$ bash <(curl -s https://raw.githubusercontent.com/konlpy/konlpy/master/scripts/mecab.sh)
```
<br/>

3. Mecab(eKoNLPy) == 0.0.1
- [eKoNLPy](https://github.com/entelecheia/eKoNLPy) 공식 깃허브 참고
```
$ git clone https://github.com/entelecheia/eKoNLPy.git

$ cd eKoNLPy

$ pip install .

$ pip install . --upgrade
```

