# 종합 plate 1 / plate 9 복구 설정

- 복구 기준 파일: `/Users/chenjing/dev/카리브디스/3d프린터 설계도/종합.3mf`
- 기준 시점: 프로젝트 내부 `project_settings.config`
- 대상 출력물: `종합_plate_1`, `종합_plate_9`
- 프린터: `Bambu Lab P1S`
- 프린터 프리셋: `Bambu Lab P1S 0.4 nozzle`
- 베드: `Textured PEI Plate`
- 노즐: `0.4 mm`
- 베이스 프로세스 프로필: `0.08mm Extra Fine @BBL X1C`
- 실제 사용 필라멘트(Extruder 1): `Bambu PLA Silk @BBL X1C`

## 핵심 설정
- 레이어 높이: `0.08 mm`
- 첫 레이어: `0.2 mm`
- 벽 수: `4`
- 상단 레이어: `9`
- 하단 레이어: `7`
- 인필: `70%` / `grid`
- 브림: `auto_brim` / `5 mm`
- 서포트: `tree(auto)` / build plate only=`1` / critical only=`1` / angle=`15`
- 래프트 레이어: `3`

## 속도
- 외벽: `['50', '200']`
- 내벽: `['50', '350']`
- 탑서피스: `['50', '200']`
- 인필: `['50', '450']`
- 서포트: `['50', '150']`
- 서포트 인터페이스: `['50', '80']`
- 이동: `['300', '500']`

## 온도 / 냉각 (Extruder 1 기준)
- 노즐: `210°C`
- 첫 레이어 노즐: `210°C`
- 텍스처드 PEI 베드: `55°C`
- 첫 레이어 베드: `55°C`
- 팬 최소/최대: `100` / `100`
- 추가 쿨링 팬: `0`

## 복구용 프리셋 파일
- 프로세스: `종합_plate1-9_recovered_process_preset.json`
- 필라멘트: `종합_plate1-9_recovered_filament_preset.json`
- 전체 덤프: `종합_plate1-9_effective_project_settings.json`

## 주의
이 복구는 **클라우드 출력기록을 직접 복호화한 값이 아니라**, 프로젝트 파일 안에 저장된 슬라이서 스냅샷 기준이다. 그래서 출력 직전 체크박스(예: bed leveling / flow calibration / timelapse on/off)는 별도 보장되지 않는다.
