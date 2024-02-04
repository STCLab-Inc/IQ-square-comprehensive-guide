# IQ² (IQ Square) 설치 가이드

## 소개

IQ² (IQ Square)는 서버의 실시간 상태를 반영하여 트래픽을 최적화하는 혁신적인 솔루션입니다. 이는 리소스 과부하를 방지하고, 우선순위에 따라 트래픽을 효율적으로 처리하며, 모든 서버 메트릭과 라우팅 통계를 통합적으로 모니터링하여 서비스의 연속성과 품질을 보장합니다.

## 주요 구성 요소

IQ²는 다음과 같은 세 가지 핵심 구성 요소로 구성되어 있습니다:

- **Controller**: 트래픽 제어 정책을 결정하고 Connector에 실행 지침을 전달합니다.
- **Connector**: Controller의 지침에 따라 실제 트래픽 제어를 담당합니다.
- **Scouter**: 서버의 실시간 상태를 모니터링하고 Controller에 중요 정보를 보고합니다.

## 설치 프로세스

IQ²의 설치는 명확하고 단계별로 진행됩니다. 각 구성 요소의 상세 설치 가이드를 따라 설치를 완료할 수 있습니다:

### 1. Controller 설치

Controller는 IQ²의 핵심 요소로, 트래픽 제어 정책을 관리합니다.

- 상세 설치 가이드: [`installation/controller/README.md`](installation/controller/README.md)

### 2. Scouter 설치

Scouter는 서버의 실시간 상태를 모니터링하고, Controller에 중요 정보를 전달합니다.

- 상세 설치 가이드: [`installation/scouter/README.md`](installation/scouter/README.md)

### 3. Connector 설치

Connector는 Controller의 지침에 따라 실제 트래픽을 제어합니다. 사용 환경에 맞는 Connector를 선택하여 설치합니다.

- **NGINX용 Connector**
    - 상세 설치 가이드: [`installation/connector/NGINX/README.md`](installation/connector/NGINX/README.md)
- **CA Layer7 API Gateway용 Connector**
    - 상세 설치 가이드: [`installation/connector/CA Layer7 API Gateway/README.md`](installation/connector/CA%20Layer7%20API%20Gateway/README.md)

추가 Connector 설치 가이드는 [`installation/connector/README.md`](installation/connector/README.md) 에서 확인할 수 있습니다.

---

IQ²를 선택해 주셔서 감사합니다. 설치 과정에서 질문이나 필요한 지원이 있으시면 언제든지 [이슈 트래커](#)를 통해 문의해 주세요.
