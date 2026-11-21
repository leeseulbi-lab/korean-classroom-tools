# 한국어 수업 도구 · Korean Classroom Tools

한국어 선생님이 교실에서 바로 쓸 수 있는 작은 웹 도구 모음입니다. 모두 HTML 파일이라 설치나 가입 없이 브라우저에서 열면 됩니다.

Small, free web tools for Korean language classrooms. Each tool is a plain HTML page: open it in a browser — no sign-up, no installation.

**바로 쓰기 · Open the tools:** https://leeseulbi-lab.github.io/korean-classroom-tools/

| 도구 · Tool | 누가 · For | 하는 일 · What it does |
|---|---|---|
| [짝 정하기 · Pair Maker](pair-maker/) | 교사 · teacher | 출석한 학생만 골라 2·3·4명씩 섞습니다. 이미 짝을 했던 학생끼리는 다시 만나지 않게 피합니다. · Random pairs/groups that avoid repeating past partners. |
| [한글 퀴즈 · Hangul Quiz](hangul-quiz/) | 학생 · students | 모음·자음·받침·소리 변화를 듣고 고르거나 소리 내어 읽습니다. 음원 내장. · Listen-and-choose and read-aloud Hangul practice, audio built in. |
| [활용 연습 · Conjugation Quiz](conjugation-quiz/) | 학생 · students | 문법 형태를 골라 동사·형용사 활용을 연습합니다. · Conjugation practice for the grammar forms you pick. |

---

## 한국어 안내

### 1. 링크로 쓰기 (가장 쉬운 방법)
위 주소를 열고 쓰고 싶은 도구를 누르세요. 교실 화면에 띄우거나 학생에게 링크를 보내면 됩니다.

- **짝 정하기**: "명단 편집"을 누르고 한 줄에 한 명씩 학생 이름을 적은 뒤 "명단 저장"을 누르세요. 결석한 학생은 이름을 눌러 빼고, "새로 섞기"(또는 스페이스바)로 짝을 정합니다. "이 짝으로 확정"을 누르면 기록에 남고, 다음에는 이미 짝을 했던 학생끼리 피합니다.
- 명단과 짝 기록은 **그 컴퓨터의 그 브라우저에만** 저장되고 어디로도 보내지지 않습니다. 다른 컴퓨터에서 쓰려면 "백업 내려받기"로 파일을 받아 그 컴퓨터에서 "백업 불러오기"를 하세요.
- 퀴즈 링크 뒤에 `?lesson=6`을 붙이면 활용 연습이 6과 문법만 골라진 상태로 열립니다.

### 2. 내려받아 인터넷 없이 쓰기
GitHub 저장소 페이지에서 초록색 **Code → Download ZIP**을 누르고, 압축을 푼 뒤 각 폴더의 `index.html`을 더블클릭하세요. 한글 퀴즈는 음원이 파일 안에 들어 있어서 인터넷이 없어도 소리가 납니다. (글꼴은 인터넷이 없으면 기본 글꼴로 보입니다.)

### 3. 우리 반에 맞게 고치기
**활용 연습 문제 바꾸기** — `conjugation-quiz/data.js` 파일 하나만 고치면 됩니다. 한 줄이 문제 하나입니다.

```js
{ lesson: 6, form: "-아/어요", stem: "먹다", type: "", answer: "먹어요", meaning: "eat" },
```

- `lesson`: 과 번호(숫자). 화면에서 과별로 묶입니다.
- `form`: 문법 형태. `-아/어요`, `-았/었어요`, `-(으)세요`, `-(으)ㄹ 거예요`처럼 파일 맨 위에 적힌 형태를 쓰면 그럴듯한 오답이 자동으로 만들어집니다. 다른 형태도 쓸 수 있습니다.
- `type`: 불규칙 등 활용 유형(힌트로 보임). 규칙 활용이면 `""`.
- `answer`: 정답, `meaning`: 영어 뜻.
- 따옴표와 쉼표, 줄 끝의 `},`는 지우지 마세요.

**GitHub에서 고치는 방법** (코딩을 몰라도 됩니다)
1. GitHub 계정으로 로그인하고 이 저장소 오른쪽 위의 **Fork**를 누르면 내 계정에 사본이 생깁니다.
2. 내 사본에서 `conjugation-quiz/data.js`를 열고 연필 아이콘(Edit)을 눌러 고친 뒤 **Commit changes**를 누릅니다.
3. 내 사본의 **Settings → Pages**에서 Branch를 `main`, 폴더를 `/ (root)`로 두고 저장하면 몇 분 뒤 `https://내아이디.github.io/korean-classroom-tools/`에서 내 버전이 열립니다.

GitHub을 쓰지 않는다면 ZIP으로 내려받아 `data.js`를 메모장(Windows)이나 텍스트 편집기(Mac)로 고쳐도 됩니다.

### 의견 보내기
고쳤으면 하는 점이나 새 기능 아이디어는 저장소의 **Issues**에 남겨 주세요.

---

## English

### Use it from the link
Open the address above and pick a tool. Project it in class or send the link to students.

- **Pair Maker**: click "명단 편집" (edit roster), type one name per line and save. Click absent students to remove them, then shuffle with "새로 섞기" or the space bar. "이 짝으로 확정" saves the pairs so future shuffles avoid repeating partners.
- The roster and history are stored **only in this browser on this computer** and are never sent anywhere. Use "백업 내려받기" (download backup) and "백업 불러오기" (load backup) to move them to another computer.
- Add `?lesson=6` to the conjugation quiz link to open it with lesson 6 forms preselected.

### Use it offline
On the repository page, click **Code → Download ZIP**, unzip it and double-click `index.html` in any folder. The Hangul quiz has its audio built in, so it works without internet.

### Adapt it for your class
Edit `conjugation-quiz/data.js` to change the conjugation questions — one line per question. Field notes are at the top of the file. To publish your own version, **Fork** this repository, edit the file on GitHub, then turn on **Settings → Pages** (branch `main`, folder `/ (root)`).

### Feedback
Suggestions and bug reports are welcome in **Issues**.

---

## 만든 사람 · Author
Seul Bi Lee (이슬비) — Korean language teacher and researcher, based in Cambridge, UK.
https://sites.google.com/view/seulbilee

## 라이선스 · License
MIT License. 자유롭게 쓰고, 고치고, 나눌 수 있습니다. 다시 나눌 때는 `LICENSE` 파일을 함께 두세요.
Free to use, adapt and share; keep the `LICENSE` file when you redistribute.
