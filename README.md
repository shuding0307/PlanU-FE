<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
<div align="center">

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

<a href="#english"><img src="https://img.shields.io/badge/English-0A66C2?style=for-the-badge" alt="English"></a>
<a href="#korean"><img src="https://img.shields.io/badge/한국어-E03C31?style=for-the-badge" alt="한국어"></a>

</div>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Plan-You/PlanU-FE">
    <img src="src/assets/logo/planU.png" alt="PlanU logo" height="80">
  </a>

  <h3 align="center">PlanU — Frontend</h3>

  <p align="center">
    A scheduling service that makes it easy to plan meetups and coordinate group schedules with friends, clubs and project teams.
    <br />
    친구와의 약속, 단체 모임, 팀플 일정을 쉽게 조율할 수 있는 일정 공유 서비스
    <br />
    <a href="#about-the-project"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/Plan-You/PlanU-FE">Original Team Repo</a>
    ·
    <a href="#my-contributions">My Contributions</a>
    ·
    <a href="#real-time-chat">Real-time Chat</a>
    <br />
    <a href="https://docs.google.com/spreadsheets/d/18EIL5t-26ZWqH48sPKfZn6WFGB1dvD_Fgw3HQe5gk_M/edit?usp=sharing">Requirements</a>
    ·
    <a href="https://www.figma.com/board/R6UVJ9RXqBV2Ak84GVTpBS/planU-Flowchart?node-id=0-1">Flowchart</a>
    ·
    <a href="https://app.notion.com/p/59f004a32f45484fbc1791adab7f04c6?v=af7bef0f65034923990653878d82c880">API Spec</a>
  </p>
</div>

---

<a id="english"></a>

# 🇺🇸 English

> This repository is a fork of the team project [Plan-You/PlanU-FE](https://github.com/Plan-You/PlanU-FE).
> I worked on it as the **team lead and a frontend developer** from November 2024 to June 2025 ([My Contributions](#my-contributions)).

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#key-features">Key Features</a></li>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#project-documents">Project Documents</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#project-structure">Project Structure</a></li>
    <li><a href="#my-contributions">My Contributions</a></li>
    <li><a href="#real-time-chat">Real-time Chat</a></li>
    <li><a href="#team-conventions">Team Conventions</a></li>
    <li><a href="#contributors">Contributors</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

<!-- Add a screenshot here: ![PlanU Screenshot](docs/screenshot.png) -->

Planning a meetup with several people usually means a long group chat full of "when are you free?" messages. **PlanU** puts schedules, availability and chat in one place.

* Users manage their own calendar and mark when they are available.
* Groups combine their members' availability to find a time that works for everyone, then create a group event.
* Each group has a real-time chat room, and each event has its own comments and location.

### Key Features

| Feature | Description |
| --- | --- |
| Sign up & login | Email verification, find ID / password |
| My calendar | Create, edit and delete personal events; mark available times |
| Groups | Create groups, invite members, manage members |
| Group calendar | See members' combined availability and create group events |
| Event details | Location on a map, participants, comments |
| Real-time group chat | WebSocket (STOMP/SockJS), read receipts, live unread counts, image messages, chat search |
| Friends & notifications | Friend requests and management, notification list |
| My page | Profile edit |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* [![React][React.js]][React-url]
* [![TypeScript][TypeScript]][TypeScript-url]
* [![Vite][Vite]][Vite-url]
* [![TanStack Query][TanStackQuery]][TanStackQuery-url]
* [![Zustand][Zustand]][Zustand-url]
* [![React Router][ReactRouter]][ReactRouter-url]
* [![React Hook Form][ReactHookForm]][ReactHookForm-url]
* [![Storybook][Storybook]][Storybook-url]

Also: STOMP.js, SockJS, styled-components, SCSS Modules, date-fns, Google Maps, react-hot-toast, ESLint (Airbnb), Prettier.
Deployed with Vercel. Collaboration: GitHub Issues & Projects, Figma, Swagger, Notion.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Project Documents

As team lead, I wrote the requirements and the feature flow before development started, and the team built from them.

| Document | What it covers |
| --- | --- |
| [Requirements](https://docs.google.com/spreadsheets/d/18EIL5t-26ZWqH48sPKfZn6WFGB1dvD_Fgw3HQe5gk_M/edit?usp=sharing) | Feature requirements by screen (Google Sheets) |
| [Flowchart](https://www.figma.com/board/R6UVJ9RXqBV2Ak84GVTpBS/planU-Flowchart?node-id=0-1) | User flows and feature specification (FigJam) |
| [API Spec](https://app.notion.com/p/59f004a32f45484fbc1791adab7f04c6?v=af7bef0f65034923990653878d82c880) | REST and chat API endpoints shared with the backend (Notion) |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

* Node.js 18+
* The PlanU backend API

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/shuding0307/PlanU-FE.git
   cd PlanU-FE
   git checkout dev
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Set up HTTPS for the local server. Check that `init-https.sh` and two `.pem` files were created in the project root.
   ```sh
   npm run init-https
   ```
4. Run the dev server (served over HTTPS)
   ```sh
   npm run dev
   ```
5. (Optional) Run Storybook on http://localhost:6006
   ```sh
   npm run storybook
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- PROJECT STRUCTURE -->
## Project Structure

```
src
├── api           # API functions by domain (calendar, chat, friend, group, location, notification, schedule, user)
├── components    # shared components (buttons, calendar, headers, input boxes, map, modals, nav-bar ...)
├── pages         # one folder per page
│   └── <Page>/{page,components}   # page entry + page-only components
├── routes        # React Router routes
├── store         # Zustand stores
├── types         # API types split by the API spec's categories
└── constants · layout · styles · utils · assets
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MY CONTRIBUTIONS -->
## My Contributions

I joined as a frontend developer and took the **team lead** role for the first time. I made 212 commits between November 2024 and June 2025.

**Team lead**
* Planned the product and defined its features and screens.
* Split the work by area and coordinated the schedule with the backend developers and the designer.

**Real-time group chat**
* Connected the chat to the server over WebSocket with STOMP and SockJS.
* Built read receipts, unread counts that update live when another member enters the room, and sender display.
* Added image messages (with photo removal before sending), chat room search and message copy.
* Grouped messages by date, showed the date on messages older than a day, and limited the last message in the chat list to two lines.
* Connected group details and entry messages to the chat room.

**Schedules & comments**
* Built the create and edit schedule pages, including the date/time picker, an all-day option that hides the time picker, and a location box with a map.
* Integrated the APIs for viewing, editing and deleting personal and group events.
* Built event comments: a floating comment button, a comment modal, and fetch / create / delete APIs.

**Sign up, login & shared UI**
* Built the start, sign-up, login and find ID / password pages; integrated the email verification API and refactored the forms with React Hook Form.
* Made shared button and input components and documented the inputs in Storybook.
* Built the group calendar page and the shared Tab, Card and event card components, and the My Page components.

**QA**
* Fixed issues found in two rounds of QA, including the chat input layout, long messages and event detail colors.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- REAL-TIME CHAT -->
## Real-time Chat

The group chat was the most complex feature I built. It had to keep many pieces of state in sync while messages arrive over a live connection.

| Problem | What I did |
| --- | --- |
| Connecting to the chat server | Connected through STOMP over SockJS, subscribing to each group's chat room |
| Showing who has read a message | Calculated the unread count for each message and updated it live when another member entered the room |
| Long chat history | Grouped messages by date and showed the date for messages more than a day old |
| Sending images | Added image messages with a preview and the option to remove a photo before sending |
| Finding a chat room | Added search on the chat list; long last messages are cut to two lines |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- TEAM CONVENTIONS -->
## Team Conventions

* **Workflow:** every task goes on the kanban board and is linked to an issue; each issue gets its own branch (`feat/#32`, `style/#30`).
* **Branches:** `main` for deployment, `dev` for development; direct pushes to both are blocked, and changes go through pull requests.
* **Commits:** prefixes such as `Feat`, `Fix`, `Style`, `Refactor`, `Docs`, `Conf`, `Chore`.
* **Types:** API types live in `types/`, split by the API spec's categories, and named `I` + method + API name + `Request`/`Response` + `BodyType`.
* **Code style:** camelCase for functions, variables and hooks; PascalCase for components and types; `is` / `has` / `can` prefixes for booleans; `handle` prefix for event handlers; absolute imports.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTORS -->
## Contributors

PlanU was built by the PlanU team. Thanks to everyone who worked on it.

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/shuding0307">
        <img src="https://github.com/shuding0307.png" width="100" alt="shuding0307" /><br />
        <sub><b>shuding0307</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/jjaeho0415">
        <img src="https://github.com/jjaeho0415.png" width="100" alt="jjaeho0415" /><br />
        <sub><b>jjaeho0415</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/d0-neii">
        <img src="https://github.com/d0-neii.png" width="100" alt="d0-neii" /><br />
        <sub><b>d0-neii</b></sub>
      </a>
    </td>
  </tr>
</table>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Suhyeon Lee · [@shuding0307](https://github.com/shuding0307)

Project Link: [https://github.com/shuding0307/PlanU-FE](https://github.com/shuding0307/PlanU-FE/tree/dev)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Plan-You/PlanU-FE](https://github.com/Plan-You/PlanU-FE), the original team repository
* [Best-README-Template](https://github.com/othneildrew/Best-README-Template)
* [Shields.io](https://shields.io)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<a id="korean"></a>

# 🇰🇷 한국어

> 이 레포지토리는 팀 프로젝트 [Plan-You/PlanU-FE](https://github.com/Plan-You/PlanU-FE)를 포크한 것입니다.
> 2024년 11월부터 2025년 6월까지 **팀장이자 프론트엔드 개발자**로 참여했습니다([담당 업무](#ko-contributions)).

<!-- TABLE OF CONTENTS -->
<details>
  <summary>목차</summary>
  <ol>
    <li>
      <a href="#ko-about">프로젝트 소개</a>
      <ul>
        <li><a href="#ko-features">주요 기능</a></li>
        <li><a href="#ko-built-with">기술 스택</a></li>
        <li><a href="#ko-documents">프로젝트 문서</a></li>
      </ul>
    </li>
    <li>
      <a href="#ko-getting-started">시작하기</a>
      <ul>
        <li><a href="#ko-prerequisites">사전 준비</a></li>
        <li><a href="#ko-installation">설치 및 실행</a></li>
      </ul>
    </li>
    <li><a href="#ko-structure">프로젝트 구조</a></li>
    <li><a href="#ko-contributions">담당 업무</a></li>
    <li><a href="#ko-chat">실시간 채팅</a></li>
    <li><a href="#ko-conventions">팀 컨벤션</a></li>
    <li><a href="#ko-contributors">기여자</a></li>
    <li><a href="#ko-contact">연락처</a></li>
    <li><a href="#ko-acknowledgments">참고 및 감사</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
<a id="ko-about"></a>

## 프로젝트 소개

<!-- 스크린샷 추가: ![PlanU 스크린샷](docs/screenshot.png) -->

여러 명이 약속을 잡으려면 "언제 시간 돼?"로 시작하는 긴 단톡방이 생기기 마련입니다. **PlanU**는 일정, 가능한 시간, 채팅을 한곳에 모았습니다.

* 유저는 개인 캘린더에서 일정을 관리하고 가능한 시간을 표시합니다.
* 그룹은 멤버들의 가능한 시간을 모아 모두가 되는 시간을 찾고, 그룹 일정을 만듭니다.
* 그룹마다 실시간 채팅방이 있고, 일정마다 댓글과 장소가 있습니다.

<a id="ko-features"></a>

### 주요 기능

| 기능 | 설명 |
| --- | --- |
| 회원가입 · 로그인 | 이메일 인증, 아이디 / 비밀번호 찾기 |
| 나의 캘린더 | 개인 일정 생성 · 수정 · 삭제, 가능한 시간 표시 |
| 그룹 | 그룹 생성, 멤버 초대, 멤버 관리 |
| 그룹 캘린더 | 멤버들의 가능한 시간 확인, 그룹 일정 생성 |
| 일정 상세 | 지도로 보는 장소, 참석자, 댓글 |
| 실시간 그룹 채팅 | WebSocket(STOMP/SockJS), 읽음 처리, 실시간 안 읽은 사람 수, 이미지 전송, 채팅방 검색 |
| 친구 · 알림 | 친구 요청 및 관리, 알림 목록 |
| 마이페이지 | 프로필 수정 |

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<a id="ko-built-with"></a>

### 기술 스택

* [![React][React.js]][React-url]
* [![TypeScript][TypeScript]][TypeScript-url]
* [![Vite][Vite]][Vite-url]
* [![TanStack Query][TanStackQuery]][TanStackQuery-url]
* [![Zustand][Zustand]][Zustand-url]
* [![React Router][ReactRouter]][ReactRouter-url]
* [![React Hook Form][ReactHookForm]][ReactHookForm-url]
* [![Storybook][Storybook]][Storybook-url]

그 외: STOMP.js, SockJS, styled-components, SCSS Modules, date-fns, Google Maps, react-hot-toast, ESLint(Airbnb), Prettier.
배포: Vercel. 협업: GitHub Issues · Projects, Figma, Swagger, Notion.

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<a id="ko-documents"></a>

### 프로젝트 문서

팀장으로서 개발 전에 요구사항과 기능 흐름을 정리했고, 팀은 이 문서를 기준으로 개발했습니다.

| 문서 | 내용 |
| --- | --- |
| [요구사항 명세서](https://docs.google.com/spreadsheets/d/18EIL5t-26ZWqH48sPKfZn6WFGB1dvD_Fgw3HQe5gk_M/edit?usp=sharing) | 화면별 기능 요구사항 (Google Sheets) |
| [기능 명세 · 플로우차트](https://www.figma.com/board/R6UVJ9RXqBV2Ak84GVTpBS/planU-Flowchart?node-id=0-1) | 사용자 흐름과 기능 명세 (FigJam) |
| [API 명세서](https://app.notion.com/p/59f004a32f45484fbc1791adab7f04c6?v=af7bef0f65034923990653878d82c880) | 백엔드와 공유한 REST · 채팅 API 명세 (Notion) |

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<!-- GETTING STARTED -->
<a id="ko-getting-started"></a>

## 시작하기

<a id="ko-prerequisites"></a>

### 사전 준비

* Node.js 18 이상
* PlanU 백엔드 API

<a id="ko-installation"></a>

### 설치 및 실행

1. 레포 클론
   ```sh
   git clone https://github.com/shuding0307/PlanU-FE.git
   cd PlanU-FE
   git checkout dev
   ```
2. 패키지 설치
   ```sh
   npm install
   ```
3. 로컬 서버 HTTPS 설정. 루트 경로에 `init-https.sh`와 `.pem` 파일 2개가 생성됐는지 확인합니다.
   ```sh
   npm run init-https
   ```
4. 개발 서버 실행 (HTTPS 적용)
   ```sh
   npm run dev
   ```
5. (선택) Storybook 실행 후 http://localhost:6006 접속
   ```sh
   npm run storybook
   ```

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<!-- PROJECT STRUCTURE -->
<a id="ko-structure"></a>

## 프로젝트 구조

```
src
├── api           # 도메인별 API 함수 (calendar, chat, friend, group, location, notification, schedule, user)
├── components    # 공통 컴포넌트 (buttons, calendar, headers, inputBoxes, map, modals, nav-bar ...)
├── pages         # 페이지별 폴더
│   └── <Page>/{page,components}   # 페이지 진입점 + 페이지 전용 컴포넌트
├── routes        # React Router 라우트
├── store         # Zustand 스토어
├── types         # API 명세서 카테고리별로 분리한 타입
└── constants · layout · styles · utils · assets
```

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<!-- MY CONTRIBUTIONS -->
<a id="ko-contributions"></a>

## 담당 업무

프론트엔드 개발자로 참여하면서 처음으로 **팀장**을 맡았고, 2024년 11월부터 2025년 6월까지 212개의 커밋을 작성했습니다.

**팀장**
* 서비스를 기획하고 기능과 화면을 정의했습니다.
* 영역별로 업무를 나누고 백엔드 개발자, 디자이너와 일정을 조율했습니다.

**실시간 그룹 채팅**
* STOMP와 SockJS로 WebSocket 채팅 서버와 연동했습니다.
* 읽음 처리, 다른 멤버가 채팅방에 들어오면 실시간으로 갱신되는 안 읽은 사람 수, 보낸 사람 표시를 구현했습니다.
* 이미지 전송(전송 전 사진 삭제 포함), 채팅방 검색, 메시지 복사 기능을 추가했습니다.
* 메시지를 날짜별로 묶고, 하루가 지난 메시지에는 날짜를 표시했으며, 채팅 목록의 마지막 메시지는 두 줄까지만 보이도록 했습니다.
* 채팅방에 그룹 상세 정보와 입장 메시지를 연동했습니다.

**일정 · 댓글**
* 날짜·시간 선택, 종일 선택 시 시간 선택 숨기기, 지도가 포함된 장소 입력을 갖춘 일정 생성·수정 페이지를 구현했습니다.
* 개인 일정과 그룹 일정의 조회 · 수정 · 삭제 API를 연동했습니다.
* 플로팅 댓글 버튼, 댓글 모달, 댓글 조회 · 생성 · 삭제 API로 일정 댓글 기능을 구현했습니다.

**회원가입 · 로그인 · 공통 UI**
* 시작, 회원가입, 로그인, 아이디·비밀번호 찾기 페이지를 구현하고, 이메일 인증 API를 연동했으며 폼을 React Hook Form으로 리팩토링했습니다.
* 공통 버튼·입력 컴포넌트를 만들고 입력 컴포넌트를 Storybook으로 문서화했습니다.
* 그룹 캘린더 페이지와 공통 Tab, Card, 일정 카드 컴포넌트, 마이페이지 컴포넌트를 구현했습니다.

**QA**
* 두 차례 QA에서 나온 채팅 입력창 레이아웃, 긴 메시지, 일정 상세 색상 등의 문제를 수정했습니다.

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<!-- REAL-TIME CHAT -->
<a id="ko-chat"></a>

## 실시간 채팅

그룹 채팅은 제가 맡은 기능 중 가장 복잡했습니다. 실시간으로 들어오는 메시지에 맞춰 여러 상태를 함께 맞춰야 했습니다.

| 문제 | 해결 |
| --- | --- |
| 채팅 서버 연결 | SockJS 위에서 STOMP로 연결하고, 그룹별 채팅방을 구독 |
| 누가 메시지를 읽었는지 표시 | 메시지별 안 읽은 사람 수를 계산하고, 다른 멤버가 입장하면 실시간으로 갱신 |
| 길어지는 채팅 기록 | 메시지를 날짜별로 묶고, 하루가 지난 메시지에 날짜 표시 |
| 이미지 전송 | 미리보기와 전송 전 사진 삭제가 가능한 이미지 메시지 |
| 채팅방 찾기 | 채팅 목록 검색, 긴 마지막 메시지는 두 줄까지만 표시 |

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<!-- TEAM CONVENTIONS -->
<a id="ko-conventions"></a>

## 팀 컨벤션

* **작업 방식:** 모든 작업은 칸반 보드에 올리고 이슈로 연결한 뒤, 이슈마다 브랜치를 새로 만들어 작업합니다(`feat/#32`, `style/#30`).
* **브랜치:** `main`은 배포, `dev`는 개발 브랜치이며, 두 브랜치 모두 직접 push를 막고 PR로만 반영합니다.
* **커밋:** `Feat`, `Fix`, `Style`, `Refactor`, `Docs`, `Conf`, `Chore` 등의 접두사를 사용합니다.
* **타입:** API 타입은 `types/`에 API 명세서 카테고리별로 나누고, `I` + 메소드 + API 종류 + `Request`/`Response` + `BodyType` 형식으로 이름 짓습니다.
* **코드 스타일:** 함수·변수·훅은 camelCase, 컴포넌트·타입은 PascalCase, Boolean은 `is` / `has` / `can` 접두사, 이벤트 핸들러는 `handle` 접두사, import는 절대경로를 사용합니다.

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<!-- CONTRIBUTORS -->
<a id="ko-contributors"></a>

## 기여자

PlanU는 PlanU 팀이 함께 만들었습니다. 함께한 모든 팀원에게 감사드립니다.

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/shuding0307">
        <img src="https://github.com/shuding0307.png" width="100" alt="shuding0307" /><br />
        <sub><b>shuding0307</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/jjaeho0415">
        <img src="https://github.com/jjaeho0415.png" width="100" alt="jjaeho0415" /><br />
        <sub><b>jjaeho0415</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/d0-neii">
        <img src="https://github.com/d0-neii.png" width="100" alt="d0-neii" /><br />
        <sub><b>d0-neii</b></sub>
      </a>
    </td>
  </tr>
</table>

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<!-- CONTACT -->
<a id="ko-contact"></a>

## 연락처

이수현 · [@shuding0307](https://github.com/shuding0307)

프로젝트 링크: [https://github.com/shuding0307/PlanU-FE](https://github.com/shuding0307/PlanU-FE/tree/dev)

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<!-- ACKNOWLEDGMENTS -->
<a id="ko-acknowledgments"></a>

## 참고 및 감사

* [Plan-You/PlanU-FE](https://github.com/Plan-You/PlanU-FE): 원본 팀 레포지토리
* [Best-README-Template](https://github.com/othneildrew/Best-README-Template)
* [Shields.io](https://shields.io)

<p align="right">(<a href="#readme-top">맨 위로</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/Plan-You/PlanU-FE.svg?style=for-the-badge
[contributors-url]: https://github.com/Plan-You/PlanU-FE/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Plan-You/PlanU-FE.svg?style=for-the-badge
[forks-url]: https://github.com/Plan-You/PlanU-FE/network/members
[stars-shield]: https://img.shields.io/github/stars/Plan-You/PlanU-FE.svg?style=for-the-badge
[stars-url]: https://github.com/Plan-You/PlanU-FE/stargazers
[issues-shield]: https://img.shields.io/github/issues/Plan-You/PlanU-FE.svg?style=for-the-badge
[issues-url]: https://github.com/Plan-You/PlanU-FE/issues
[React.js]: https://img.shields.io/badge/React_18-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://react.dev/
[TypeScript]: https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white
[TypeScript-url]: https://www.typescriptlang.org/
[Vite]: https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white
[Vite-url]: https://vitejs.dev/
[TanStackQuery]: https://img.shields.io/badge/TanStack_Query_v5-FF4154?style=for-the-badge&logo=reactquery&logoColor=white
[TanStackQuery-url]: https://tanstack.com/query
[Zustand]: https://img.shields.io/badge/Zustand-443E38?style=for-the-badge&logo=react&logoColor=white
[Zustand-url]: https://zustand-demo.pmnd.rs/
[ReactRouter]: https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=reactrouter&logoColor=white
[ReactRouter-url]: https://reactrouter.com/
[ReactHookForm]: https://img.shields.io/badge/React_Hook_Form-EC5990?style=for-the-badge&logo=reacthookform&logoColor=white
[ReactHookForm-url]: https://react-hook-form.com/
[Storybook]: https://img.shields.io/badge/Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=white
[Storybook-url]: https://storybook.js.org/
