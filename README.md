# thetree-skin-liberty (`jeoriga-liberty` branch)

> 본 브랜치는 [thetree-skin-liberty](https://github.com/wjdgustn/thetree-skin-liberty) 의 파생물(fork) 입니다.
> 원본은 **GPL-3.0-or-later** 라이선스로 공개되어 있으며, 본 파생본 또한 **동일한 GPL-3.0-or-later** 로 배포됩니다.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Branch: jeoriga-liberty](https://img.shields.io/badge/branch-jeoriga--liberty-informational)](https://github.com/Kuco-dev/thetree-skin-liberty/tree/jeoriga-liberty)

> **저장소 구조 안내**
> 본 저장소(`Kuco-dev/thetree-skin-liberty`)는 GitHub fork 기능으로 [`wjdgustn/thetree-skin-liberty`](https://github.com/wjdgustn/thetree-skin-liberty) 를 포크한 뒤, 한 저장소 안에서 두 개의 변형을 브랜치로 운영합니다.
> - **이 브랜치(`jeoriga-liberty`)** — 본 README 가 적용되는 브랜치. 스킨 설정 키 네임스페이스가 `skin.jeoriga-liberty.*` 로 분리되어 있고, notfound 워터마크가 `/jeoriga.png` 한 장으로 고정된 변형.
> - [`liberty`](https://github.com/Kuco-dev/thetree-skin-liberty/tree/liberty) — 스킨 설정 키는 원본과 동일한 `skin.liberty.*` 를 그대로 쓰고, notfound 워터마크가 `/notfound1.png` / `/notfound2.png` 중 랜덤 선택되는 변형.
> - `master` — 원작자 저장소(`wjdgustn/thetree-skin-liberty`) 의 기본 브랜치를 그대로 추적하는 fork 의 기본 브랜치. 본 fork 에서는 직접 수정하지 않고 upstream 동기화 용도로만 유지합니다.
>
> 즉, 저장소 자체가 GitHub 상에서 원본의 fork 로 표시되며(저장소 페이지의 "forked from wjdgustn/thetree-skin-liberty" 표기), 그 fork 안에서 `liberty` / `jeoriga-liberty` 두 작업 브랜치로 분기한 구조입니다.

## 개요

`thetree` 위키 엔진용 Liberty 스킨의 커스터마이즈 버전입니다. 원본 스킨에 다음을 추가/변경하였습니다.

- **스킨 설정 키 네임스페이스 분리**: thetree 엔진의 스킨 설정 키를 `skin.liberty.*` → `skin.jeoriga-liberty.*` 로 일괄 변경(13개 키). 같은 thetree 인스턴스에서 원본 `liberty` 스킨과 본 변형이 공존해도 설정 영역이 충돌하지 않도록 분리.
- **404(notfound) 페이지 워터마크**: 존재하지 않는 문서에 진입했을 때 `.wiki-article` 영역에 워터마크 이미지를 자동 표시. 워터마크 src 는 `/jeoriga.png` 로 고정.
- **드롭다운 메뉴 정렬 변경**: `파일 올리기` 항목을 메뉴 상단에서 `RandomPage`와 `라이선스` 사이로 이동.
- **`@keyframes name-gradient` CSS 추가**: 닉네임/로고 텍스트 등에 그라디언트 흐름 애니메이션을 적용하기 위한 키프레임 정의(`css/default.css` 끝).
- **`--liberty-navbar-logo-image` fallback 단순화**: `wiki.logo_url` 가드(`&&`)를 제거하여 코드 단순화.
- **상단 네비게이션 바에 "랭킹" 외부 링크 추가**: `최근 변경` 좌측에 `https://rank.kemonofantasy.world` 로 연결되는 외부 링크 아이템(`fa fa-trophy`) 추가. `target="_blank" rel="noopener noreferrer"` 적용.

## 원본(Upstream) 출처

| 항목 | 값 |
|---|---|
| 원작자 | **wjdgustn** — <https://github.com/wjdgustn> |
| 원본 저장소 | <https://github.com/wjdgustn/thetree-skin-liberty> |
| 본 저장소(GitHub fork) | <https://github.com/Kuco-dev/thetree-skin-liberty> |
| Fork 베이스 브랜치 | `master` (upstream 의 기본 브랜치) |
| 본 작업 브랜치 | `jeoriga-liberty` |
| 사용 엔진 | [the tree](https://github.com/wjdgustn/thetree) |
| Liberty Skin 의 원조 | [Librewiki / Liberty-MW-Skin](https://gitlab.com/librewiki/Liberty-MW-Skin) — Copyright (C) 2016 Liberty LLC. |

수정되지 않은 원본 코드는 위 원본 저장소 또는 본 fork 의 `master` 브랜치(upstream 추적용)에서 그대로 받을 수 있습니다.

## 라이선스

본 브랜치는 **GNU General Public License v3.0 또는 그 이후 버전(GPL-3.0-or-later)** 으로 배포됩니다.

- SPDX 식별자: `GPL-3.0-or-later`
- 라이선스 전문: 저장소의 [`LICENSE`](./LICENSE) 파일 (원본 라이선스 파일을 그대로 보존)
- GNU 공식 원문: <https://www.gnu.org/licenses/gpl-3.0.html>

```
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <https://www.gnu.org/licenses/>.
```

## 수정 사항 (Modifications, GPL-3.0 §5(b))

원본 `wjdgustn/thetree-skin-liberty` 대비 본 브랜치에서 변경된 항목입니다. 줄 단위 diff 는 `git diff master..jeoriga-liberty` 또는 GitHub 브랜치 비교 화면에서 확인할 수 있습니다.

| 일자 | 파일 | 유형 | 요약 |
|---|---|---|---|
| 2026-04-30 | `README.md` | 수정 | 원작자 출처 / GPL-3.0 고지 / 수정 사항 표 / 수정자 정보 추가 |
| 2026-04-30 | `layout.vue` | 수정 | 스킨 설정 키 네임스페이스 변경 — `skin.liberty.*` 13개 키를 `skin.jeoriga-liberty.*` 로 일괄 치환 (아래 §"변경된 설정 키 목록" 참고). |
| 2026-04-30 | `layout.vue` | 추가 | `notfound` 페이지 워터마크 기능 (`updateNotFoundImage` 메서드, `watch['$store.state.page.viewName']`, `mounted()` 훅). 워터마크 src 는 `/jeoriga.png` 로 고정. |
| 2026-04-30 | `layout.vue` | 수정 | 드롭다운 메뉴의 `파일 올리기` 위치 이동(상단 → 메뉴 끝쪽). `dropdown-divider` 1개 제거. |
| 2026-04-30 | `layout.vue` | 수정 | `--liberty-navbar-logo-image` 의 `wiki.logo_url` 가드(`&&`) 제거. |
| 2026-04-30 | `css/default.css` | 추가 | `@keyframes name-gradient { 0%/50%/100% background-position-x }` 정의 12줄 추가. |
| 2026-05-07 | `README.md` | 수정 | 미해결 git merge conflict 마커(`<<<<<<< HEAD` / `=======` / `>>>>>>> d071cbc` / `>>>>>>> a38b795` / `>>>>>>> f0e95db` / `>>>>>>> 235d006`) 일괄 제거. `jeoriga-liberty` 분기 측 내용으로 통합. |
| 2026-05-07 | `layout.vue` | 수정 | 미해결 git merge conflict 마커(`<<<<<<< HEAD` / `=======` / `>>>>>>> d071cbc` / `>>>>>>> 8a7340c` / `>>>>>>> 235d006`) 제거. `notfound-watermark` 의 `src` 를 `/jeoriga.png` 로 확정. footer Github 링크를 `tree/jeoriga-liberty` 로 확정. |
| 2026-05-07 | `layout.vue` | 추가 | 상단 네비게이션 바 `최근 변경` 좌측에 외부 링크 `<li>` 추가. `https://rank.kemonofantasy.world` 로 연결되는 "랭킹" 항목(`fa fa-trophy`, `target="_blank" rel="noopener noreferrer"`). |

폰트(`fonts/`) / 이미지 / `LICENSE` / `.editorconfig` / `.gitignore` / `components/` / `layouts/` / `css/` 의 다른 파일 / `bootstrap.min.css` / `font-awesome.min.css` 등은 **원본과 동일** 합니다.

### 변경된 설정 키 목록

다음 13개 키가 `skin.liberty.X` → `skin.jeoriga-liberty.X` 로 변경되었습니다. **기존 `skin.liberty.*` 설정값은 자동으로 이전되지 않으므로**, 본 브랜치를 적용한 후 thetree 어드민 페이지에서 새 키로 다시 입력해야 합니다.

```
skin.liberty.navbar_logo_text          → skin.jeoriga-liberty.navbar_logo_text
skin.liberty.footer_html               → skin.jeoriga-liberty.footer_html
skin.liberty.brand_color_1             → skin.jeoriga-liberty.brand_color_1
skin.liberty.brand_color_2             → skin.jeoriga-liberty.brand_color_2
skin.liberty.brand_dark_color_1        → skin.jeoriga-liberty.brand_dark_color_1
skin.liberty.brand_bright_color_1      → skin.jeoriga-liberty.brand_bright_color_1
skin.liberty.brand_bright_color_2      → skin.jeoriga-liberty.brand_bright_color_2
skin.liberty.navbar_logo_image         → skin.jeoriga-liberty.navbar_logo_image
skin.liberty.navbar_logo_minimum_width → skin.jeoriga-liberty.navbar_logo_minimum_width
skin.liberty.navbar_logo_width         → skin.jeoriga-liberty.navbar_logo_width
skin.liberty.navbar_logo_size          → skin.jeoriga-liberty.navbar_logo_size
skin.liberty.navbar_logo_padding       → skin.jeoriga-liberty.navbar_logo_padding
skin.liberty.navbar_logo_margin        → skin.jeoriga-liberty.navbar_logo_margin
```

## 외부 자산 의존

본 브랜치의 코드가 참조하는 정적 파일은 다음과 같습니다. 저장소에 포함되어 있지 않으므로 배포 환경에서 별도로 제공해야 합니다.

- `/jeoriga.png` (실제 워터마크로 사용)
- `/notfound1.png`, `/notfound2.png` (코드에 변수만 남아 있고 실제 src 로는 사용되지 않음 / 데드 코드. 정리 시 함께 제거 권장)

본 브랜치의 코드가 참조하는 외부(원격) 엔드포인트는 다음과 같습니다. 본 저장소가 운영하지 않으며, 가용성/콘텐츠/보안 정책은 해당 도메인 운영자 책임입니다.

- `https://rank.kemonofantasy.world` (상단 네비게이션 "랭킹" 링크의 대상 URL)

## 수정자 정보

| 항목 | 값 |
|---|---|
| 수정자 | **KucoSang** |
| 연락처 | <kucosang@gmail.com> |
| 본 fork 시작일 | 2026-04-30 |
| 최근 갱신일 | 2026-05-07 |

## 원본과의 관계

- 본 저장소는 GitHub 의 fork 기능으로 `wjdgustn/thetree-skin-liberty` 를 포크한 것이며, GitHub 상단에 fork 관계가 표시됩니다.
- 본 브랜치(`jeoriga-liberty`)는 그 fork 의 `master` 브랜치(=upstream 추적 브랜치) 에서 분기하여 추가 수정을 적용한 작업 브랜치입니다.
- 변경 사실/일자는 위 §"수정 사항" 표 및 git 커밋 메시지 트레일러(`Original-Source:`, `Modified-By:`, `Modified-Date:`, `License: GPL-3.0-or-later`)에 명시됩니다.
- upstream 의 변경 사항을 가져올 때는 `master` 브랜치에서 sync 후 본 브랜치로 merge 하고, 머지 커밋에 `Upstream-Commit:` 트레일러를 갱신해 둡니다.

## 설치 / 사용 방법

본 스킨은 `the tree` 엔진의 스킨 디렉터리에 배치하여 사용합니다. 원본 README 의 설치 절차와 동일합니다.
thetree 어드민 페이지에서 설정 키를 입력할 때 **`skin.liberty.*` 가 아니라 `skin.jeoriga-liberty.*`** 네임스페이스를 사용해야 함에 주의하세요.

## 기여 / 이슈

PR 환영합니다. 라이선스 위반 의심 사항이나 GPL 관련 문의는 위 연락처로 알려 주십시오.

## Acknowledgements

- 원작자 **wjdgustn** — `thetree-skin-liberty` 및 `the tree` 엔진의 저자.
- **Librewiki / Liberty LLC.** — Liberty-MW-Skin 의 원조 저작권자 (Copyright (C) 2016 Liberty LLC.). <https://librewiki.net/>
- 본 fork 의 기여자 목록은 git history (`git log`) 에서 확인할 수 있습니다.

---

> This branch is a fork of [thetree-skin-liberty](https://github.com/wjdgustn/thetree-skin-liberty)
> by **wjdgustn**, distributed under **GPL-3.0-or-later**. Modifications and modification dates
> are summarized in the *Modifications* section above, in accordance with GPL-3.0 §5(a)(b)(c).
> Full license text: [`LICENSE`](./LICENSE) / <https://www.gnu.org/licenses/gpl-3.0.html>.
