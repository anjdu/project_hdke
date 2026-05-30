# 홍대 키이스케이프 — 배포용 빌드 (dist)

이미지·CSS·스크립트가 **각 HTML 안에 모두 포함**된 자체완결형 빌드입니다.
외부에서 불러오는 건 **영상뿐**입니다.

## 올리는 법 (GitHub Pages)

1. 이 `dist/` 폴더 안의 파일을 레포 루트에 업로드
2. `videos/` 폴더를 만들고 아래 이름으로 영상 업로드
3. **Settings → Pages → Branch** 를 `main` / `/(root)` 로 설정

```
index.html      ← 루트 진입 → pretbbo.html 자동 이동
pretbbo.html    ← 삐릿뽀
holiday.html    ← 홀리데이
goback.html     ← 고백
videos/         ← 직접 업로드 (아래 이름 규칙)
```

## 영상 이름 규칙 (`videos/` 폴더)

| 페이지 | 영상 파일 |
|--------|-----------|
| pretbbo | `p1.mp4` `p2.mp4` `p3.mp4` `p4.mp4` |
| holiday | `h1.mp4` `h2.mp4` `h3.mp4` `h4.mp4` |
| goback  | `g1.mp4` `g2.mp4` `g3.mp4` `g4.mp4` |

각 페이지 하단 영상 섹션에 1→4 순서로 로딩됩니다.

## 참고

- 이미지는 웹용으로 압축(다운스케일 + JPEG/PNG)되어 인라인됐습니다. 원본 25MB+ → 페이지당 3~5MB.
- 내용을 다시 수정하려면 **편집용 원본**(`pretbbo.html` / `holiday.html` / `goback.html`, dist 바깥)에서 Tweaks로 고친 뒤 이 빌드를 다시 만들어 주세요. dist 파일은 직접 편집용이 아닙니다.
