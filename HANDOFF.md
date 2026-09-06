# 인수인계 (HANDOFF) — 뉴스리그 (n-league.net)

> 다른 PC의 Claude Code로 이어받을 때 이 문서를 먼저 읽어주세요.
> **프로젝트 전체 맥락·구조·다음 단계는 베이스 레포의 HANDOFF.md에 있어요:**
> https://github.com/appmong/astro_base → `HANDOFF.md`

최종 업데이트: 2026-09-05

---

## 이 레포는?

애드센스 승인용 사이트 **"뉴스리그"** (도메인 예정: `n-league.net`).
공통 베이스 템플릿(`appmong/astro_base`)에서 찍어낸 첫 테스트 사이트예요.

- 레포: **github.com/appmong/website01**
- 사이트명 `뉴스리그`, 도메인 `n-league.net`은 `src/site.config.ts`·`astro.config.mjs`·`public/robots.txt`에 이미 주입됨.

## 새 PC 셋업

```
git clone https://github.com/appmong/website01.git
cd website01
npm install
npm run dev        # http://localhost:4321
```
- Node.js 필요(`winget install OpenJS.NodeJS.LTS`).
- 미리보기가 안 되면 `.claude/launch.json`의 `node.exe` 경로를 이 PC에 맞게 수정.

## 이 사이트의 상태

- ✅ 골격·컴포넌트·필수 페이지·SEO·체류 위젯 전부 포함 (베이스와 동일)
- ✅ 빌드 15페이지 오류 0, 미리보기 검증됨
- ⬜ 콘텐츠는 견본 1편만(`src/content/posts/재산세-이의신청-기한.md`)
- ⬜ 니치·저자 프로필 확정 필요
- ⬜ 도메인 구매·배포(Cloudflare)·애드센스 신청 남음

## 자세한 내용

기술 스택, 설정 파일 설명, 새 사이트 찍어내는 법, 전체 로드맵, 함정(gotchas)은
**베이스 레포의 `HANDOFF.md`**를 보세요. (구조·워크플로우는 모든 사이트 공통)
