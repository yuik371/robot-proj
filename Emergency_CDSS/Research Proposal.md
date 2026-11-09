# 골든타임 응급대응 소셜 로봇 연구제안서
연구 책임자: 오염덕 & 연구원: 유익
## 1. 연구의 요약 및 핵심 주장(Executive Summary)
본 연구 과제의 핵심 가치는 의학적 "진단(Diagonosis)"이 아니라, 급성 응급 발생 시 발견-신고-초동 지시까지 발생하는 3대 치명적 지연 시간, 즉 '인식 지연(Time-to-Recognition)', '출동 지연(Time-to-Dispatch)', '초동 압박 지연(Time-to-First-Compression)'을 최소화하는 것에 있다. 이 세 구간은 심정지 및 뇌졸중 환자의 생존율을 결정짓는 골든타임 손실의 대부분을 차지하며, 물리적·의학적 처치를 직접 수행할 수 없는 '비접촉 데스크톱 소셜 로봇'이 개입하여 사회적 기여를 할 수 있는 유일하고도 가장 효과적인 오퍼레이션 구간이다.

본 연구는 로봇의 역할을 고비용의 전문 진단 기기가 아닌, **"현장 밀착형 트리아지(Triage) 보조 및 119 디스패처 연장 단말(Dispatcher-Assisted CPR On-Scene Terminal)"**로 명확히 포징한다. 이러한 접근법은 기술적 실현 가능성을 극대화할 뿐만 아니라, 의료기기 인허가 장벽을 영리하게 우회하는 전략적 기반이 된다.
## 2. 대상 사건 및 시스템 사양 (Target Events & System Specifications)
2.1 대상 사건 (Target Emergency Events)
- 급성 허탈 (Acute Collapse): 심정지가 의심되는 급작스러운 쓰러짐 및 움직임 소실.
뇌졸중 의심 징후 (Acute Stroke Indicators): 안면 및 편측 마비(Hemiplegia), 구음장애(Dysarthria), 비대칭적 낙상 패턴.
의식 소실을 동반한 중증 낙상 (Traumatic Fall with Loss of Consciousness).

2.2 하드웨어 플랫폼 전제 및 사양 (Platform Constraints)
본 연구는 고전력·고비용의 맞춤형 로봇을 배제하고, 코딩 교육용 로봇(누아로보틱스 케비로봇)의 사양을 basekube으로 전제한다.
![alt text](image-1.png)
- 센서 풋프린트: RGB 비전 카메라, 마이크 어레이(Microphone Array), PIR(인체감지) 센서, IR(적외선) 낙하 감지 센서, 정전식 터치 센서.
- 액추에이터 및 I/O: 7인치 터치 디스플레이, 다축 상지 관절 모듈(Expressive Upper Limbs), 듀얼 스피커, 상태 표시형 LED 인디케이터.
- 기능적 경계: 환자에 대한 직접적인 물리적 처치(Mechanical Intervention) 기능은 포함하지 않음.