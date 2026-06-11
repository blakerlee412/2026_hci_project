## 프로젝트 소개

인도 레스토랑에서 실제로 사용할 수 있는 QR 기반 비대면 주문 시스템입니다.
테이블마다 QR 코드를 붙여두면 고객이 직접 스마트폰으로 스캔해서 주문하고, 직원은 관리자 페이지에서 실시간으로 주문을 확인할 수 있습니다.

## 사용 기술

- React, Vite
- Firebase Firestore (실시간 DB)
- Vercel (배포)

## 주요 기능

- 테이블별 QR 코드 생성 및 인쇄
- 메뉴 탐색 및 옵션 선택 후 장바구니 주문
- 인원수, 매운맛, 채식 여부 기반 메뉴 추천 필터
- 관리자 페이지에서 주문 상태 실시간 관리 (접수 → 준비중 → 완료)

## 배포 링크

바로 실행해보실 수 있습니다.

- 고객 주문 페이지: https://menu-app-six-beryl.vercel.app/menu?table=1
- 관리자 페이지: https://menu-app-six-beryl.vercel.app/admin (비밀번호: indic1234)
- QR 코드 페이지: https://menu-app-six-beryl.vercel.app/qr

## 로컬 실행 방법

### 사전 준비

Node.js가 설치되어 있어야 합니다. 아래 명령어로 확인하세요.

```bash
node -v
```

v18 이상이면 됩니다. 없으면 https://nodejs.org 에서 LTS 버전을 설치해주세요.

### 실행

```bash
# 프로젝트 폴더로 이동
cd menu-app

# 패키지 설치 (최초 1회)
npm install

# 개발 서버 실행
npm run dev
```

실행 후 브라우저에서 아래 주소로 접속합니다.

| 주소 | 설명 |
|---|---|
| http://localhost:5173/menu?table=1 | 고객 주문 화면 |
| http://localhost:5173/admin | 관리자 페이지 (비밀번호: indic1234) |
| http://localhost:5173/qr | QR 코드 생성 |


