## 📚 강의 등록 및 신청 플랫폼


## 🎯 프로젝트 목표


## 🧩 주요 기능


## 🗂️ 프로젝트 구조

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


## ⚙️ 기술 스택

![REACT](https://img.shields.io/badge/react-61DAFB?style=flat-square&logo=react&logoColor=white)


## 1️⃣ Branch 명명 규칙

브랜치 prefix로 작업 성격을 구분합니다.

유형	설명	예시
| 유형 | 설명 | 예시 |
|------|------|------|
| feature | 새로운 기능 개발 | feature/lecture-create#12 |
| fix | 긴급 버그 수정 | fix/login-error#5 |


## 2️⃣ Commit Message 규칙

📌 Prefix 종류
| Prefix | 의미 |
|--------|------|
| [FEATURE] | 새로운 기능 추가 |
| [FIX] | 버그 수정 |
| [RENAME] | 파일/폴더명 변경 |
| [STYLE] | 코드 변경 없는 스타일 수정 |


📌 작성 방식 : [FEATURE] 강의 등록 기능 구현#12

✔️ 커밋 메시지를 통해 이슈 자동 종료


## 3️⃣ Issue & PR 규칙

📌 Issue 작성 규칙

제목 : [FEATURE] 강의 등록 기능 구현#12

Label: feature / fix

📌 PR 규칙

제목 : [FEATURE] 강의 등록 기능 구현#12

Assignee: 팀원 2명 지정

Label: feature / fix


## 4️⃣ 협업 프로세스

1. 기능 단위로 Issue 생성
2. 브랜치 생성 후 작업 진행
3. 작업 완료 후 push (⚠️ push 전 팀원에게 공유)
4. Pull Request 생성
5. 팀원 2명 모두 리뷰 진행
6. 리뷰 완료 후 1명이 merge
7. 전체 pull 받아 최신 상태 유지

## 컴포넌트 구조 설계

``` bash
([App]
	├──MainLayOut
			├── Header
			├── Nav
			├── Side
			├── Outlet
						├── HomePage
									├── SearchBar (검색창)
									├── CategorySelector (카테고리바)
									├── LectureItem (mode=box)
						├── LectureDetailPage (mode=box | mode=list) (강의상세조회)
									├── LectureItem (mode=detail | mode=myDetail)
						├── MyLecturePage (내 강의)
									├── LectureItem (mode=list)
						├── ProjectManagePage (프로젝트관리)
									├── LectureItem (mode=proList)
						├── InterviewManagePage (모의면접관리)
									├── LectureItem (mode=invList)
						├── ProjectTotalPage (프로젝트 전체 조회)
									├── ProjectItem (mode=student | mode=teacher)
						├── ProjectDetailPage (프로젝트 상세 조회)
									├── ProjectItem (mode=detail | mode=myDetail)
						├── InterviewDetailPage (모의면접 상세 조회)
									├── interviewItem (mode=detail)
						
						├── CartPage (수강생-장바구니)
									├── CartItem
						├── ProjectPage (수강생-프로젝트 제출)
									├── ProjectTemplate
									├── Project
						├── ProjectWritePage (수강생-프로젝트 작성)
									├── ProjectForm
						├── InterviewNoticePage (수강생-모의면접안내)
						├── InterVIewPracticePage (수강생-모의면접진행)
									├── InterviewQuestion
											
						├── LectureRegistPage (강사-강의등록)
									├── LectureForm (mode=regist)
						├── LectureEditPage (강의수정)
									├── LectureForm (mode=edit)
						├── ProjectRegistPage (강사-프로젝트등록)
									├── ProjectTemplateForm (mode=regist)
						├── ProjectEditPage (강사-프로젝트수정)
									├── ProjectTemplateForm (mode=edit)
						├── InterviewRegistPage (강사-모의면접등록)
									├── InterviewForm (mode=regist)
						├── InterviewEditPage (강사-모의면접수정)
									├── InterviewForm (mode=edit)
						├── InterviewTotalPage (강사-모의면접 전체 조회)
									├── interviewItem (mode=list)
						
						
						├── ManagerDashboardPage (관리자-대시보드)
									├── userItem(mode=latest)
						├── UserManagePage (관리자-회원관리)
									├── SearchBar (검색창)
									├── userItem(mode=list)
						├── LectureManagePage (관리자-강의관리)
									├── SearchBar (검색창)
									├──LectureItem (mode=list)
						├── DataManagePage (관리자-자료관리)
									├── SearchBar (검색창)
									├── PotfolioItem
						
						├── LoginPage
						
						├── SignPage
									├── SignForm
									
			├── Footer
```
