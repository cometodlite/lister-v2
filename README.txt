# Lister v2 (Design-first)
이 템플릿은 GitHub Pages에 올려 **바로 배포**할 수 있는 정적(HTML/CSS/JS) Lister 사이트입니다.
## 디자인 포인트
- 다크/라이트 테마 (우측 상단 🌓)
- 메인 히어로 + Featured 카드
- 아티스트 카드 / 트랙 커버 / 호버 효과
- 하단 고정 플레이어 (시크바/볼륨/이전/다음)
- 검색 (상단 입력창, `/` 키로 바로 포커스)
- 데이터 분리: `artists.json`만 수정하면 목록 갱신
## 내 노래로 교체하기
1) mp3를 `music/` 폴더에 넣기  
2) `artists.json`의 각 트랙 `src`를 파일명으로 바꾸기  
3) 커버 이미지도 바꾸려면 `cover`에 png/jpg/webp 경로를 넣어도 됨
## GitHub Pages 배포
1. 이 폴더를 GitHub 레포에 업로드
2. GitHub → Settings → Pages
3. **Build and deployment**
   - Source: Deploy from a branch
   - Branch: `main` / folder: `/ (root)`
4. 몇 분 뒤 `https://<username>.github.io/<repo>/` 로 접속
## 팁
- 로컬에서 테스트 시 브라우저 정책 때문에 mp3가 막히면 VS Code Live Server를 추천.
- mp3 용량이 크면 Git LFS 또는 외부 스토리지(S3/R2 등)로 옮기고 `src`만 URL로 바꿔도 됨.
## 중요: 스타일이 안 보일 때
- 브라우저 주소가 `...zip.../index.html` 처럼 보이면 **압축을 풀지 않고 열고 있는 상태**라서 CSS/JS/이미지를 못 찾을 수 있어요.
- 해결: ZIP을 '모두 압축 풀기'로 풀고, 폴더 안의 `index.html`을 열거나 Live Server로 실행하세요.
