# Min Yujin · Backend Engineer

산업 안전 IoT 플랫폼(ProtectGO) 백엔드를 다룹니다. 단일 테넌트 NestJS 모놀리스를 **외부 고객사 단위 SaaS**로 전환하면서, **격리 · 실시간 정합성 · 운영 가시성** 세 축을 중심으로 BE 도메인 전반을 맡고 있어요.

```yaml
name:     Min Yujin (민유진)
role:     Backend Engineer @ IDB Lab
since:    2025.07 — present (~10 months)
domain:   Industrial Safety IoT · Realtime anomaly detection · Multi-tenant SaaS
focus:    Tenant isolation · Realtime consistency · Operational observability
email:    gnxm37@naver.com
```

---

## 📊 임팩트

<table align="center">
  <tr>
    <td align="center"><b>머지 PR</b></td>
    <td align="center"><b>기여 레포</b></td>
    <td align="center"><b>WS 격리</b></td>
    <td align="center"><b>변경 규모</b></td>
  </tr>
  <tr>
    <td align="center"><b>430</b><br>(446 중 96%)</td>
    <td align="center"><b>8</b><br>BE · Auth · Admin · Lib · Edge</td>
    <td align="center"><b>5 게이트웨이</b><br>tenant room 격리</td>
    <td align="center"><b>+111K LOC</b><br>2,700+ 파일</td>
  </tr>
</table>

---

## 🎯 대표 성과

- **외부 고객사 단위 멀티테넌시 전환 (DEL-686)** — HTTP / gRPC / MQTT / WebSocket 모든 진입점에 `TenantContext` 일관 적용, 5개 게이트웨이를 `tenant:${projectId}:*` room 키로 격리해 cross-tenant 누설 차단. **18+ PRs**
- **대시보드 실시간 파이프라인 개선** — emit 루프를 "위젯별 → 클라이언트별"에서 "클라이언트별 → 위젯 묶음"으로 뒤집고, `(type, chartId)` 단위 선집계로 같은 사용자 화면 동기화·중복 fetch 제거
- **차트 윈도우 정책 안정화** — TimeTrend / TimePlace 차트의 "카운트가 흐를수록 -1 되는" 회귀를 **KST 일 anchor → rolling N 시간 + 00:00 clamp** 4단계로 정착
- **DBMS 메타 트리 통합 API** — `databases-with-status`·`tables-with-status` 2종 → `tree` 단일 엔드포인트 통합. `graphable` 플래그로 FE 활성/비활성 분기를 BE 정책 한 곳(`isGraphableField`)으로 일원화
- **온보딩 가이드 상태 API (AUTH + BE)** — `/auth/me` 응답을 `User` → `userProject` 단위로 재구성, `PATCH` 신설, `/auth/me` 캐시 무효화까지 cross-repo 정리
- **엣지 디바이스 헬스 모니터링 PoC** — Prometheus + Grafana + Alertmanager + cAdvisor + jetson_stats_exporter, Slack 알림 연동

---

## 💡 일하는 방식

<table align="center">
  <tr>
    <td width="50%"><b>📊 데이터로 의사결정</b><br/>캐시 PR 3건을 머지하고도 "일관성 비용 > 캐시 이득"으로 데이터 기반 전면 revert. 차트 윈도우 정책도 4단계에 걸쳐 회귀를 데이터로 검증.</td>
    <td width="50%"><b>🔄 마이그레이션은 하위호환 후 제거</b><br/>room key · WS 이벤트 등 깨지는 변경은 신규 + 레거시 병행 → 검증 → 제거 4단계. 즉시 cut-over 금지.</td>
  </tr>
  <tr>
    <td><b>🧩 도메인 경계와 책임 분리</b><br/>`PlaceDetailRepository` junk drawer 해체, 메서드를 본래 도메인으로 이전. 모듈 의존성은 도메인 모듈 import로 명시.</td>
    <td><b>🔭 운영 가시성 먼저</b><br/>공용 로깅 라이브러리와 엣지 헬스 모니터링으로 "무슨 일이 벌어지는지"를 채널·대시보드로 노출. 현장 신고 이전에 인지.</td>
  </tr>
</table>

---

## 🛠️ Tech Stack

<table align="center">
  <tr>
    <td align="center" width="160"><b>Language</b></td>
    <td>
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=000000" />
      <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=FFD43B" />
    </td>
  </tr>
  <tr>
    <td align="center"><b>Framework</b></td>
    <td>
      <img src="https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white" />
      <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" />
      <img src="https://img.shields.io/badge/TypeORM-FE0803?style=for-the-badge&logo=typeorm&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td align="center"><b>Database · Storage</b></td>
    <td>
      <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
      <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
      <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
      <img src="https://img.shields.io/badge/MinIO-C72E49?style=for-the-badge&logo=minio&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td align="center"><b>Realtime · IoT</b></td>
    <td>
      <img src="https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socket.io&logoColor=white" />
      <img src="https://img.shields.io/badge/gRPC-244C5A?style=for-the-badge&logo=grpc&logoColor=white" />
      <img src="https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=eclipsemosquitto&logoColor=white" />
      <img src="https://img.shields.io/badge/AWS_IoT_Core-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td align="center"><b>Ops · Observability</b></td>
    <td>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
      <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white" />
      <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white" />
      <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
    </td>
  </tr>
</table>

---

## 📌 Now (2026.05)

- 🌳 **DBMS 실시간 패널 / 메타 트리 통합 API** — `with-status` 2종을 `tree` 단일 엔드포인트로, `graphable` 플래그로 FE 분기를 BE 한 곳에 일원화
- 🧭 **온보딩 가이드 상태 API (AUTH + BE)** — `/auth/me` 응답을 `userProject` 단위로 재구성, `PATCH` 신설
- 🎨 **차트 윈도우 정책 안정화** — KST 일 anchor + rolling N 시간 + 00:00 clamp 정착
- 🌐 배너 i18n + 인덱스 성능 개선

---

## 📊 GitHub Stats

<p align="center">
  <img height="180" src="https://streak-stats.demolab.com/?user=gnxm37&theme=tokyonight&hide_border=true&starting_year=2025" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/gnxm37/gnxm37/output/github-contribution-grid-snake-dark.svg" alt="snake" />
</p>

---

## 🔗 Connect

<p align="center">
  <a href="https://www.notion.so/35d0c3a6bfb581828afdd40c1e7784a3" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=notion&logoColor=white" alt="Portfolio" />
  </a>
  <a href="https://github.com/gnxm37" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <a href="mailto:gnxm37@naver.com" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/Naver_Mail-03C75A?style=for-the-badge&logo=naver&logoColor=white" alt="Email" />
  </a>
</p>
