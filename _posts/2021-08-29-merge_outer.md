## merge() - outer 옵션

함수의 옵션 이번엔 outer옵션을 줘서 id를 기준으로 합치되, 어느한쪽에라도 없는 데이터가 있는 경우 NaN값이 지정된다


```python
merge_outer = pd.merge(df1,df2, how='outer',on='id') 
```
