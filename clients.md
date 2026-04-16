### . CTD 문서 구조

- CTD는 모듈 1~5로 구성 → **모듈 2 & 3 우선 적용**
- 원료 의약품 7개 항목 / 완제 의약품 8개 항목 각각 별도 파일 생성
- 내용 대부분은 내부 시스템에 저장된 Word/Excel 파일에서 추출한 표와 텍스트
- 일부 문서에는 그래프·이미지 포함 → 해석 없이 **정확한 선택 및 배치**만 필요
- CTD 파일 한 건당 **79~500페이지 이상**

---

### 2. CTD vs PQR 차이점

| 구분 | CTD | PQR |
| --- | --- | --- |
| **작성 빈도** | 연간 약 7건 | 연간 약 100건 |
| **건당 소요시간** | 약 320시간 | 약 7시간 |
| **버전 관리** | ✅ 있음 | ❌ 없음 |
| **업데이트 시점** | 제조 변경 발생 시 (배치 사이즈, 원료 공급업체, 설비 등) | 매년 1회 |

변경 사항은 보통 **2~3건씩 묶어서** 식약처에 제출 (심사 기간 1~6개월 소요)

---

### 3. 자동화 가능성

- 문서 작성 프로세스 자체는 **자동화 가능**으로 판단
- 변경 트리거는 항상 **사람이 직접 판단**하여 입력
- 그래프·이미지는 제목이 잘 정리되어 있어 → **해석 없이 선택 로직 구현 가능**
- **검증 모듈** 필요 — 자동 생성 결과를 현업 담당자가 검토하는 구조 원함
- 의약품 규제 산업 특성상 **높은 정확도 필수** (80% 수준으로는 불충분)

---

### 4. 필요 데이터 및 샘플

- **JW 제공 예정:** 원천 데이터 샘플, SOP, 완성된 CTD 예시 (최초 등록본 + 부분 변경본)
- **콕스웨이브 요청:** 제조처별 원천 데이터 형식 차이가 클 경우 → 다양한 샘플 추가 필요

---

### 🔗 Reference Docs

---

## CTD vs PQR???

### CTD — (Common Technical Document)

> CTD는 **제품 여권**이라고 생각하면 됩니다. 의약품을 판매하기 위한 정부 승인을 받고, 이후 변경 사항이 생길 때마다 승인을 유지하기 위해 제출하는 핵심 문서입니다.
> 

| 항목 | 내용 |
| --- | --- |
| **포함 내용** | 성분, 제조 공정, 설비, 시험 결과, 안정성 데이터, 공급업체 정보 |
| **작성 시점** | 최초 허가 등록 시 — 이후 변경 사항 발생 시마다 업데이트 (신규 공급업체, 배치 사이즈, 설비 변경 등) |
| **사용 주체** | 규제 기관 제출용 (식품의약품안전처). 내부적으로는 RA(허가) 부서에서 관리 |
| **규모 및 건수** | 79–500페이지 이상 · 연간 약 7건 · 건당 약 320시간 소요 |
| **구조** | 모듈 1–5 · 핵심: 모듈 2 (요약) & 모듈 3 (세부 기술 데이터) · 원료 의약품 7개 항목 · 완제 의약품 8개 항목 |
| **버전 관리** | ✅ 있음 — 버전 관리 적용. 변경 사항은 2–3건씩 묶어서 제출 (심사 기간 1–6개월 소요) |

**필요 입력 파일:**

- 제조지시기록서
- 제품표준서
- 성적서 (CoA)
- 원자재 및 완제품 시험규격서
- PV / SPV 보고서
- DMF (원료 제조원 자료)
- 그래프 및 흐름도 (워드 파일 내 이미지)

---

### PQR — (Product Quality Review)

> PQR은 **연간 건강검진**이라고 생각하면 됩니다. 각 의약품이 지난 12개월 동안 어떻게 생산·관리되었는지를 돌아보는 연간 보고서입니다.
> 

| 항목 | 내용 |
| --- | --- |
| **포함 내용** | 연간 배치 요약, 시험 결과, 일탈, 불만, 변경 사항, CAPA 조치, 안정성 데이터 |
| **작성 시점** | 제품별 연 1회 — 매년 새로 작성하는 단독 문서 |
| **사용 주체** | 내부 QA/QC 팀의 품질 모니터링용. 규제 기관 실사 시 검토 대상 |
| **규모 및 건수** | 약 40페이지 · 연간 약 100건 · 건당 약 7시간 소요 |
| **구조** | 배치 요약 → 시험 결과 → 일탈 → 변경 관리 → 불만 → CAPA 목록 → 안정성 업데이트 |
| **버전 관리** | ❌ 없음 — 매년 신규 문서 작성, 이전 버전 이월 없음 |

**필요 입력 파일:**

- EMR 제조기록
- LIMS 시험 결과
- WMS 입고 정보
- 엑셀 그래프 및 통계 데이터
- 일탈 / CAPA 목록
- 허가 이력

---

#### CTD vs PQR 비교

|  | **CTD** | **PQR** |
| --- | --- | --- |
| **목적** | 제품 허가 등록 및 변경 관리 | 연간 품질 검토 |
| **작성 시점** | 최초 등록 또는 변경 발생 시 | 매년 1회 정기 작성 |
| **연간 건수** | 약 7건 | 약 100건 |
| **건당 소요 시간** | 약 320시간 | 약 7시간 |
| **페이지 수** | 79–500페이지 이상 | 약 40페이지 |
| **버전 관리** | ✅ 있음 — 지속 업데이트 | ❌ 없음 — 매년 신규 작성 |
| **제출 대상** | 외부 규제 기관 (식약처) | 내부 QA/QC 팀 |
| **복잡도** | 높음 — 다중 출처, 버전 관리 필요 | 중간 — 정형화된 연간 보고 |

---

### **Input Files (Source Data)**

| File | Type | Description |
| --- | --- | --- |
| Manufacturing records (제조지시기록서) | Word / System export | Step-by-step manufacturing instructions per product |
| Product standards (제품표준서) | Word | Product specifications and standards |
| CoA (Certificate of Analysis) | Word / PDF | Quality test results from manufacturer |
| Raw material & finished product test specs (시험규격서) | Word | Testing criteria for ingredients and final product |
| PV / SPV reports | Word | Process validation reports |
| DMF (Drug Master File) | Word / PDF | Raw material manufacturer's confidential technical data |
| EMR manufacturing records | System export (Excel/CSV) | Electronic manufacturing records |
| LIMS test results | System export (Excel/CSV) | Lab test results from internal system |
| WMS receiving info | System export (Excel/CSV) | Warehouse/incoming material records |
| Graphs & flow diagrams | Images (embedded in Word) | Process flow charts, experimental result graphs |

---

### **Output Files (What Gets Generated)**

| File | Type | Description |
| --- | --- | --- |
| CTD Module 2 & 3 | Word (multi-hundred pages) | Regulatory submission document — full technical package |
| PQR Report | Word / Excel | Annual product quality review, ~40 pages |

---

**Key Takeaway on Complexity**

- Most inputs are **Word or Excel files** pulled from internal systems
- The hard part is that **formats vary by manufacturer** — same type of data, different layouts
- Images/graphs are **embedded inside Word files** and need to be selectively extracted, not interpreted
- CTD outputs need **version control** (updated when manufacturing changes); PQR does not

### ✅ Tasks

---

| 액션 | 담당 | 일정 |
| --- | --- | --- |
| CTD 샘플 파일 + 원천 데이터 공유 | JW | 최대한 빨리 (당일~익일) |
| 지원 사업 제안서 작성 및 제출 | 콕스웨이브 | 다음 주 |
| 제안서 피드백 요청 | 콕스웨이브 | 초안 완성 후 |
| 솔루션 배포 및 연동 체크리스트 준비 | 콕스웨이브 | 5월 이전 |
| 데이터 교환 + 연동 가능성 검토 | 양측 공동 | 5월 중 |

지원 사업 마감은 **다음 주**, PoC는 예산 편성을 위해 **6월 이내** 착수 목표,
5월은 **데이터 전달 및 환경 세팅** 단계로 활용 예정.
