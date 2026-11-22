# 올케어 입시 시뮬

**jungsi.allcare-edu.com 배포 파일. 게시는 GitHub Pages의 `gh-pages` 브랜치다.** (빌드 없음)

> ⚠ 예전 README에 "Netlify가 main 브랜치를 게시한다"고 적혀 있었으나 사실이 아니다(2026-11 확인).
> - 사이트에 반영되는 것은 **`gh-pages` 브랜치뿐**이다. `main`에 올려도 주소는 바뀌지 않는다.
> - **이 저장소 파일(또는 G드라이브 `배포용_2028` 폴더)을 Netlify에 올리지 않는다.**
>   학원 Netlify에는 `info.allcare-edu.com`(예비고1 입시설명회, 카페·QR에 나간 주소)이 붙어 있어,
>   올리면 설명회 화면이 시뮬레이터로 덮어써진다. 2026-11-22에 실제로 이 사고가 났다.

## 경로 (gh-pages 기준, 지우지 않는다)

| 경로 | 내용 |
|---|---|
| `/` | 고1·고2 통합판(한눈에·수시·정시) |
| `/go3/` | 고3 정시 |
| `/15/` | 고3 정시 상위 15개 대학 환산판 |
| `/ipsi/`, `/ipsi/guide/` | 입시 시뮬(고1·고2) · 사용설명서 |
| `/susi/` | `/#susi`로 넘김 |
| `/suneung-eng/` | 2027 수능 영어 FINAL 체크 |
| `/m/{코드}/` | 학생별 면접 플랜 웹앱 짧은 주소 |

`CNAME`(jungsi.allcare-edu.com)과 `.nojekyll`도 gh-pages에 있다. 지우면 주소가 끊긴다.

## 올리는 법

- 원장: GitHub에서 브랜치를 **`gh-pages`**로 바꾼 뒤 Add file → Upload files → Commit.
- Claude: `gh-pages`를 worktree로 열어 바꿀 경로의 파일만 넣고 커밋 → `git push origin gh-pages`.
- 올린 뒤 1~2분 뒤 jungsi 주소를 열어 확인하고, **info.allcare-edu.com도 열어 설명회(「2027 예비고1 입시설명회」)가 그대로인지 확인**한다.

`_redirects`는 GitHub Pages가 읽지 않는다. 주소를 넘길 때는 `경로/index.html` 이동 페이지를 만든다.
