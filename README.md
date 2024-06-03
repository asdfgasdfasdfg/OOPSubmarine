# 시연 영상 링크
https://bit.ly/4e2uJXr 

# 게임 흐름 정리

**(서버, 클라이언트 모두에게 적용 시 강조)**

→ <내용>  :  서버, 또는 클라이언트에게 실제 출력할 내용

*기울어진 글씨체*  :  선택지 조정

## 게임 단계 순서

0 → 1 → 2 → 3 → 4 → 5

---

# 0단계(서버 접속)

## 서버

### 서버 시작

서버 로그: 플레이어 1, 2 모두 접속시까지 대기..(0/2)

서버 로그: 플레이어 1 접속 (1/2)

플레이어 1에게 웰컴 메시지 전송

→ "환영합니다, <nickname>님!"

→ **<nickname> 님이 서버에 접속했습니다.**

→ 대전 상대를 찾는 중..

서버 로그: 플레이어 2 접속시까지 대기..(1/2)

서버 로그: 플레이어 2 접속 (2/2)

플레이어 2에게 웰컴 메시지 전송

→ "환영합니다, <nickname>님!"

→ **<nickname> 님이 서버에 접속했습니다.**

모든 플레이어에게 게임 시작 메시지 전송

→ "게임이 시작됩니다."

---

## 클라이언트

### 클라이언트 시작

접속할 IP, 닉네임 순서대로 입력

→ "접속할 서버의 주소를 입력해주세요"

→ "올바른 IP 주소 형식을 입력해주세요 (예: 192.168.1.1)"

→ "사용하실 닉네임을 입력해주세요"

→ "올바른 닉네임 형식을 입력해주세요 (예: David)"

서버 접속 성공 시 welcome message 수신

→ **<nickname> 님이 서버에 접속했습니다.**

→ "게임이 시작됩니다."

서버 접속 실패 시 오류 메시지 전송

→ "서버에 접속할 수 없습니다. 다시 시도해주세요."

---

# 1단계(난이도 선택)

## 서버

### 플레이어 1인 경우

메시지 전송

→ "당신은 방장입니다. 잠시 후 게임 난이도를 선택해주세요"

플레이어 1에게 난이도 선택 창 띄움

→ 순서대로 Beginner, Intermediate, Expert 중 3개의 버튼 중 1개를 20초 안에 선택

→ “**선택하지 않을 경우 기본 난이도 Beginner로 설정됩니다” 를 선택 버튼 밑에 띄움**

### 플레이어 2인 경우

메시지 전송

→ "방장이 게임 룰을 설정하고 있습니다.."

*난이도 선택 완료 시 모든 플레이어에게 메시지 전송*

→ **"난이도 선택이 완료되었습니다. 선택된 난이도는 <난이도>입니다."**

플레이어 2에게도 창을 동시에 띄워서 무슨 난이도가 선택되었는지 확인시키기.

---

## 클라이언트

### 플레이어 1인 경우

난이도 선택 창 표시

→ "당신은 방장입니다. 잠시 후 게임 난이도를 선택해주세요"

→ 난이도 버튼 (Beginner, Intermediate, Expert)

→ *선택하지 않을 경우 기본 난이도 Beginner 선택한 것으로 간주*

### 플레이어 2인 경우

난이도 선택 대기 메시지 표시

→ "방장이 게임 룰을 설정하고 있습니다.."

난이도 선택 완료 시 메시지 표시

→ **"난이도 선택이 완료되었습니다. 선택된 난이도는 <난이도>입니다."**

---

# 2단계 (능력 설정)

## 서버

### 플레이어 1, 2 모두에게 메시지 전송

→ "능력을 선택하십시오!"

플레이어에게 능력 선택 창 띄움

→ 가능한 능력 이미지와 설명을 표시 (각 플레이어에게 무작위로 배정된 능력 풀 중에서 중복되지 않게 선택)

→ *능력을 선택할 수 있는 남은 시간 표시*

플레이어가 능력을 선택하면 다른 플레이어가 선택 중임을 표시

### 모든 플레이어가 선택 완료 시 메시지 전송

→ "능력 선택이 완료되었습니다."

---

## 클라이언트

능력 선택 창 표시

→ "능력을 선택하십시오!"

→ 능력 이미지와 설명이 나타나고, 선택 시 해당 능력 확정

→ *능력을 선택할 수 있는 남은 시간 표시*

능력 선택 완료 시 메시지 표시

→ "능력 선택이 완료되었습니다."

---

# 3단계 (지뢰 매설)

## 서버

### 모든 플레이어에게 메시지 전송

→ "지뢰를 매설하십시오!"

플레이어가 지뢰를 매설할 수 있는 창 띄움

→ 각 플레이어는 자신의 맵에 5개의 지뢰를 매설

→ *지뢰를 매설할 수 있는 남은 시간 표시*

플레이어가 지뢰 매설 완료 시 다른 플레이어가 매설 중임을 표시

### 모든 플레이어가 매설 완료 시 메시지 전송

→ "모든 지뢰가 매설되었습니다. 게임을 시작합니다."

---

## 클라이언트

지뢰 매설 창 표시

→ "지뢰를 매설하십시오! (각 플레이어는 5개의 지뢰를 매설해야 합니다)"

→ *지뢰를 매설할 수 있는 남은 시간 표시*

지뢰 매설 완료 시 메시지 표시

→ "다른 플레이어가 지뢰를 매설 중입니다.."

---

# 4단계 (게임 진행)

## 서버

### 플레이어 1, 2 모두에게 메시지 전송

→ "게임이 시작됩니다. 첫 번째 차례는 <플레이어 1>입니다."

현재 차례의 플레이어에게 메시지 전송

→ "당신의 차례입니다! 행동을 선택하십시오."

상대방 차례의 플레이어에게 메시지 전송

→ "상대의 차례입니다. 잠시 기다려주세요."

### 각 플레이어의 행동에 따라 게임 진행

→ 선택된 위치에 따른 결과 전송 (지뢰 발견, 보물 발견 등)

→ *행동 요약 표시*

플레이어 차례가 끝나면 상대방에게 차례 알림 메시지 전송

---

## 클라이언트

게임 진행 창 표시

→ "게임이 시작됩니다. 첫 번째 차례는 <플레이어 1>입니다."

차례인 경우 메시지 표시

→ "당신의 차례입니다! 행동을 선택하십시오."

차례가 아닌 경우 메시지 표시

→ "상대의 차례입니다. 잠시 기다려주세요."

행동 선택 후 결과 표시

→ 선택된 위치에 따른 결과 (지뢰 발견, 보물 발견 등)

→ *행동 요약 표시*

---

# 5단계 (결과 출력 및 선택)

## 서버

### 게임 종료 시 모든 플레이어에게 결과 메시지 전송

→ "게임 종료! 결과를 확인하십시오."

→ 결과창 표시 (예: <플레이어> 승리! 몇 점 차이로, 지뢰 몇 개 밟았고, 승리수, 패배수 등)

→ *각 플레이어의 상세한 행동 로그 추가*

승리 플레이어에게 재시작, 종료 선택 메시지 전송

→ "재시작 또는 종료를 선택하십시오."

패배 플레이어에게 복수, 종료 선택 메시지 전송

→ "복수 또는 종료를 선택하십시오."

모든 플레이어가 재시작 선택 시 게임 재시작

→ 1단계로 돌아감

모든 플레이어가 종료 선택 시 게임 종료

---

## 클라이언트

게임 종료 후 결과 표시

→ "게임 종료! 결과를 확인하십시오."

→ 결과창 (예: <플레이어> 승리! 보물 개수, 지뢰 몇 개 밟았고, 승리 수, 패배 수)

→ *각 플레이어의 상세한 행동 로그 추가*

승리 시 재시작 또는 종료 선택

→ "재시작 또는 종료를 선택하십시오."

패배 시 복수 또는 종료 선택

→ "복수 또는 종료를 선택하십시오."

재시작 선택 시 게임 재시작

→ 1단계로 돌아감

종료 선택 시 게임 종료

→ 게임 종료 메시지 표시

---
