### 표 구성
* <td>: table data. 셀 내용 
    - 내용은 전부 td로 묶어줘야 함
* <tr>
    - 같은 열끼리 묶어준다.

*html tag wrap 확장프로그램
    => alt + w 

* <caption>
    - 테이블의 제목이나 설명
    - 반드시 첫번째 자식으로 사용
    - 선택적으로 사용

---
### 의미 구성
*<thead> : 열 그룹 -> 칼럼명 묶어주기
*<tbody> : 테이블 데이터 모음 -> 데이터 묶어주기
*<tfoot> : 요약
이 세 코드의 순서를 바꿔도 상관 없어지지만, 가독성 위해 순서 맞추자.
* <th> 행 1열 -> <td>를 <th>로 바꿔주기
    상위 행 제목이 있지 않으면 궂이  

---

### 셀 병합

* collspan
    행에 나란한 열들 병합해줄 때 사용
    같은 tr 내에서 사용
* rowspan
    열에 나란한 행을 병햅해줄 때 사용

---
### scope
* scope 속성
    은 th 태그에 사용하여 헤더가 어떤 셀에 대한 제목셀인지 명확하게 지정
   -  scope="col": 열 헤더를 정의합니다.
    - scope="row": 행 헤더를 정의합니다.
    - scope="colgroup": 열 그룹 헤더를 정의합니다.
    - scope="rowgroup": 행 그룹 헤더를 정의합니다.

---

### 순서
* 다중지정 : ctl + d
* 다중커서 : alt + click
1. table>td*n 
2. 왼쪽 위부터, 세로로 <td> 데이터 쭉 작성
    - 공백은 &nbsp;
4. 열 갯수만큼 <tr>로 wrap 해주기
5. <thead>, <tbody>, <tfoot>묶기
6. colspan, rowspan 병합
7. <th>
8. <th scope>
    - 열 제목: col
    - 열 제목 그룹: colgroup -> 셀이 하나밖에 없다면 그냥 col로 해도 됨.

---

### 표 접근성 높이기
* <caption>
    - 반드시 넣기
    - 무조건 table의 첫번째 자식으로. 스크린 리더 고려하여.
* scope, th 엘레멘트 사용
* thead, tbody, tfoot 구조화

