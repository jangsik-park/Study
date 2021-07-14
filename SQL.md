# SQL

1. 연산 순서는 보통 안쪽에서부터 바깥쪽 순이다.
   DISTINCT한 값들만 COUNT하려면 DISTINCT 키워드를 COUNT괄호 안쪽에 넣는다.
   바깥쪽(SELECT문 다음에있는) DISTINCT는 이미 중복을 포함한 후의 COUNT 값에 대해 DISTINCT하는 것이다.
   
   EX) SELECT DISTINCT g.Name AS genre_name ,COUNT(**DISTINCT** i.CustomerId) AS 'The Number of customer_ID
