# Yong Jin Lee 연구자 프로필 수정 안내

CV와 프로필 사진이 반영된 GitHub Pages용 정적 웹사이트입니다. 어두운 네이비 톤을 전 영역에 통일하고, 비대칭 첫 화면, 카드형 연구 이력과 읽기 편한 글씨 체계를 적용했습니다. 2026년 9월 고려대학교 산업경영공학과 박사과정 정보, 영문 소개문, 한국자동차연구원 GPBL 및 LG전자 IPBL 활동이 반영되어 있습니다.

## 파일 구성

- `index.html`: 이름, 소개, 이메일, 학력, 논문, 경력, 학술대회, 프로젝트, 수상, 기술
- `style.css`: 네이비·블루 색상, 작은 글자 체계, 카드 배치와 모바일 화면
- `images/profile.jpg`: 별도 이미지 폴더에 저장된 실제 프로필 사진

## 컴퓨터에서 확인하기

`index.html`을 더블클릭하면 브라우저에서 바로 열립니다. 수정 후 저장하고 브라우저를 새로고침하면 됩니다.

## 아직 추가해야 할 정보

CV에 없는 GitHub와 LinkedIn 주소는 임시로 `#`으로 남겨 두었습니다. `index.html` 상단에서 다음 부분을 찾아 실제 주소로 바꿉니다.

```html
<a href="#" aria-label="GitHub link to be added"
```

예시:

```html
<a href="https://github.com/본인아이디" aria-label="GitHub"
```

LinkedIn도 같은 방식으로 변경합니다. 계정이 없다면 `<div class="social-links">`부터 해당 `</div>`까지 삭제할 수 있습니다.

## 논문 추가하기

`index.html`에서 다음 블록을 복사하고 내용만 변경합니다.

```html
<li class="publication-item">
  논문 정보를 입력합니다.
</li>
```

본인 이름은 `<strong>Yong Jin Lee</strong>`로 작성하면 굵게 표시됩니다. 저널명은 `<em>Journal Name</em>`으로 작성합니다.

## GitHub Pages에 올리기

1. GitHub에서 새 저장소를 생성합니다.
2. 저장소 이름을 정확히 `내아이디.github.io`로 지정합니다.
3. `index.html`, `style.css`, `README.md`, `images` 폴더를 구조 그대로 업로드합니다.
4. `Settings → Pages`로 이동합니다.
5. Source를 `Deploy from a branch`로 설정합니다.
6. Branch는 `main`, 폴더는 `/(root)`를 선택합니다.
7. 잠시 후 `https://내아이디.github.io/`에서 확인합니다.

## 개인정보 안내

공개 웹페이지에는 이메일만 반영했습니다. CV에 있는 휴대전화 번호는 넣지 않았습니다. 전화번호를 공개하려면 `index.html`의 `contact-lines` 영역에 직접 추가할 수 있습니다.
