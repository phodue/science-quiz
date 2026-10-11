# science-quiz

중2 과학 퀴즈 사이트. 구조와 문제 작성 형식은 README.md 참고.

## 브랜치 규칙

- 모든 작업은 `dev` 브랜치에서 한다. 작업 시작 전 `git switch dev && git pull`.
- 수정이 끝나면 `dev`에 커밋하고 push한다.
- 사용자가 배포하라고 하면 `main`에 merge해서 push한다 (`main` = 배포 브랜치).
  ```
  git switch main && git pull && git merge dev && git push && git switch dev
  ```
- `main`에 직접 커밋하지 않는다.

## 참고

- Windows PC에서 작업한다. 줄바꿈은 git이 처리하도록 `core.autocrlf=true`.
- 로컬 확인은 폴더에서 `python -m http.server` 후 http://localhost:8000 (file://로 열면 문제가 안 보임).
