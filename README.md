# Space War / Neon Rift v427

## 구성
- index.html: 기기 판정
- pc_original.html: PC 오리지널 기반, 태블릿에서도 진짜 PC 화면으로 고정
- mobile_v392.html: 휴대폰 v392 원본 그대로

## 핵심 수정
- pc_original.html의 viewport를 데스크톱 폭으로 고정
- pc_original.html 내부 isMobile() 강제 OFF
- pc_original.html 안의 pointer:coarse 미디어쿼리 비활성화
- 모바일/태블릿 조작 UI 강제 숨김

## 판정
- iPad / Galaxy Tab / SM-X / SM-T / Tablet: 무조건 PC
- 휴대폰: 짧은 쪽 390px 이하 + 긴 쪽 850px 이하
- 태블릿/PC: 그 외 전부 pc_original.html
