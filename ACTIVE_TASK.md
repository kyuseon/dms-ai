# ACTIVE TASK: 중기 과제 목록

## ImageServer 중기 개선 과제

### Phase 3 — 코드 품질

| # | 이슈 | 수정 내용 |
|---|------|-----------|
| M1 | 매직 넘버 | `constexpr` 상수로 추출 (`HASH_HEX_LEN`, `TIMESTAMP_LEN` 등) |
| M2 | 에러 처리 정책 혼재 | null 파라미터 → 예외, "미발견" → false, I/O 실패 → 예외 로 통일 |
| M3 | `addImage` 73줄 | 내부 헬퍼 메서드로 분리 |

### Adversarial Review 잔류 항목

| # | 위치 | 이슈 | 비고 |
|---|------|------|------|
| A3 | `FileBlobStorage.cpp:125` | `ext` 미검증 → 경로 주입 가능 | 운영 재량으로 보류 |
| B1 | `unlink` 상대경로 의존 | 프로세스 CWD 고정 운영 시 실질 위험 낮음 | |
| B2 | `getImageItem()` O(N) 풀 스캔 | 추후 SQLite 또는 carrierId 기반 hashmap 전환 | |
| B3 | `findByHashInternal()` thundering herd | 단일 인스턴스 구조에서 즉각 위험 없음 | |
