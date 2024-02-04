# IQ² (IQ square) 설치 가이드

## 설치 프로세스

IQ²의 설치는 명확하고 단계별로 진행됩니다. 각 구성 요소의 상세 설치 가이드를 따라 설치를 완료할 수 있습니다:

### 1. Controller 설치

Controller는 IQ²의 핵심 요소로, 트래픽 제어 정책을 관리합니다.

- 상세 설치 가이드: [`controller/README.md`](controller/README.md)

### 2. Scouter 설치

Scouter는 서버의 실시간 상태를 모니터링하고, Controller에 중요 정보를 전달합니다.

- 상세 설치 가이드: [`scouter/README.md`](scouter/README.md)

### 3. Connector 설치

Connector는 Controller의 지침에 따라 실제 트래픽을 제어합니다. 사용 환경에 맞는 Connector를 선택하여 설치합니다.

- **NGINX용 Connector**
    - 상세 설치 가이드: [`connector/nginx/README.md`](connector/nginx/README.md)
- **CA Layer7 API Gateway용 Connector**
    - 상세 설치 가이드: [`connector/ca-layer7-api-gateway/README.md`](connector/ca-layer7-api-gateway/README.md)

추가 Connector 설치 가이드는 [`connector/README.md`](connector/README.md) 에서 확인할 수 있습니다.

---

IQ²를 선택해 주셔서 감사합니다. 설치 과정에서 질문이나 필요한 지원이 있으시면 언제든지 [이슈 트래커](#)를 통해 문의해 주세요.
