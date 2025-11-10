# Multi_Class_Classification_Example

## 핵심 개념 정리

### 1. Batch Normalization
```python
각 층의 출력을 정규화하여 학습 안정화
장점:
- 더 높은 학습률 사용 가능
- 초기 가중치에 덜 민감
- 정규화 효과 (Dropout과 유사)
```

### 2. Learning Rate Scheduler
```python
학습 중 학습률을 동적으로 조정
ReduceLROnPlateau: 검증 손실 개선이 멈추면 학습률 감소
효과: 세밀한 최적화 가능, 로컬 미니멈 탈출
```

### 3. Early Stopping
```python
검증 손실이 개선되지 않으면 학습 조기 종료
장점:
- 과적합 방지
- 학습 시간 절약
- 최적 모델 자동 선택
```

### 4. 혼동 행렬 해석
```python
대각선: 올바른 예측
비대각선: 잘못된 예측

예시: [실제: 8, 예측: 3]이 많다면?
→ 8과 3이 시각적으로 유사할 가능성
```

### 5. Precision vs Recall
```python
Precision (정밀도):
"예측이 얼마나 정확한가?"
스팸 필터: 정상 메일을 스팸으로 잘못 분류하면 안 됨

Recall (재현율):
"실제 양성을 얼마나 잘 찾아내는가?"
질병 진단: 환자를 놓치면 안 됨
```

### 6. F1-Score
```python
Precision과 Recall의 균형
불균형 데이터셋에서 유용
1에 가까울수록 좋은 성능
```
