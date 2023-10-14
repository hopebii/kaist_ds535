**[Recsys 2023] Trending Now: Modeling Trend Recommendations**

**논문 선정 이유** 

▢  **Research topic** : 'trending now' 

최근 추천시스템에서는 일반적으로 "현재 인기있는 상품 (trending now)" 과 같은 별도의 추천 항목을 제시해주어 해당 상품의 인기를 높여 활성유저를 유치하고 있습니다. 그러나 일반적으로 "시간 간격 내 interaction 수" 와 같은 단순한 휴리스틱 방법을 기반으로 추천해주기 때문에 개선의 여지가 많이 남아있으며, 추천시스템에서 trend 를 모델링하는 연구는 제한적으로 이루어져 있습니다.  따라서 해당 논문은 **시계열 예측** 이라는 새로운 관점에서 trend 를 반영한 추천시스템 모델을 제안합니다. item trendiness 에 대한 정의를 통해 trend recommendation task 를 one-step time series forecasting 문제로 공식화합니다. item 의 미래 trend 를 예측하고 추천 리스트를 생성하는 deep latent variable 모델인 TrendRec 을 제안합니다.
현재 시점에서의 trend 를 파악하고 유저에게 관련 item 을 추천하는 것을 시계열 예측으로 접근한 관점이 신선했고, "acceleration" 이라는 개념을 정의하여 인기가 "빠르게 상승" 하고 있고 가까운 미래에 인기를 얻을 가능성이 있는 item 을 추천한다는 아이디어가 참신한 것 같아 해당 논문을 선정하게 되었습니다. 


### 1. Introudction 

#### 1-a. Definition 

|용어|내용| 
|------|---| 
|Popularity|특정 시간 간격의 상호작용 횟수| 
|trend in the recommendation context |인기도 (popularity) 또는 가속도 (acceleration) 변화율| 
|trending now|현재 시점에서 점점 더 많은 interaction 이 발생하는 item 이지만, 반드시 가장 인기있는 item 을 뜻하진 않는다. popularity bias 없이 효과적으로 item 을 탐색한다.| 

#### 1-b. Challenge 
 
▢  **Problem**: 현재 트렌드를 안정적이고 신뢰성 있게 파악하기 위해서는 충분한 상호작용을 수집하는 데 일정 시간이 필요하며, 트렌드는 역동적으로 변화하고 데이터 수집 기간 동안 변동이 있을 수 있다. 

▢  **Solution** : trend recommendation 을 one-step forecasting problem 으로 공식화한다. 


#### 1-c. Problem setting : One-step forecasting problem 

![image]()

### 2. Preliminaries 


### 3. Model : collaborative time series forecasting model with user-item interactions (TRENDREC)


### 4. Experiments


### 5. Conclusion



**논문 요약** 
**나의 의견** (ex. 만약 Spectral GNN에 대해 관심이 있으시거나 어느정도의 배경지식을 갖고 계신 분이라면 많은 것을 얻어갈 수 있는 논문이라고 생각합니다. 가장 마음에 들었던 부분은 핵심인 Universality보다도, 최적화 측면에서 표현력이 같은 기존 spectral GNN들의 실험적 성능에 차이가 생길 수밖에 없는 이유를 분석하고 JacobiConv를 motivate한 부분이었습니다.그렇지만 이 논문에서도 아쉬웠던 부분이 없지는 않았습니다.이런 아쉬운 점도 있었지만, 그래도 이 논문이 갖는 가치는 엄청나다고 생각하고, Spectral GNN이라는 분야가 발전함에 있어 중요한 분기점 중 하나가 될 연구라고 생각합니다. )



#### Review writer information 
- 이다현 (Lee Dahyeon) 
  - Master student, Department of Data science, KAIST 
  - contact : isdawell@kaist.ac.kr 
