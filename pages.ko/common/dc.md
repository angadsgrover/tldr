# dc

> 임의 정밀도 계산기. 역방향 폴란드어 표기법(RPN)을 사용.
> 참고: `bc`, `qalc`.
> 더 많은 정보: <https://www.gnu.org/software/bc/manual/dc-1.05/html_mono/dc.html>.

- 대화형 세션 시작:

`dc`

- 스크립트 실행:

`dc {{경로/대상/스크립트.dc}}`

- 지정된 척도를 사용하여 표현식을 계산:

`dc --expression='{{10}} k {{5 3 /}} p'`

- 4 곱하기 5 (4 5 \*)를 계산하고, 17 (17 -)을 뺀 후에, 결과값을 출력([p]rint):

`dc --expression='4 5 * 17 - p'`

- 소수 자릿수를 7 (7 k)로 지정하고, 5를 -3 (5 \_3 /)으로 나눈 다음, 결과값을 출력([p]rint):

`dc --expression='7 k 5 _3 / p'`

- 황금비, phi를 계산: 소수 자릿수를 100 (100 k)으로 설정하고, 5 (5 v) 더하기 1 (1 +)의 제곱근을 2 (2 /)로 나눈 후, 결과값을 출력([p]rint):

`dc --expression='100 k 5 v 1 + 2 / p'`
