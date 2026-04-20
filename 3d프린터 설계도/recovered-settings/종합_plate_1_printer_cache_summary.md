# 종합_plate_1 실제 출력 복구 (프린터 cache 기준)

이 문서는 **현재 저장된 프로젝트 파일이 아니라, 프린터 cache에 남아 있던 실제 출력용 파일** 기준이다.

## 실제 근거 파일
- `/tmp/bambu_recover/plate1.3mf`
- `/tmp/bambu_recover/plate1.gcode`
- 원격 원본:
  - `ftps://192.168.0.6/cache/종합_plate_1.3mf`
  - `ftps://192.168.0.6/cache/종합_plate_1_plate_1.gcode`

## plate 1 실제 기록
- 프로젝트명: `종합_plate_1`
- 프린터: `Bambu Lab P1S`
- 프린터 프리셋: `Bambu Lab P1S 0.4 nozzle`
- 베드: `Textured PEI Plate`
- 필라멘트: `PETG`
- 사용량: `79.69 g`
- tray_info_idx: `GFG01`
- 로컬 AMS 매핑 기준 슬롯 추정: `A4`
- gcode header 무게: `79.69 g`

## 실제 슬라이스 설정
- print_settings_id: `카리브디스권장설정`
- 레이어 높이: `0.15`
- 첫 레이어: `0.15`
- support_type: `normal(auto)`
- support_style: `grid`
- support_threshold_angle: `50`

## 퍼지스킨
- gcode 기준 `fuzzy_skin = none`
- gcode 기준 `fuzzy_skin_point_distance = 0.8`
- gcode 기준 `fuzzy_skin_thickness = 1`
- printer cache 3mf 기준 `fuzzy_skin = none`
- printer cache 3mf 기준 `fuzzy_skin_thickness = 1`

## 결론
이전 복구가 틀렸던 이유는 **현재 저장된 종합.3mf** 를 기준으로 봤기 때문이다.
실제 출력된 `종합_plate_1` 은 프린터 cache 기준으로 **PETG 79.69g / A4 추정 / 카리브디스권장설정 / 0.15 layer** 이 맞다.
다만 **actual plate_1 gcode** 에 남아 있는 퍼지스킨 활성 모드는 `none` 이다.
