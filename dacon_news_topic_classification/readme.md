# DACON 뉴스 토픽 분류 competition

#task flow

### 7/9 
    preprocessing :Mecab/  keras tokenizer
    LSTM

### 7/11
    * preprocessing : tfidf tokenizer / doc2vec
    
    * Model
        Random Forest
        Logistic Regression** val_score 기준 0.79~0.83
        LGBM
        XGB
        Adaboost
        bagging classifier

### 7/12
    하이퍼 파라미터 튜닝

### 7/13~17
    * preprocessing : Mecab(Morphs, Nouns) , keras tokenizer
    
    * Model
        Conv1D CNN. Ref. Yoon Kim
            - embedding - dropout - Conv1D - Maxpooling/ (Averagepooling) - FC - dropout - output
        Conv2D CNN
        Bidirectional LSTM

        val_score 기준 0.7~0.82 / submission score 기준 ~0.78

### 7/17~19
    tfidf + logistic regression searchgridcv(CV=3) 파라미터 튜닝 
    submission score : 0.79XX -> 0.80XX
    
    stacking 예정


