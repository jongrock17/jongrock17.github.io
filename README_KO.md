# 새 홈페이지 적용하기 — 한국어 안내

완성된 홈페이지 주소: **https://jongrock17.github.io** (GitHub Pages 배포 후)

## 1. 이 ZIP을 먼저 압축 해제하세요

ZIP을 GitHub에 그대로 올리면 홈페이지가 바뀌지 않습니다. 압축을 풀어서 내부 파일을 업로드해야 합니다.

## 2. GitHub 저장소의 파일을 교체하세요

1. https://github.com/jongrock17/jongrock17.github.io 열기
2. **Add file → Upload files** 클릭
3. 압축을 푼 `jongrock17.github.io` 폴더 **안의 파일과 폴더**를 업로드합니다. 경로와 폴더 구조를 유지하세요.
   - `_quarto.yml`, `index.qmd`, `research.qmd`, `cv.qmd`, `contact.qmd`, `custom.scss`, `cv.pdf`
   - `images/favicon.svg`
   - `.github/workflows/publish.yml` (기존 배포 설정 유지)
4. 아래의 **Commit changes** 클릭

파일 여러 개를 한 번에 업로드하기 어렵다면 **GitHub Desktop**에서 저장소를 내려받아 파일을 복사한 뒤 `Commit` → `Push` 하는 방법도 있습니다.

## 3. GitHub Pages 공개 설정을 확인하세요

- 설정 페이지: https://github.com/jongrock17/jongrock17.github.io/settings/pages
- **Settings → Pages → Build and deployment → Source: GitHub Actions** 선택
- 이미 `GitHub Actions`로 되어 있으면 변경하지 마세요.
- **Actions** 페이지: https://github.com/jongrock17/jongrock17.github.io/actions
- **Publish website** 작업의 초록 체크 표시 확인
- 작업이 실행되지 않았다면 **Publish website → Run workflow** 실행

> 'Build and deployment'가 보이지 않으면 우선 위의 `settings/pages` 직접 링크로 들어가고, 저장소 설정 페이지를 보고 있는지 확인하세요.

## 4. 실제 홈페이지 방문

https://jongrock17.github.io

## 5. 다음에 바꾸면 좋은 내용

- **홈 소개 문장:** `index.qmd`
- **논문 및 링크:** `research.qmd` (확인된 SSRN 논문 개별 URL 추가 권장)
- **CV 최신본:** `cv.pdf` 교체
- **이메일 및 프로필 주소:** `contact.qmd`, `_quarto.yml`, `index.qmd`
- **전체 디자인:** `custom.scss`

**주의:** 첨부된 CV PDF를 원본 그대로 넣었습니다. CV 내부에 예전 Political Analysis 투고 상태가 표시되어 있으므로, 박사 지원서에 링크를 넣기 전에 최신 CV로 교체하는 것을 권합니다. 사이트의 논문 목록에는 현재 심사 상태를 주장하지 않았습니다.

홈페이지 공개는 무료입니다. 개인 도메인(.com 등)을 연결하려면 별도 도메인 구입이 필요합니다.


## 배포 오류 복구 (2026-11-21 수정)
이 ZIP은 Quarto `title: false` 오류를 수정했습니다. 4개의 `.qmd` 파일 모두 제목 문자열을 사용하고, 실제 화면에서는 `custom.scss`가 자동 생성된 제목 블록을 감춰 디자인을 유지합니다.

GitHub 저장소에서 `Add file` → `Upload files`로 압축을 푼 내부 파일들을 업로드합니다. 기존 파일을 덮어쓰도록 `Commit changes` 합니다. `.github/workflows/publish.yml`가 기존 저장소에 있으면 유지하세요. `Actions` → `Publish website`에서 초록색 체크가 확인되면 https://jongrock17.github.io 로 접속합니다.
