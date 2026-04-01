📚 강의 등록 및 신청 플랫폼

📌 프로젝트 소개

🎯 프로젝트 목표

🧩 주요 기능

🗂️ 프로젝트 구조

``` bash
src (예시 구조)
 ├── pages
 │    ├── lecture
 │    ├── student
 │    ├── lecturer
 │    └── admin
 ├── components
 ├── css
 ├── js
 └── assets
```
⚙️ 기술 스택

React

🔄 Git 협업 규칙

1️⃣ Branch 명명 규칙

브랜치 prefix로 작업 성격을 구분합니다.

유형	설명	예시
| 유형 | 설명 | 예시 |
|------|------|------|
| feature | 새로운 기능 개발 | feature/lecture-create#12 |
| fix | 긴급 버그 수정 | fix/login-error#5 |

2️⃣ Commit Message 규칙
📌 Prefix 종류
| Prefix | 의미 |
|--------|------|
| [FEATURE] | 새로운 기능 추가 |
| [FIX] | 버그 수정 |
| [RENAME] | 파일/폴더명 변경 |
| [STYLE] | 코드 변경 없는 스타일 수정 |

📌 작성 방식
[FEATURE] 강의 등록 기능 구현#12

✔️ 커밋 메시지를 통해 이슈 자동 종료

3️⃣ Issue & PR 규칙

📌 Issue 작성 규칙

제목 (예시)

[Feature] 강의 등록 - 썸네일 업로드 기능 추가

본문

작업 목적
해야 할 일 목록

필수 설정

Assignee: 팀원 2명 지정
Label: feature / fix

📌 PR 규칙

PR 제목

[FEATURE] 강의 등록 기능 구현#12

4️⃣ 협업 프로세스

1. 기능 단위로 Issue 생성
2. 브랜치 생성 후 작업 진행
3. 작업 완료 후 push (⚠️ push 전 팀원에게 공유)
4. Pull Request 생성
5. 팀원 2명 모두 리뷰 진행
6. 리뷰 완료 후 1명이 merge
7. 전체 pull 받아 최신 상태 유지
