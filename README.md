# Django-DRF-1

장고 DRF 특강 1일차 과제

=============================================================================

1. args, kwargs를 사용하는 예제 코드 짜보기

 first with args
args = ("two", 3, 5)
>>> test_args_kwargs(
args)
arg1: two
arg2: 3
arg3: 5

 now with kwargs:
>>> kwargs = {"arg3": 3, "arg2": "two", "arg1": 5}
>>> test_args_kwargs(kwargs)
arg1: 5
arg2: two
arg3: 3

================================================================================

2. mutable과 immutable은 어떤 특성이 있고, 어떤 자료형이 어디에 해당하는지 서술하기

mutable = 값이 변한다는 뜻
immutable = 값이 변하지 않는다는 뜻


mutable : 딕셔너리, 리스트
immutable : 숫자형, 문자열, 튜플 

================================================================================

3. DB Field에서 사용되는 Key 종류와 특징 서술하기

FK: Foreign Key의 약자이며, 다른 테이블을 참조 할 때 사용된다.

UK: Unique Key의 약자이며, 중복 값을 허용하지 않는다.

PK: Primary Key의 약자이며, 테이블에서 반드시 존재해야 한다.
   > PK는 2개 이상 존재 할 수 없고, UK와 마찬가지로 중복 값을 허용하지 않는다.
   > Foreign Key를 사용할 경우 참조 할 테이블의 PK를 바라본다.

================================================================================

4. django에서 queryset과 object는 어떻게 다른지 서술하기

field is object
오브젝트 is 객체
class Review > Class -- a blueprint for objects
Review.objects.all() > 쿼리셋
Review.objects.get(name=) > 쿼리셋에 필터 적용
