# 챗봇 학습툴 구현
챗봇의 학습 데이터를 관리하는 툴을 제작한다

* ### __프로젝트 구조__
```
chatbot
    |-----train_tols : 챗봇 학습 툴 관련 파일
    |-----models     : 챗봇 엔진에서 사용하는 딥러닝 모델 관련 파일
    |        |-----intent : 의도 분류 모델 관련 파일
    |        |-----ner    : 개체 인식 모델 관련 파일
    |-----utils      : 챗봇 개발에 필요한 유틸리티 라이브러리
    |-----config     : 챗봇 개발에 필요한 설정
    |-----test       : 챗봇 개발에 필요한 테스트 코드
        
```

* ### __DB(Mysql) 테이블 : chatbot_train_data__
|컬럼|속성|설명|
|--|--|--|
|id|int primary key not null| 학습 데이터 id|
|intent|varchar(45)|의도명, 의도가 없는 경우 null|
|ner|varchar(45)|개체명, 개체명이 없는 경우 null|
|query|text null|질문 텍스트|
|answer|text not null|답변 텍스트|
|answer_image|varchar(2048)|답변에 들어갈 이미지 URL, 이미지 URL 사용 안할 시 null|