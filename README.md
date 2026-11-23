# 한국어 수업 도구 · Korean Classroom Tools

한국어 선생님이 교실에서 바로 쓸 수 있는 작은 웹 도구 모음입니다. 모두 HTML 파일이라 설치나 가입 없이 브라우저에서 열면 됩니다.

Small, free web tools for Korean language classrooms. Each tool is a plain HTML page: open it in a browser — no sign-up, no installation.

**바로 쓰기 · Open the tools · Ouvrir les outils :** https://leeseulbi-lab.github.io/korean-classroom-tools/

**언어 · Languages · Langues:** 한국어 · English · Français — 화면 위의 단추로 바꿉니다. · Switch with the buttons at the top of each page. · [Français ci-dessous](#français).

| 도구 · Tool | 누가 · For | 하는 일 · What it does |
|---|---|---|
| [짝 정하기 · Pair Maker](pair-maker/) | 교사 · teacher | 출석한 학생만 골라 2·3·4명씩 섞습니다. 이미 짝을 했던 학생끼리는 다시 만나지 않게 피합니다. · Random pairs/groups that avoid repeating past partners. |
| [한글 퀴즈 · Hangul Quiz](hangul-quiz/) | 학생 · students | 모음·자음·받침·소리 변화를 듣고 고르거나 소리 내어 읽습니다. 음원 내장. · Listen-and-choose and read-aloud Hangul practice, audio built in. |
| [활용 연습 · Conjugation Quiz](conjugation-quiz/) | 학생 · students | 문법 형태를 골라 동사·형용사 활용을 연습합니다. · Conjugation practice for the grammar forms you pick. |

---

## 한국어 안내

### 1. 링크로 쓰기 (가장 쉬운 방법)
위 주소를 열고 쓰고 싶은 도구를 누르세요. 교실 화면에 띄우거나 학생에게 링크를 보내면 됩니다.

- **화면 언어**: 각 도구 위쪽의 단추(한국어 · English · Français)로 바꿉니다. 고른 언어는 그 브라우저에 기억됩니다. 주소 끝에 `?lang=fr`(또는 `en`, `ko`)를 붙인 링크를 보내면 처음부터 그 언어로 열립니다. 프랑스어 화면에서는 한글 퀴즈와 활용 연습의 낱말 뜻도 프랑스어로 보입니다. 활용 연습에서 영어나 프랑스어 화면으로 "학생용 링크 복사"를 하면 그 언어가 링크에 함께 들어갑니다.
- **짝 정하기**: "명단 편집"을 누르고 한 줄에 한 명씩 학생 이름을 적은 뒤 "명단 저장"을 누르세요. 결석한 학생은 이름을 눌러 빼고, "새로 섞기"(또는 스페이스바)로 짝을 정합니다. "이 짝으로 확정"을 누르면 기록에 남고, 다음에는 이미 짝을 했던 학생끼리 피합니다.
- 명단과 짝 기록은 **그 컴퓨터의 그 브라우저에만** 저장되고 어디로도 보내지지 않습니다. 다른 컴퓨터에서 쓰려면 "백업 내려받기"로 파일을 받아 그 컴퓨터에서 "백업 불러오기"를 하세요.

### 2. 내려받아 인터넷 없이 쓰기
GitHub 저장소 페이지에서 초록색 **Code → Download ZIP**을 누르고, 압축을 푼 뒤 각 폴더의 `index.html`을 더블클릭하세요. 한글 퀴즈는 음원이 파일 안에 들어 있어서 인터넷이 없어도 소리가 납니다. (글꼴은 인터넷이 없으면 기본 글꼴로 보입니다.)

### 3. 우리 반에 맞게 고치기
**활용 연습 어휘 바꾸기 (코딩 없이, 화면에서)**
1. 활용 연습을 열고 **어휘 바꾸기**(영어 화면에서는 **Edit words · 어휘 바꾸기**)를 누릅니다.
2. 위의 목록에서 문법 형태(예: `-고 싶어요`)를 고르고, 아래 칸에 한 줄에 한 단어씩 씁니다.
   ```
   먹다, 먹고 싶어요, eat
   듣다, 듣고 싶어요, listen
   ```
   `기본형, 정답, 뜻` 순서입니다. 불규칙 활용이면 네 번째 칸에 유형을 쓰면 힌트로 보입니다(예: `듣다, 들어요, listen, ㄷirregular`).
3. **+ 새 문법 형태**로 `-지만`, `-(으)면` 같은 형태를 더할 수 있고, **이 형태 빼기**로 쓰지 않는 형태를 뺄 수 있습니다.
4. **저장하고 돌아가기**를 누르면 그 브라우저에서 바로 바뀐 어휘로 연습합니다.
5. 학생 기기에서도 같은 어휘로 연습하게 하려면 **학생용 링크 복사**를 눌러 링크를 보내세요. 어휘가 링크 안에 들어 있어서 따로 저장할 곳이 필요 없습니다.
6. 처음 어휘로 돌아가려면 **기본 어휘로 되돌리기**를 누릅니다.

- 객관식 오답은 자동으로 만들어집니다. `-아/어요`, `-았/었어요`, `-(으)세요`, `-(으)ㄹ 거예요` 같은 기본 형태는 그럴듯한 틀린 활용형이 나오고, 새로 더한 형태는 같은 형태의 다른 단어 답이나 같은 단어의 다른 활용형이 오답으로 쓰입니다. 한 형태에 4개 이상 넣으면 보기가 잘 만들어집니다.

**내 저장소의 기본 어휘 자체를 바꾸기**
화면에서 고친 뒤 **data.js 내려받기**를 누르면 지금 어휘가 담긴 `data.js` 파일이 생깁니다. 이 파일로 저장소의 `conjugation-quiz/data.js`를 바꾸면, 링크 없이 열어도 그 어휘가 기본이 됩니다.

**GitHub에서 내 버전 만들기** (코딩을 몰라도 됩니다)
1. GitHub 계정으로 로그인하고 이 저장소 오른쪽 위의 **Fork**를 누르면 내 계정에 사본이 생깁니다.
2. 내 사본에서 `conjugation-quiz` 폴더를 열고 **Add file → Upload files**로 내려받은 `data.js`를 올린 뒤 **Commit changes**를 누릅니다.
3. 내 사본의 **Settings → Pages**에서 Branch를 `main`, 폴더를 `/ (root)`로 두고 저장하면 몇 분 뒤 `https://내아이디.github.io/korean-classroom-tools/`에서 내 버전이 열립니다.

### 의견 보내기
고쳤으면 하는 점이나 새 기능 아이디어는 저장소의 **Issues**에 남겨 주세요.

---

## English

### Use it from the link
Open the address above and pick a tool. Project it in class or send the link to students.

- **Language**: use the buttons at the top of each tool (한국어 · English · Français). Your choice is remembered in that browser. A link ending in `?lang=fr` (or `en`, `ko`) opens directly in that language. With the French screen, word meanings in the Hangul Quiz and the Conjugation Quiz are shown in French too. In the Conjugation Quiz, a student link copied from the English or French screen carries that language with it.
- **Pair Maker**: click **Edit list**, type one name per line and save. Click absent students to remove them, then shuffle with **Shuffle** or the space bar. **Confirm these groups** saves the groups so future shuffles avoid repeating partners.
- The list and history are stored **only in this browser on this computer** and are never sent anywhere. Use **Download backup** and **Load backup** to move them to another computer.

### Use it offline
On the repository page, click **Code → Download ZIP**, unzip it and double-click `index.html` in any folder. The Hangul quiz has its audio built in, so it works without internet.

### Adapt it for your class
In the conjugation quiz, click **Edit words · 어휘 바꾸기**. Pick a grammar form, type one word per line as `dictionary form, answer, meaning` (add a fourth field such as `ㄷirregular` for a hint), add or remove forms, and press **Save**. Saved words stay in that browser. Press **Copy student link** to share the same list with students — the words travel inside the link. **Download data.js** exports your list so you can replace `conjugation-quiz/data.js` in your own fork (**Fork** → upload the file → **Settings → Pages**, branch `main`, folder `/ (root)`).

### Feedback
Suggestions and bug reports are welcome in **Issues**.

---

## Français

De petits outils web gratuits pour la classe de coréen. Chaque outil est une simple page HTML : ouvrez-la dans un navigateur, sans inscription ni installation.

### Utiliser les outils depuis le lien
Ouvrez l’adresse ci-dessus et choisissez un outil. Projetez-le en classe ou envoyez le lien aux élèves.

- **Langue** : utilisez les boutons en haut de chaque outil (한국어 · English · Français). Votre choix est mémorisé dans ce navigateur. Un lien qui se termine par `?lang=fr` s’ouvre directement en français, par exemple `https://leeseulbi-lab.github.io/korean-classroom-tools/hangul-quiz/?lang=fr`.
- **Créer des binômes** (pour l’enseignant) : cliquez sur **Modifier la liste**, écrivez un nom par ligne et enregistrez. Cliquez sur les élèves absents pour les retirer, puis mélangez avec **Mélanger** ou la barre d’espace. **Valider ces groupes** enregistre les groupes : les mélanges suivants évitent de réunir les mêmes élèves.
- La liste et l’historique sont enregistrés **uniquement dans ce navigateur, sur cet ordinateur**, et ne sont envoyés nulle part. **Télécharger une sauvegarde** et **Charger une sauvegarde** permettent de les transférer sur un autre ordinateur.
- **Quiz de hangeul** (pour les élèves) : lire à voix haute, ou écouter et choisir. Le sens des mots s’affiche en français.
- **Quiz de conjugaison** (pour les élèves) : choisissez des formes grammaticales, en choix multiple ou en écrivant la réponse. Le sens des mots par défaut s’affiche en français.

### Utiliser les outils hors ligne
Sur la page du dépôt, cliquez sur **Code → Download ZIP**, décompressez l’archive et double-cliquez sur `index.html` dans le dossier voulu. L’audio du quiz de hangeul est intégré au fichier : il fonctionne sans Internet.

### Adapter à votre classe
Dans le quiz de conjugaison, cliquez sur **Modifier les mots · 어휘 바꾸기**. Choisissez une forme grammaticale et écrivez un mot par ligne : `forme du dictionnaire, réponse, sens` (un quatrième champ, par exemple `ㄷirregular`, sert d’indice). Vous pouvez ajouter ou retirer des formes, puis cliquer sur **Enregistrer et revenir**. Les mots enregistrés restent dans ce navigateur. **Copier le lien élève** partage la même liste avec les élèves : les mots voyagent dans le lien, qui s’ouvre en français. **Télécharger data.js** exporte votre liste pour remplacer `conjugation-quiz/data.js` dans votre propre copie du dépôt (**Fork** → envoyer le fichier → **Settings → Pages**, branche `main`, dossier `/ (root)`).

### Remarques et suggestions
Les suggestions et les signalements d’erreurs sont les bienvenus dans **Issues**.

---

## 만든 사람 · Author · Auteure
Seul Bi Lee (이슬비) — Korean language teacher and researcher, based in Cambridge, UK.
https://sites.google.com/view/seulbilee

## 라이선스 · License · Licence
[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) (저작자표시-비영리-동일조건변경허락)

- 비영리 목적이라면 자유롭게 쓰고, 고치고, 나눌 수 있습니다.
- 쓸 때는 만든 사람(Seul Bi Lee, 이슬비)과 라이선스를 밝히고, 고쳤다면 고쳤다고 적어 주세요.
- 판매하거나 유료 강좌·상품·서비스에 넣는 등 상업적으로 이용할 수 없습니다.
- 고친 것을 나눌 때는 같은 라이선스로 나누어야 합니다.

Free to use, adapt and share for non-commercial purposes. Credit Seul Bi Lee and link to the licence, mark any changes, do not sell the tools or include them in paid courses, products or services, and share adapted versions under the same licence. See `LICENSE`.
Free to use, adapt and share; keep the `LICENSE` file when you redistribute.

Utilisation, adaptation et partage libres à des fins non commerciales. Citez Seul Bi Lee et indiquez la licence, signalez vos modifications, ne vendez pas les outils et ne les intégrez pas à des cours, produits ou services payants, et partagez les versions adaptées sous la même licence. Voir `LICENSE`.
