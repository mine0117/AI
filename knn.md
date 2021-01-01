# knn

**fish_data = [[l, w] for l, w in zip(length, weight)]**    
(사이킷런(scikit-learn)을 사용하기 위해 2차원 리스트를 만들기)

**fish_target = [1]*35 + [0]*14** 

(머신러닝 알고리즘을 통해 생선의 길이와 무게를 보고 도미와 빙어를 찾는 규칙을 원하기 때문에, 도미와 빙어가 무엇인지 알려주어야함 따라서, 도미와 빙어를 숫자 1과 0으로 표기(도미 : 1, 빙어 : 0) 

**kn.fit(fish_data, fish_target)**
(사이킷런(scikit-learn)의 훈련 메서드(fit)

**kn.score(fish_data, fish_target)** 
(모델을 평가하는 메서드로서 0에서 1사이의 값을 반환, 1은 모든 데이터를 모두 맞힌것)

**kn.predict([[30, 600]])** 
(predict는 새로운 데이터의 정답 예측)
