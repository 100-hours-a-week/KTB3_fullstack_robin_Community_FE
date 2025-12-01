# 그나저나 (Frontend)
주제를 바꿔 대화를 이어가는 말 '그나저나'<br>이곳에서 여러 주제의 대화를 끊임없이 이어가보세요!<br><br>

## 개요
정적 HTML/CSS/JS만으로 구성한 소셜 피드 UI. 로그인·게시글·프로필 흐름을 브라우저 단에서 구현했습니다.
- 개발기간: 25.11.03 ~ 
- 개발인원: 1명

### 소개영상
![소개영상+(1) (1)](https://github.com/user-attachments/assets/9835f474-bbd1-4185-befa-2926ed3ad462)
- 음성포함)고화질 영상 링크 : [![그나저나_소개영상](www.youtube.com)](https://youtu.be/mygmCDOUXP4)


## 제공 기능
- 🔑 로그인/로그아웃, 토큰 자동 갱신, 기본 입력 검증
- 🆕 회원가입: 이메일·닉네임 중복 확인, 프로필 이미지 업로드
- 📰 피드: 무한 스크롤 목록, 작성자 아바타, 카드 클릭 시 상세 이동
- 📄 상세: 좋아요, 조회·댓글 카운트, 댓글 작성/수정/삭제, 작성자만 글 수정·삭제
- ✏️ 글 작성/수정: 제목 길이 제한, 본문 필수, 이미지 첨부
- 👤 프로필: 닉네임 변경, 프로필 이미지 업로드/삭제, 회원 탈퇴
- 🔒 비밀번호 변경 후 토스트 안내

## 기술 스택·구조
- 정적 HTML/CSS와 Vanilla JS(ES Modules). **이후 React 로 마이그레이션 예정.**
- 기본 폴더: `static/html`(페이지), `static/css`(스타일), `static/assets`(이미지), `static/app`(JS)
- JS는 공용 유틸(core)·도메인 API(features)·UI 컴포넌트(components)·페이지 스크립트(pages)로 나눔

## 페이지 맵
- `login.html`, `signup.html`: 인증 진입
- `postList.html`, `postDetail.html`, `postWrite.html`, `postEdit.html`: 피드/상세/작성·수정
- `editUserInfo.html`, `editPassword.html`: 프로필·비밀번호 관리
