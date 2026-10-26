<font color='purple' size=2.5><i>2024년 8월 업데이트</i></font>
![Presentation1](https://user-images.githubusercontent.com/59842360/159695863-678be5bc-d146-4340-9592-003ad93241e1.jpg)
# 선형대수 강의

이 강의 노트는 선형대수 입문 수업을 위한 자료로, 대학생, 프로그래머, 데이터 분석가, 알고리즘 트레이더 등에 적합합니다.

이 강의 노트는 다음 교재들을 참고했습니다.

1. Gilbert Strang의 <b><i>Linear Algebra and Its Applications</i></b>
2. David Lay의 <b><i>Linear Algebra and Its Applications</i></b>
3. DeFranza & Gagliardi의 <b><i>Introduction to Linear Algebra With Applications</i></b>
4. Gareth Williams의 <b><i>Linear Algebra With Applications</i></b>

![cover-min](https://user-images.githubusercontent.com/59842360/83939172-64df6c00-a7e3-11ea-80b1-058af696d5a3.png)

이 강의의 핵심은 정리를 증명하는 것보다 개념을 실제로 활용하고 시각화하는 데 있습니다. 엄밀한 추론이나 표기법에 집중하기보다는 이해하기 어려운 개념을 명확히 설명하려고 합니다. Python/MATLAB 덕분에 이 작업도 훨씬 쉬워졌습니다.

## 선수 지식
초보자를 위한 강의이지만, 선형대수와 미적분을 어느 정도 접해 봤다면 도움이 됩니다.

또한 다음 도구에 대한 기본 지식이 필요합니다. 약 3일 정도 학습한 수준이면 충분합니다.
- [x] Python
- [x] NumPy
- [x] Matplotlib
- [x] SymPy

모든 코드는 효율성이나 전문적인 코딩 스타일보다 <b>직관적인 이해</b>를 우선해 작성했습니다. 따라서 코드는 매우 단순하고 이해하기 어렵지 않을 것입니다.

## 환경 설정
저는 Poetry로 환경을 관리합니다. 저처럼 VS Code를 사용한다면 다음 순서대로 진행하세요.
1. Windows PowerShell에서 ``` (Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -p```를 실행해 Poetry를 설치합니다.
2. ```cd $env:APPDATA\Python\Scripts```로 이동해 Poetry가 설치되었는지 확인합니다.
3. ```notepad $profile```로 프로필을 열고, 메모장에서 ```Set-Alias poetry "C:\Users\user\AppData\Roaming\Python\Scripts\poetry.exe"```를 추가합니다. Windows에서는 환경 변수 경로 설정이 작동하지 않을 때가 있어 이 방식을 사용합니다.
4. ```. $profile```로 프로필을 다시 불러옵니다.
5. 개인 컴퓨터라면 ```Set-ExecutionPolicy RemoteSigned -Scope CurrentUser```를 실행해 실행 정책의 제한을 완화하고 `Y`를 선택합니다.
6. 보안을 위해 ```Set-ExecutionPolicy Restricted -Scope CurrentUser```로 기본 제한 정책을 복원합니다.
7. ```poetry --version```을 실행해 버전이 출력되는지 확인합니다.
8. ```poetry update```를 사용하거나, 원하는 방식으로 버전을 관리합니다.

## 이 강의 노트에서 배울 내용
이 강의 노트는 선형대수에 크게 의존하는 Data Science, Econometrics, Mathematical Statistics, Financial Engineering, Control Theory 등의 분야를 공부하는 데 필요한 기초 지식을 다룹니다. 튜토리얼을 차근차근 따라가면 선형대수의 기본 개념을 더 잘 이해할 수 있을 것입니다. 그다음에는 자신의 분야에 맞춰 특수한 행렬과 그 활용법을 공부해 보세요.

## 목차
더 편하게 읽으려면 웹사이트를 방문해 주세요: [Linear Algebra for Python](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/linear-algebra-index)<br>
[1장 - 선형 방정식계](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%201%20-%20Linear%20Equation%20System)<br>
[2장 - 기초 행렬 대수](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%202%20-%20Basic%20Matrix%20Algebra)<br>
[3장 - 행렬식](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%203%20-%20Determinant)<br>
[4장 - LU 분해](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%204%20-%20LU%20Factorization)<br>
[5장 - 벡터의 덧셈, 뺄셈과 스칼라 곱](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%205%20-%20Vector%20Addition%2C%20Subtraction%20and%20Scalar%20Multiplication)<br>
[6장 - 선형 결합](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%206%20-%20Linear%20Combination)<br>
[7장 - 선형 독립](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%207%20-%20Linear%20Independence)<br>
[8장 - 벡터 공간과 부분 공간](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%208%20-%20Vector%20Space%20and%20Subspace)<br>
[9장 - 기저와 차원](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%209%20-%20Basis%20and%20Dimension)<br>
[10장 - 영공간, 열공간, 행공간과 계수](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2010%20-Null%20Space%20vs%20Col%20Space%2C%20Row%20Space%20and%20Rank)<br>
[11장 - 선형 변환](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2011%20-%20Linear%20Transformation)<br>
[12장 - 고유값과 고유벡터](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2012%20-%20Eigenvalues%20and%20Eigenvectors)<br>
[13b장 - 주성분 분석](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2013b%20-%20Principal%20Component%20Analysis)<br>
[13a장 - 대각화](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2013a%20-%20Diagonalization)<br>
[14장 - 동적 시스템에의 응용](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2014%20-%20Applications%20to%20Dynamic%20System)<br>
[15장 - 내적과 직교성](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2015%20-%20Innear%20Product%20and%20Orthogonality)<br>
[16장 - Gram-Schmidt 과정과 QR 분해](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2016%20-%20Gram-Schmidt%20Process%20and%20QR%20Decomposition)<br>
[17장 - 대칭 행렬, 이차 형식과 Cholesky 분해](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2017%20-%20Symmetric%20Matrices%20%2C%20Quadratic%20Form%20and%20Cholesky%20Decomposition)<br>
[18장 - 특이값 분해](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2018%20-%20The%20Singular%20Value%20Decomposition)<br>
[19장 - 다변량 정규분포](https://www.weijiechen.com/tutorials/linear-algebra-with-python-book/qmd/Chapter%2019%20-%20Multivariate%20Normal%20Distribution)<br>

## 화면 예시
![截图01](https://user-images.githubusercontent.com/59842360/122352881-6b043e80-cf47-11eb-9ca4-8f52c93c0efa.jpg)
![截图03](https://user-images.githubusercontent.com/59842360/122352926-78212d80-cf47-11eb-9bb4-c33e03b7f085.jpg)
![截图00](https://user-images.githubusercontent.com/59842360/122352940-7b1c1e00-cf47-11eb-9f80-e26454d4baaf.jpg)
![截图00](https://user-images.githubusercontent.com/59842360/126001287-9f8de290-3940-4000-b5db-7b12d8b70005.jpg)
![截图01](https://user-images.githubusercontent.com/59842360/126001290-d342db9f-76eb-41ce-98b2-208075bd4640.jpg)
![截图02](https://user-images.githubusercontent.com/59842360/126001291-5cee0e1b-d02b-4912-9d27-65eaaff13178.jpg)
![截图03](https://user-images.githubusercontent.com/59842360/126001463-0b262316-0032-482e-bb0f-1ccbbd3a2835.jpg)
