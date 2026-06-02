# Min Yujin · Backend Engineer

산업 안전 IoT 플랫폼(ProtectGO) 백엔드. NestJS 기반 IoT 백엔드에서 **실시간 정합성 · 운영 가시성**을 중심으로 다룹니다.

```yaml
name:     Min Yujin (민유진)
role:     Backend Engineer @ IDB Lab
since:    2025.07 — present (~10 months)
domain:   Industrial Safety IoT · Realtime anomaly detection
focus:    Realtime consistency · Operational observability
email:    gnxm37@naver.com
```

---

## 📊 활동 영역

<table align="center">
  <tr>
    <td align="center"><b>기여 범위</b></td>
    <td align="center"><b>주력 도메인</b></td>
    <td align="center"><b>관심 영역</b></td>
  </tr>
  <tr>
    <td align="center"><b>백엔드 전반</b><br>BE · Auth · Admin · Lib · Edge</td>
    <td align="center"><b>IoT 실시간</b><br>이상탐지 · 대시보드</td>
    <td align="center"><b>운영 가시성</b><br>모니터링 · 로깅</td>
  </tr>
</table>

---

## 🎯 대표 성과

- **대시보드 실시간 파이프라인 재설계** — emit 루프를 클라이언트 단위로 뒤집어 중복 조회·카운트 오류 해결, 캐시는 측정 결과로 revert
- **AI 에이전트 배너 + place-detail 모듈** — 사내 AI 결과를 BE 응답에 통합(느린 LLM은 캐시로 가림), 장소 상세 모듈 신설로 도메인 경계 정리
- **문서 풀 CRUD + AI 임베딩** — 문서 업로드·저장(MinIO)부터 AI 임베딩 연동까지 백엔드를 처음부터 구축

## 💡 일하는 방식

- 📊 **데이터로 의사결정** — 머지된 캐시 PR도 측정 결과로 revert
- 🔄 **하위호환 후 제거** — 깨지는 변경은 신규+레거시 병행 → 검증 → 제거
- 🧩 **도메인 경계 분리** — junk drawer repository 해체, 모듈 의존성 명시화
- 🔭 **운영 가시성 먼저** — 공용 로깅 라이브러리, 엣지 헬스 모니터링 PoC

---

## 🛠️ Tech Stack

<table align="center">
  <tr>
    <td align="center" width="160"><b>Language</b></td>
    <td>
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=000000" />
    </td>
  </tr>
  <tr>
    <td align="center"><b>Backend</b></td>
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

## 📌 Now (2026.06)

- 🌳 DBMS 실시간 패널 / 메타 트리 통합 API
- 🧭 온보딩 가이드 상태 API (AUTH + BE)
- 🎨 차트 윈도우 정책 안정화
- 🌐 배너 i18n + 인덱스 성능 개선

---

<p align="center">
  <img src="https://raw.githubusercontent.com/gnxm37/gnxm37/output/github-contribution-grid-snake-dark.svg" alt="snake" />
</p>

> 📓 프로젝트별 배경·의사결정 근거·PR 링크는 [노션 포트폴리오](https://www.notion.so/35d0c3a6bfb581828afdd40c1e7784a3)에서 확인하실 수 있습니다.

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
