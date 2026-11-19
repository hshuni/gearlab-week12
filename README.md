# GEARLAB 게이밍 기어 전문 쇼핑몰

웹프로그래밍 12주차 HTML5 DOM 활용 실습입니다. Razer, Logitech G, CORSAIR의 키보드 5개, 마우스 5개, 헤드셋 4개, 이어폰 4개를 검색하고 주요 사양을 비교할 수 있습니다.

## 실행 및 제출

1. ZIP 압축을 풀고 `index.html`을 더블클릭합니다. `img` 폴더는 `index.html`과 같은 위치에 둡니다.
2. GitHub Pages로 제출하려면 GitHub 저장소의 `main` 브랜치 루트에 `index.html`과 `img` 폴더를 올립니다.
3. 저장소의 **Settings → Pages → Deploy from a branch**에서 `main`과 `/(root)`를 선택하고 저장합니다. 배포가 끝나면 Pages 설정에 표시된 사이트 주소를 확인합니다.

[GitHub Pages 배포 방법](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## 시연 순서

1. 추천 배너를 넘기고 제품 상세의 브랜드 공식 링크를 확인합니다.
2. 마우스 카테고리를 누른 뒤 Viper V3 Pro와 PRO X SUPERLIGHT 2를 비교 목록에 담고 **제품 비교**를 누릅니다.
3. **멤버십**에서 닉네임을 등록합니다. Viper V3 Pro 한 개를 장바구니에 담아 모의 결제하면 베이직 기준 2,290 P가 적립되고 실버로 승급합니다.
4. 새로고침한 뒤 **멤버십**을 열어 등급과 포인트가 유지되는지 확인합니다.

표시 가격과 결제는 실습용입니다. 회원과 장바구니 데이터는 현재 브라우저의 localStorage에 저장됩니다.

## 과제용 프롬프트

너는 게이밍 기어 쇼핑몰 디렉터야. Razer, Logitech G, CORSAIR의 게이밍 키보드, 마우스, 헤드셋, 이어폰을 판매하는 가상의 온라인 쇼핑몰을 만들어줘. 이름은 GEARLAB으로 하고 브랜드 공식 제품 사진으로 상품 카드를 만들어줘. 짙은 보라색 배경에 라임색 버튼을 쓰고, 추천 제품 이미지 세 장이 교차하는 메인 슬라이드와 네 가지 상품 분류 버튼을 넣어줘. 키보드와 마우스는 각각 5개, 헤드셋과 이어폰은 각각 4개씩 구성해줘. 카테고리와 브랜드 필터, 제품명 검색, 가격순 정렬, 상세 보기, 최대 세 제품의 사양 비교, 장바구니 수량 조절과 모의 결제를 구현해줘. 데모 회원은 브라우저에서 닉네임으로 등록하고, 모의 결제 누적 금액에 따라 등급과 적립률을 바꿔줘. HTML5 DOM과 JavaScript 이벤트를 활용해서 사용자 조작에 따라 화면이 갱신되게 해줘. CSS와 JavaScript는 하나의 index.html에 넣고, 제품 이미지는 img 폴더에 상대경로로 연결해줘. 모바일에서도 사용할 수 있고 GitHub Pages에서 바로 실행되는 구조로 만들어줘.

## 제품 이미지 출처

브랜드 공식 사이트에서 받은 제품 사진을 WebP로 저장했습니다. 사진과 브랜드 표기의 권리는 각 권리자에게 있습니다.

| 브랜드 | 상품 | 파일 | 출처 |
| --- | --- | --- | --- |
| Razer | Viper V3 Pro | `img/viper.webp` | [공식 이미지](https://medias-p1.phoenix.razer.com/sys-master-phoenix-images-container/h08/h61/9765618188318/viper-v3-pro-black-500x500.png) |
| Logitech G | G515 LIGHTSPEED TKL | `img/g515.webp` | [공식 이미지](https://resource.logitechg.com/c_fill,q_auto,f_auto,dpr_1.0/d_transparent.gif/content/dam/gaming/en/products/g515-lightspeed-tkl/gallery/g515-keyboard-black-gallery-1-kor.png) |
| CORSAIR | HS80 MAX WIRELESS | `img/hs80.webp` | [공식 이미지](https://assets.corsair.com/image/upload/c_pad,q_auto,h_1024,w_1024,f_auto/products/Gaming-Headsets/hs80-max-wireless/steel-grey/HS80_MAX_WIRELESS_STEEL_GRAY_01.webp) |
| Logitech G | PRO X SUPERLIGHT 2 | `img/superlight.webp` | [공식 이미지](https://resource.logitechg.com/c_fill,q_auto,f_auto,dpr_1.0/d_transparent.gif/content/dam/gaming/en/products/pro-x-superlight-2/new-gallery-assets-2025/pro-x-superlight-2-mice-top-angle-white-gallery-1.png) |
| CORSAIR | K65 PLUS WIRELESS | `img/k65.webp` | [공식 이미지](https://assets.corsair.com/image/upload/c_pad,q_auto,h_1024,w_1024,f_auto/products/Gaming-Keyboards/base-k65-plus-wireless-config/gallery/CH-91D401L-NA/K65_PLUS_WIRELESS_01.webp) |
| Razer | Hammerhead HyperSpeed | `img/buds.webp` | [공식 이미지](https://medias-p1.phoenix.razer.com/sys-master-phoenix-images-container/hb0/ha7/9447214219294/hammerhead-hyperspeed-ps-v2-500x500.png) |
| Razer | Huntsman V3 Pro Mini | `img/huntsman.webp` | [공식 이미지](https://medias-p1.phoenix.razer.com/sys-master-phoenix-images-container/h61/h66/9705254158366/huntsman-v3-pro-mini-2-500x500.png) |
| Logitech G | G213 Prodigy | `img/g213.webp` | [공식 이미지](https://resource.logitechg.com/c_fill,q_auto,f_auto,dpr_1.0/d_transparent.gif/content/dam/gaming/en/non-braid/g213-finch/g213-gallery-1-nb.png) |
| CORSAIR | K70 CORE RGB | `img/k70.webp` | [공식 이미지](https://assets.corsair.com/image/upload/c_pad,q_auto,h_1024,w_1024,f_auto/products/Gaming-Keyboards/k70-core/Gallery/CH-910971E/CH-910971E_01.webp) |
| Razer | Cobra | `img/cobra.webp` | [공식 이미지](https://medias-p1.phoenix.razer.com/sys-master-phoenix-images-container/h54/h60/9591466950686/cobra-500x500.png) |
| Logitech G | G305 LIGHTSPEED | `img/g305.webp` | [공식 이미지](https://resource.logitechg.com/c_fill,q_auto,f_auto,dpr_1.0/d_transparent.gif/content/dam/gaming/en/products/g305/2025-update/g305-lightspeed-mouse-top-angle-lilac-gallery-1.png) |
| Logitech G | G502 X PLUS | `img/g502.webp` | [공식 이미지](https://resource.logitechg.com/c_fill,q_auto,f_auto,dpr_1.0/d_transparent.gif/content/dam/gaming/en/products/g502x-plus/2026-update/gallery/g502-x-plus-top-angle-black-gallery-1.png) |
| Razer | BlackShark V2 HyperSpeed | `img/blackshark.webp` | [공식 이미지](https://medias-p1.phoenix.razer.com/sys-master-phoenix-images-container/he0/h7f/9807445917726/240820-BlackShark-V2-Hyperspeed-500x500.png) |
| Logitech G | G733 LIGHTSPEED | `img/g733.webp` | [공식 이미지](https://resource.logitechg.com/c_fill,q_auto,f_auto,dpr_1.0/d_transparent.gif/content/dam/gaming/en/products/g733/gallery/g733-lilac-gallery-1.png) |
| Logitech G | PRO X 2 LIGHTSPEED | `img/prox2.webp` | [공식 이미지](https://resource.logitechg.com/c_fill,q_auto,f_auto,dpr_1.0/d_transparent.gif/content/dam/gaming/en/products/pro-x-2-lightspeed/gallery/gallery-1-pro-x-2-lightspeed-gaming-headset-white.png) |
| Razer | Hammerhead V3 Chroma | `img/chroma.webp` | [공식 이미지](https://medias-p1.phoenix.razer.com/sys-master-phoenix-images-container/h8f/hf0/10537386442782/hammerhead-v3-chroma-500x500.png) |
| Razer | Hammerhead V3 HyperSpeed | `img/hyper3.webp` | [공식 이미지](https://medias-p1.phoenix.razer.com/sys-master-phoenix-images-container/h00/hb8/10045185622046/hammerhead-v3-hyperspeed-500x500.png) |
| Razer | Hammerhead V3 X HyperSpeed | `img/hyper3x.webp` | [공식 이미지](https://medias-p1.phoenix.razer.com/sys-master-phoenix-images-container/hba/hba/10045185589278/hammerhead-v3-x-hyperspeed-500x500.png) |
