# 식사일기 음식 데이터

식사일기의 데이터 전용 업데이트 저장소입니다. 앱 소스 코드, 식사·건강 기록, 개인 음식과 인증 정보는 포함하지 않습니다.

## 출처

- 식약처 K-FIND 음식 DB 2026-08-28 / 가공식품 DB 2026-10-29: https://various.foodsafetykorea.go.kr/nutrient/general/down/historyList.do
- 농촌진흥청 국가표준식품성분 DB 10.4: https://koreanfood.rda.go.kr/
- 공식 브랜드 보완: 빽다방 https://paikdabang.com/menu/menu_new/ · 이디야 https://www.ediya.com/contents/drink.html · 공차 https://www.gong-cha.co.kr/brand/menu/product_nutrition · 할리스 https://www.hollys.co.kr/menu/espresso.do · 롯데리아 https://www.lotteeatz.com/upload/etc/ria/items.html
- 공식 웹 보완의 sourceDate/checkedDate는 확인일, generatedDate는 원문 기준일(미공개 가능), manifest.published는 배포일입니다. 컵 용량과 중량은 환산하지 않습니다.
- 각 항목의 source, version, sourceDate, url에 출처를 보존합니다. 칼로리는 기록을 돕는 추정값이며 현재 판매 메뉴와 다를 수 있습니다.

## 브랜드 보완 범위

카페: 스타벅스, 투썸플레이스, 이디야, 메가커피, 컴포즈커피, 빽다방, 공차, 할리스.
버거 단품: 맥도날드, 버거킹, 롯데리아, 맘스터치.

공식 영양정보가 확인된 항목만 검토 후 반영합니다. 신메뉴를 실시간 수집하는 서비스가 아니며, 사이즈·온도·제공량·출처가 확인되지 않는 값은 추정해 추가하지 않습니다.

## 배포 형식

manifest.json은 배포 번호·배포일·SHA-256·크기·개수를 포함합니다. catalog-<SHA-256>.json은 불변 데이터입니다. 데이터 파일을 먼저 배포한 후 manifest.json을 갱신합니다. 수정 또는 이전 내용 복구도 배포 번호를 올려 배포합니다.
