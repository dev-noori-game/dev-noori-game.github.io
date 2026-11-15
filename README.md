# Son to Son 웹사이트

정적 웹사이트예요. 서버 없이 GitHub Pages에 올리면 바로 돌아가요.

## 올리기 전에 바꿀 것 (전체 찾기/바꾸기)

| 찾을 글자 | 바꿀 내용 | 파일 |
|---|---|---|
| `YOUR_EMAIL@example.com` | 문의용 이메일 | index.html, privacy.html |
| `XXX-XX-XXXXX` | 사업자등록번호 | index.html |
| `pub-0000000000000000` | AdMob 게시자 ID (AdMob → 설정 → 계정 정보) | app-ads.txt |

출시 후에는 index.html의 Google Play 버튼 `href="#"`를 실제 스토어 주소로 바꾸고 `disabled`를 지우세요.

## GitHub Pages에 올리기

1. GitHub에서 새 저장소를 만들고 이름을 **`아이디.github.io`** 로 정해요. (예: `nuri.github.io`)
   - 꼭 이 이름이어야 해요. app-ads.txt는 도메인 맨 앞(루트)에 있어야 AdMob이 인식해요.
2. 이 폴더 안의 파일을 전부 업로드해요 (`Add file → Upload files`, 폴더째 드래그).
3. 저장소 `Settings → Pages`에서 Source가 `Deploy from a branch`, 브랜치 `main` / `(root)`인지 확인.
4. 1~2분 뒤 `https://아이디.github.io` 접속.

## Play Console에 넣을 것

- 개발자 아이콘: `assets/developer-icon-512.png`
- 헤더 이미지: `assets/header-4096x2304.png`
- 웹사이트 주소: `https://아이디.github.io`
- 개인정보처리방침 URL (앱 → 정책 → 앱 콘텐츠): `https://아이디.github.io/privacy.html`

AdMob에 앱을 등록할 때도 스토어 등록정보의 웹사이트가 이 주소여야 app-ads.txt 확인이 돼요.

## 나중에 도메인을 사면

`sontoson.com` 같은 도메인을 사서 `Settings → Pages → Custom domain`에 넣으면 돼요.
