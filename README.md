1. 게임이름과 컨셉

-제목 I WANNA DO BOSSRUSH (IWDB) (원작 I WANNA BE THE BOSHY (IWBTB))

<img src="https://user-images.githubusercontent.com/37091845/94274990-61821300-ff81-11ea-9280-c22e3c6a2f6b.png" alt="보시" style="zoom: 80%;" />

- 게임의 컨셉은 키보드만을 이용해 사용자의 컨트롤을 극한으로 끌어 올리는 것 입니다.

- 게임의 핵심 메카니즘은 패턴을 피하며 총알을 발사해

  보스를 잡는것입니다.

---

2. **GAMESTATE(SCENE)의 수 및 각각의 이름**

Scene의 수 : 6개

a.Logo Scene

b.게임 시작 전 Scene

c.보스 선택 가능 Scene

d.보스와의 싸움 Scene

e.랭킹 Scene

f.일시중지 Scene

---

3.

각 Scene 끼리의 이동 가능 도시화

<img src="https://user-images.githubusercontent.com/37091845/94274814-1d8f0e00-ff81-11ea-8fc4-7b7b6721fce1.png" alt="도식화" style="zoom: 50%;" />



a.게임 시작전 Scene

게임시작,랭킹,게임종료 3가지 선택을 할 수 있는 Scene 

<img src="https://user-images.githubusercontent.com/37091845/94274977-5e872280-ff81-11ea-8b05-acd4b60a54c4.png" alt="게임시작전" style="zoom: 50%;" />

b. 보스 선택 Scene (삭제)

보스를 선택하는 Scene

Enter 시 보스 싸움 Scene으로 간다.  하지만 난 보스 한개만 만들것이다.

<img src="https://user-images.githubusercontent.com/37091845/94274988-60e97c80-ff81-11ea-887e-4a1bb9acb10a.png" alt="보스선택" style="zoom:33%;" />

c. 보스와의 싸움 Scene

본격적으로 보스와 싸울수 있는 Scene이다.

공격시 총알이 직진으로 나간다.

c.1 - 게임의 전반적인 모습

<img src="https://user-images.githubusercontent.com/37091845/94274986-6050e600-ff81-11ea-84e8-4a26f56dfb35.png" alt="보스" style="zoom: 33%;" />

c.2 - 플레이어가 보스 공격 시

![image](https://user-images.githubusercontent.com/37091845/95650616-ad0af400-0b1f-11eb-91aa-3c14b2585d8f.png)

c.3 - 보스가 플레이어 공격 시

![image](https://user-images.githubusercontent.com/37091845/95650628-b8f6b600-0b1f-11eb-8a4d-fafec673f1e5.png)

d. 일시중지 Scene

여러가지 Scene으로 이동 가능한 Pause Scene이다.

<img src="https://user-images.githubusercontent.com/37091845/94274994-62b34000-ff81-11ea-9313-51547889f919.png" alt="일시정지" style="zoom:33%;" />

e.

랭킹 Scene

<img src="https://user-images.githubusercontent.com/37091845/94274972-5a5b0500-ff81-11ea-9e20-8e7f1914d06b.png" alt="랭크" style="zoom: 33%;" />

f. Logo Scene

별다를건 없이 kpu 로고를 보여주며

2초뒤 게임 시작 전 Scene으로 넘어간다. 

---

4.

**다른과목에서 배운 기술**

* 이미지 바운딩 충돌처리

---

**기대되는 기술**

* 제가 뭘 배울지 잘 모르겠습니다.
* 맵 툴 관련 대해서는 배울것같은데 기대됩니다.

---

5.

**개발 범위**

| **대상**      | **최소범위**                                                 | **추가**                   |
| ------------- | ------------------------------------------------------------ | -------------------------- |
| 캐릭터        | 좌우이동,점프(최대2단)                                       |                            |
| 보스          | 1종류, 패턴  3개                                             | 2종류, 패턴 8개까지        |
| UI            | 보스의 HP상황                                                | 보스 패턴시, 흔들리는 효과 |
| 사운드        | 캐릭터(이동,점프,공격,사망)  보스(패턴 마다 다른소리, 맞았을 때 소리)  배경음 |                            |
| 에니메이션    | 캐릭터(움직임)  보스(패턴)                                   |                            |
| 충돌체크,처리 | 캐릭터와 보스(사망)  캐릭터와 맵 끝(사망)  캐릭터의 공격과 보스(Hit)  보스의 패턴과 캐릭터(사망) |                            |

---

6.

**개발 일정**

| **주차****(10.12~)** | **개발일정**                                                 |
| -------------------- | ------------------------------------------------------------ |
| 1주차                | 1.리소스 수집  2.플레이어 기본 이동,공격,점프  로직(에니메이션) |
| 2주차                | 보스, 패턴1 로직,에니메이션                                  |
| 3주차                | 보스패턴 2 로직,에니메이션                                   |
| 4주차                | 보스패턴 3 로직,에니메이션                                   |
| 5주차                | 각종 오브젝트들의 충돌처리                                   |
| 6주차                | UI구현,(보스HP,  땅바닥)  메뉴,pause  등 각종 Scene 제작     |
| 7주차                | 각종 sound 삽입, 추가구현,버그수정                           |
| 8주차                | 추가구현, 버그수정                                           |

---

**수업에서 다루면 좋을것 같은 기술들**

* win32 api 에서는 alphablend() 를 통해 이미지를 투명화 시켜줄 수 있었는데

pico2d에서는 어떻게 하는 지 궁금합니다. --- 해결

---

---

---

---

**2차발표**

**현재까지의 개발 진행 상황**

| **대상**      | **최소범위**                                                 | **진행상황** |
| ------------- | ------------------------------------------------------------ | ------------ |
| 캐릭터        | 좌우이동,점프(최대2단)                                       | 100%         |
| 보스          | 1종류, 패턴  3개                                             | 100%         |
| UI            | 보스의 HP상황                                                | 100%         |
| 사운드        | 캐릭터(이동,점프,공격,사망)  보스(패턴 마다 다른소리, 맞았을 때 소리)  배경음 | 0%           |
| 에니메이션    | 캐릭터(움직임)  보스(패턴)                                   | 90%          |
| 충돌체크,처리 | 캐릭터와 보스(사망)  캐릭터와 맵 끝(사망)  캐릭터의 공격과 보스(Hit)  보스의 패턴과 캐릭터(사망) | 100%         |
| 게임 Scene    | Rank,Pause,Start,Select                                      | 0%           |

---

**주차별 깃허브 커밋 횟수 **

![image](https://user-images.githubusercontent.com/37091845/99868805-2f033800-2c09-11eb-9f35-3a537620e487.png)

---

**각 클래스 별 관계도**

![image](https://user-images.githubusercontent.com/37091845/99868811-3f1b1780-2c09-11eb-880b-d0138f436f27.png)

---

클래스가 책임지는 핵심 코드

Player- handle_event 함수로 플레이어 움직임, bullet 생성

​           -die 함수로 blood 생성

Boss - behavior_tree 구조를 이용하여, 자신의 상태에 맞게 함수를 실행 시킴

---

변경점 - 보스 선택 Scene 삭제

- 1차발표때의 추가구현에는 보스의 종류 2가지와, 각각 보스마다 패턴을 8개씩  만드는것이 목적이었지만

  시간 관계상 추가구현에서 보스를 두개를 만들고 둘다 어설프게 만드는것 보단, 보스 하나를 정해서 하나를 제대로

  구현 하는게 맞다고 판단하여, 보스의 종류는 한개로 고정했습니다.

  그러다보니, 보스 종류를 선택하는 보스 선택Scene이 쓸모가 없다고 판단되어 이 Scene에 대한 제작은 삭제하는걸로 정했습니다.

  

