# Yong Jin Lee 연구자 프로필 수정 안내

CV와 프로필 사진이 반영된 GitHub Pages용 웹사이트임
어두운 네이비 톤을 전 영역에 통일하고, 비대칭 첫 화면, 카드형 연구 이력과 읽기 편한 글씨 체계를 적용함

## 파일 구성

- `index.html`: 이름, 소개, 이메일, 학력, 논문, 경력, 학술대회, 프로젝트, 수상, 기술
- `style.css`: 네이비·블루 색상, 작은 글자 체계, 카드 배치와 모바일 화면
- `images/profile.jpg`: 별도 이미지 폴더에 저장된 실제 프로필 사진

## 컴퓨터에서 확인하기

`index.html`을 더블클릭하면 브라우저에서 확인 가능하며 수정 후 저장하고 브라우저를 새로고침 하면 됨

## 논문 추가하기

`index.html`에서 다음 블록을 복사하고 내용만 변경

```html
<li class="publication-item">
  논문 정보를 입력합니다.
</li>
```

본인 이름은 `<strong>Yong Jin Lee</strong>`로 작성하면 굵게 표시되며 저널명은 `<em>Journal Name</em>`으로 작성하면됨

## GitHub Pages에 올리기

1. GitHub에서 새 저장소를 생성
2. 저장소 이름을 정확히 `내아이디.github.io`로 지정
3. `index.html`, `style.css`, `README.md`, `images` 폴더를 구조로 업로드
4. `Settings → Pages`로 이동
5. Source를 `Deploy from a branch`로 설정
6. Branch는 `main`, 폴더는 `/(root)`를 선택
7. 잠시 후 `https://내아이디.github.io/`에서 확인
