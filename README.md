# 마켓컬리 구매후기로 살펴보는 육가공품 제품행태 조사
<img src="https://user-images.githubusercontent.com/71205453/110089117-0f1f0b00-7dd9-11eb-8238-33760918078b.png"  width="600" height="300">   

### 1. 마켓컬리를 데이터 셋으로 선정한 이유
마켓컬리를 볼때마다 늘 느끼는 점은 정말 상품평이 많습니다.   
컬리는 고객 상품후기를 경영활동 전반에 활용도가 매우 높은곳으로 알려진 기업입니다.   
그래서 데이터를 굉장히 중요시하는 기업으로 포인트 적립을 통해 고객상품후기를 모으고 있는 곳 입니다.   
마켓컬리 데이터들의 특징은 20~30대 여성들의 제품과 관련된 소비자의 라이프 스타일을 가늠할 수 있는 데이터 셋 입니다.

### 2. 워드클라우드 사용시 주의할 점
<pre><code>market_kurry_stopwords = ['하몽', '컬리', '고객', '마켓', '배송', '진짜', '주문' , '구매' , '보고', '자주', '말씀',
                          '상품', '후기' , '살짝']
for stopword in market_kurry_stopwords:
    stopwords.append(stopword)
    
remove_char_counter = Counter({x :remove_char_counter[x] for x in count if x not in stopwords})</code></pre>   

워드 클라우드를 사용할때는 중요한 의미를 지니지 않는 불용어(stopwords)를 데이터 시각화에서 제외해주는 작업을 꼭 거쳐야 합니다.   

### 3. 결과 및 해석
![image](https://user-images.githubusercontent.com/71205453/110098443-8ce81400-7de3-11eb-8dce-a903050b8748.png)
![image](https://user-images.githubusercontent.com/71205453/110098561-b0ab5a00-7de3-11eb-82fc-8732ad94368f.png)
