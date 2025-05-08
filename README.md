### Q1
한 회사에서 컨테이너화된 애플리케이션 워크로드를 3개의 가용 영역에 걸쳐 VPC에 배포하려고 합니다. 회사에는 가용 영역 전반에 걸쳐 가용성이 높은 솔루션이 필요합니다. 솔루션을 사용 하려면 애플리케이션을 최소한으로 변경해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Elastic Container Service(Amazon ECS)를 사용하세요. 대상 추적 조정을 사용하도록 Amazon ECS 서비스 Auto Scaling을 구성합니다. 최소 용량을 3으로 설정합
니다. 가용 영역 속성을 사용하여 분산되도록 작업 배치 전략 유형을 설정합니다.
B. Amazon Elastic Kubernetes Service(Amazon EKS) 자체 관리형 노드를 사용합니다. 대상 추적 조정을 사용하도록 Application Auto Scaling을 구성합니다. 최소 용량을 3으
로 설정하세요.
C. Amazon EC2 예약 인스턴스를 사용하십시오. 분산 배치 그룹에서 3개의 EC2 인스턴스를 시작합니다. 대상 추적 조정을 사용하도록 Auto Scaling 그룹을 구성합니다. 최소 용량을 3
으로 설정하세요.
D. AWS Lambda 함수를 사용하십시오. VPC에 연결하도록 Lambda 함수를 구성합니다. Lambda를 확장 가능한 대상으로 사용하도록 Application Auto Scaling을 구성합니다. 최
소 용량을 3으로 설정하세요.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q2
한 회사가 프로덕션 Amazon Elastic Kubernetes Service(Amazon EKS) 클러스터에서 실행될 애플리케이션을 개발하고 있습니다. EKS 클러스터에는 온디맨드 인스턴스로 프로비저 닝되는 관리형 노드 그룹이 있습니다. 회사에는 개발 작업을 위한 전용 EKS 클러스터가 필요합니다. 회사는 애플리케이션의 복원력을 테스트하기 위해 개발 클러스터를 자주 사용하지 않습니다. EKS 클러스터는 모든 노드를 관 리해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 스팟 인스턴스만 포함하는 관리형 노드 그룹을 생성합니다.
B. 두 개의 관리형 노드 그룹을 생성합니다. 온디맨드 인스턴스로 하나의 노드 그룹을 프로비저닝합니다. 스팟 인스턴스로 두 번째 노드 그룹을 프로비저닝합니다.
C. 스팟 인스턴스를 사용하는 시작 구성이 있는 Auto Scaling 그룹을 생성합니다. EKS 클러스터에 노드를 추가하도록 사용자 데이터를 구성합니다.
D. 온디맨드 인스턴스만 포함하는 관리형 노드 그룹을 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q3
한 회사의 온프레미스 데이터 센터에 소량의 데이터를 Amazon S3에 정기적으로 백업해야 하는 NFS 서버가 있습니다. 이러한 요구 사항을 충족하고 가장 비용 효율적인 솔루션은 무엇입니 까?
A. 온프레미스 서버의 데이터를 Amazon S3에 복사하도록 AWS Glue를 설정합니다.
B. 온프레미스 서버에 AWS DataSync 에이전트를 설정하고 데이터를 Amazon S3에 동기화합니다.
C. AWS Transfer for SFTP를 사용하여 SFTP 동기화를 설정하여 온프레미스에서 Amazon S3로 데이터를 동기화합니다.
D. 온프레미스 데이터 센터와 VPC 간에 AWS Direct Connect 연결을 설정하고 데이터를 Amazon S3에 복사합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q4
회사에서 Amazon Elastic Container Service(Amazon ECS)를 사용할 컨테이너화된 애플리케이션을 설계하고 있습니다. 애플리케이션은 내구성이 뛰어나고 RPO(복구 지점 목표)가 8시간인 다른 AWS 리전에 데이터를 복구할 수 있는 공유 파일 시스템에 액세스해야 합니다. 파일 시스템은 리전 내의 각 가용 영역에 탑재 대상을 제공해야 합니다. 솔루션 설계자는 AWS Backup을 사용하여 다른 리전에 대한 복제를 관리하려고 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 다중 AZ 배포가 있는 Windows 파일 서버용 Amazon FSx 
B. 다중 AZ 배포가 있는 NetApp ONTAP용 Amazon FSx 
C. 표준 스토리지 클래스가 있는 Amazon Elastic File System(Amazon EFS) 
D. OpenZFS용 Amazon FSx

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q5
회사는 민감한 사용자 정보를 Amazon S3 버킷에 저장하고 있습니다. 회사는 VPC 내부의 Amazon EC2 인스턴스에서 실행되는 애플리케이션 계층에서 이 버킷에 대한 보안 액세스를 제 공하려고 합니다. 이를 달성하기 위해 솔루션 설계자가 수행해야 하는 단계 조합은 무엇입니까? (두 가지를 선택하세요.)
A. VPC 내에서 Amazon S3에 대한 VPC 게이트웨이 엔드포인트를 구성합니다. 
B. 버킷 정책을 생성하여 S3 버킷의 객체를 공개합니다. 
C. VPC에서 실행되는 애플리케이션 계층으로만 액세스를 제한하는 버킷 정책을 만듭니다. 
D. S3 액세스 정책으로 IAM 사용자를 생성하고 IAM 자격 증명을 EC2 인스턴스에 복사합니다. 
E. NAT 인스턴스를 생성하고 EC2 인스턴스가 NAT 인스턴스를 사용하여 S3 버킷에 액세스하도록 합니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q6
회사는 AWS Organizations 설정을 사용하여 다양한 애플리케이션이 포함된 여러 AWS 계정을 관리합니다. 그들은 조직 내에 전용 모니터링 회원 계정을 설정했습니다. 이 회사는 Amazon CloudWatch를 사용하여 이러한 계정 전체의 관측 가능성 데이터에 액세스하고 시각화하는 것을 목표로 합니다. 이러한 요구 사항에 가장 적합한 솔루션은 무엇입니까?
A. 모니터링 계정에 대해 CloudWatch 교차 계정 관찰 기능을 활성화합니다. 모니터링 계정에서 제공하는 AWS CloudFormation 템플릿을 각 AWS 계정에 배포하여 모니터링 계정과
데이터를 공유합니다.
B. 조직의 루트 조직 단위(OU) 아래 모니터링 계정에서 CloudWatch에 대한 액세스 권한을 부여하도록 서비스 제어 정책(SCP)을 설정합니다. 
C. 모니터링 계정에 새 IAM 사용자를 구성합니다. 각 AWS 계정에서 CloudWatch 데이터 쿼리 및 시각화를 허용하는 IAM 정책을 설정합니다. 이 새 IAM 정책을 새 IAM 사용자에게 연
결합니다.
D. 모니터링 계정에 새 IAM 사용자를 생성합니다. 각 AWS 계정에 교차 계정 IAM 정책을 설정합니다. 이러한 IAM 정책을 새 IAM 사용자에게 연결합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q7
회사에서 웹 애플리케이션으로 새로운 비디오 게임을 개발했습니다. 애플리케이션은 데이터베이스 계층에 MySQL용 Amazon RDS가 있는 VPC의 3계층 아키텍처에 있습니다. 여러 플레 이어가 온라인에서 동시에 경쟁합니다. 게임 개발자는 거의 실시간으로 상위 10개 점수판을 표시하고 현재 점수를 유지하면서 게임을 중지하고 복원할 수 있는 기능을 제공하기를 원합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 웹 애플리케이션이 표시할 점수를 캐시하도록 Memcached 클러스터용 Amazon ElastiCache를 설정합니다. 
B. Redis 클러스터용 Amazon ElastiCache를 설정하여 웹 애플리케이션이 표시할 점수를 계산하고 캐시합니다. 
C. 웹 애플리케이션 앞에 Amazon CloudFront 배포를 배치하여 애플리케이션 섹션의 점수판을 캐시합니다. 
D. MySQL용 Amazon RDS에서 읽기 전용 복제본을 생성하여 스코어보드를 계산하고 웹 애플리케이션에 읽기 트래픽을 제공하는 쿼리를 실행합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q8
한 회사에서 역사적 사건의 이미지를 저장하는 웹사이트를 운영하고 있습니다. 웹사이트 사용자는 이미지 속 사건이 발생한 연도를 기준으로 이미지를 검색하고 볼 수 있는 기능이 필요합니다. 평균적으로 사용자는 각 이미지를 1년에 한두 번만 요청합니다. 회사는 이미지를 저장하고 사용자에게 전달할 수 있는 가용성이 뛰어난 솔루션을 원합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. Amazon Elastic Block Store(Amazon EBS)에 이미지를 저장합니다. Amazon EC2에서 실행되는 웹 서버를 사용하십시오.
B. Amazon Elastic File System(Amazon EFS)에 이미지를 저장합니다. Amazon EC2에서 실행되는 웹 서버를 사용하십시오.
C. Amazon S3 Standard에 이미지를 저장합니다. S3 Standard를 사용하면 정적 웹 사이트를 통해 이미지를 직접 전달할 수 있습니다.
D. Amazon S3 Standard-Infrequent Access(S3 Standard-IA)에 이미지를 저장합니다. S3 Standard-IA를 사용하면 정적 웹 사이트를 통해 이미지를 직접 전달할 수 있습니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q9
회사에 수신 메시지를 수집하는 애플리케이션이 있습니다. 그러면 수십 개의 다른 애플리케이션과 마이크로서비스가 이러한 메시지를 빠르게 사용합니다. 메시지 수는 매우 다양하며 때로는 초 당 100,000개로 갑자기 증가하기도 합니다. 회사는 솔루션을 분리하고 확장성을 높이고자 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon Kinesis Data Analytics에 대한 메시지를 유지합니다. 메시지를 읽고 처리하도록 소비자 애플리케이션을 구성합니다.
B. Auto Scaling 그룹의 Amazon EC2 인스턴스에 수집 애플리케이션을 배포하여 CPU 지표를 기반으로 EC2 인스턴스 수를 확장합니다.
C. 단일 샤드로 Amazon Kinesis Data Streams에 메시지를 씁니다. AWS Lambda 함수를 사용하여 메시지를 사전 처리하고 Amazon DynamoDB에 저장합니다. 메시지를 처리하
기 위해 DynamoDB에서 읽을 소비자 애플리케이션을 구성합니다.
D. 여러 Amazon Simple Queue Service(Amazon SQS) 구독이 있는 Amazon Simple Notification Service(Amazon SNS) 주제에 메시지를 게시합니다. 대기열의 메시지를
처리하도록 소비자 애플리케이션을 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q10
회사는 온프레미스에서 실행되는 Windows 파일 서버에 5TB 이상의 파일 데이터를 보유하고 있습니다. 사용자와 애플리케이션은 매일 데이터와 상호 작용합니다. 이 회사는 Windows 워크로드를 AWS로 이전하고 있습니다. 회사가 이 프로세스를 계속 진행함에 따라 회사는 최소한의 대기 시간으로 AWS 및 온프레미스 파일 스토리지에 액세스해야 합 니다. 회사는 운영 오버헤드를 최소화하고 기존 파일 액세스 패턴을 크게 변경할 필요가 없는 솔루션이 필요합니다. 이 회사는 AWS에 연결하기 위해 AWS Site-to-Site VPN 연결을 사용 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS에서 Windows File Server용 Amazon FSx를 배포하고 구성합니다. 온프레미스 파일 데이터를 FSx for Windows File Server로 이동합니다. AWS에서 Windows File
Server용 FSx를 사용하도록 워크로드를 재구성합니다.
B. 온프레미스에 Amazon S3 파일 게이트웨이를 배포하고 구성합니다. 온프레미스 파일 데이터를 S3 파일 게이트웨이로 이동합니다. S3 파일 게이트웨이를 사용하도록 온프레미스 워크
로드 및 클라우드 워크로드를 재구성합니다.
C. 온프레미스에 Amazon S3 파일 게이트웨이를 배포하고 구성합니다. 온프레미스 파일 데이터를 Amazon S3로 이동합니다. Amazon S3를 직접 사용하거나 S3 파일 게이트웨이를 사
용하도록 워크로드를 재구성합니다. 각 워크로드의 위치에 따라 다릅니다.
D. AWS에서 Windows 파일 서버용 Amazon FSx를 배포하고 구성합니다. 온프레미스에 Amazon FSx 파일 게이트웨이를 배포하고 구성합니다. 온프레미스 파일 데이터를 FSx 파일
게이트웨이로 이동합니다. AWS에서 Windows File Server용 FSx를 사용하도록 클라우드 워크로드를 구성합니다. FSx 파일 게이트웨이를 사용하도록 온프레미스 워크로드를 구성 합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q11
회사에서 분산 애플리케이션을 AWS로 마이그레이션하고 있습니다. 이 애플리케이션은 다양한 워크로드를 처리합니다. 레거시 플랫폼은 여러 컴퓨팅 노드에서 작업을 조정하는 기본 서버로 구성됩니다. 회사는 복원력과 확장성을 최대화하는 솔루션으로 애플리케이션을 현대화하려고 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 아키텍처를 어떻게 설계해야 합니까?
A. 작업의 대상으로 Amazon Simple Queue Service(Amazon SQS) 대기열을 구성합니다. Auto Scaling 그룹에서 관리되는 Amazon EC2 인스턴스로 컴퓨팅 노드를 구현합니다
. 예약된 조정을 사용하도록 EC2 Auto Scaling을 구성합니다.
B. 작업의 대상으로 Amazon Simple Queue Service(Amazon SQS) 대기열을 구성합니다. Auto Scaling 그룹에서 관리되는 Amazon EC2 인스턴스로 컴퓨팅 노드를 구현합니다
. 대기열 크기에 따라 EC2 Auto Scaling을 구성합니다.
C. Auto Scaling 그룹에서 관리되는 Amazon EC2 인스턴스로 기본 서버 및 컴퓨팅 노드를 구현합니다. 작업의 대상으로 AWS CloudTrail을 구성합니다. 기본 서버의 로드를 기반으로
EC2 Auto Scaling을 구성합니다.
D. Auto Scaling 그룹에서 관리되는 Amazon EC2 인스턴스로 기본 서버 및 컴퓨팅 노드를 구현합니다. 작업의 대상으로 Amazon EventBridge(Amazon CloudWatch Events)
를 구성합니다. 컴퓨팅 노드의 로드를 기반으로 EC2 Auto Scaling을 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q12
솔루션 설계자는 보안 그룹이 0.0.0.0/0 의 SSH를 허용하는 규칙을 포함할 수 없다고 명시하는 회사의 규정 준수 정책에 대한 자동화된 솔루션을 제공해야 합니다 . 정책을 위반한 경우 회사 에 통보해야 합니다. 가능한 한 빨리 해결책이 필요합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 0.0.0.0/0 주소에 열려 있는 SSH에 대한 보안 그룹을 모니터링하고 이를 발견할 때마다 알림을 생성하는 AWS Lambda 스크립트를 작성하십시오.
B. 제한된 SSH AWS Config 관리형 규칙을 활성화하고 비준수 규칙이 생성되면 Amazon Simple 알림 서비스(Amazon SNS) 알림을 생성합니다.
C. 전 세계적으로 보안 그룹 및 네트워크 ACL을 열 수 있는 권한이 있는 IAM 역할을 생성합니다. 사용자가 역할을 맡을 때마다 알림을 생성하려면 Amazon Simple 알림 서비스
(Amazon SNS) 주제를 생성합니다.
D. 관리자가 아닌 사용자가 보안 그룹을 생성하거나 편집하는 것을 방지하는 서비스 제어 정책(SCP)을 구성합니다. 사용자가 관리자 권한이 필요한 규칙을 요청할 때 티켓팅 시스템에 알림
을 만듭니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q13
내장형 NoSQL 데이터베이스가 포함된 회사의 웹 애플리케이션은 ALB(Application Load Balancer) 뒤의 Amazon EC2 인스턴스에서 작동합니다. 이러한 인스턴스는 단일 가용 영역 으로 제한된 Amazon EC2 Auto Scaling 그룹 내에 있습니다. 트래픽 증가로 인해 애플리케이션은 고가용성을 달성해야 하며 데이터베이스는 최종 일관성을 유지해야 합니다. 이러한 요구 사항을 충족하면서 운영 오버헤드를 최소화하는 솔루션은 무엇입니까?
A. ALB를 Network Load Balancer로 교체하고 내장형 NoSQL 데이터베이스를 EC2 인스턴스의 복제 서비스와 함께 유지합니다. 
B. ALB를 Network Load Balancer로 교체하고 AWS Database Migration Service(AWS DMS)를 사용하여 내장형 NoSQL 데이터베이스를 Amazon DynamoDB로 마이그
레이션합니다.
C. EC2 인스턴스의 복제 서비스와 함께 내장된 NoSQL 데이터베이스를 유지하면서 3개의 가용 영역에서 EC2 인스턴스를 활용하도록 Auto Scaling 그룹을 수정합니다. 
D. 3개의 가용 영역에서 EC2 인스턴스를 활용하고 AWS Database Migration Service(AWS DMS)를 사용하여 내장된 NoSQL 데이터베이스를 Amazon DynamoDB로 마이그
레이션하도록 Auto Scaling 그룹을 수정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q14
회사에서 응용 프로그램의 안정적인 아키텍처를 설계하기 위해 솔루션 설계자를 고용했습니다. 이 애플리케이션은 웹 서버를 실행하는 Amazon RDS DB 인스턴스 1개와 수동으로 프로비저 닝된 Amazon EC2 인스턴스 2개로 구성됩니다. EC2 인스턴스는 단일 가용 영역에 있습니다. 직원이 최근 DB 인스턴스를 삭제했고 그 결과 애플리케이션을 24시간 동안 사용할 수 없었습니다. 회사는 환경의 전반적인 안정성에 관심이 있습니다. 애플리케이션 인프라의 안정성을 극대화하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. 하나의 EC2 인스턴스를 삭제하고 다른 EC2 인스턴스에서 종료 방지 기능을 활성화하십시오. 다중 AZ가 되도록 DB 인스턴스를 업데이트하고 삭제 방지를 활성화합니다. 
B. DB 인스턴스를 다중 AZ로 업데이트하고 삭제 방지를 활성화합니다. Application Load Balancer 뒤에 EC2 인스턴스를 배치하고 여러 가용 영역에 걸쳐 EC2 Auto Scaling 그룹에
서 실행합니다.
C. Amazon API Gateway 및 AWS Lambda 함수와 함께 추가 DB 인스턴스를 생성합니다. API Gateway를 통해 Lambda 함수를 호출하도록 애플리케이션을 구성합니다.
Lambda 함수가 두 DB 인스턴스에 데이터를 쓰도록 합니다.
D. 여러 가용 영역에 여러 서브넷이 있는 EC2 Auto Scaling 그룹에 EC2 인스턴스를 배치합니다. 온디맨드 인스턴스 대신 스팟 인스턴스를 사용하십시오. 인스턴스의 상태를 모니터링하
도록 Amazon CloudWatch 경보를 설정합니다. DB 인스턴스를 다중 AZ로 업데이트하고 삭제 방지를 활성화합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q15
AWS를 사용하는 회사에는 매달 제조 프로세스에 필요한 리소스를 예측하는 솔루션이 필요합니다. 솔루션은 현재 Amazon S3 버킷에 저장된 기록 값을 사용해야 합니다. 회사는 기계 학습 (ML) 경험이 없으며 교육 및 예측에 관리형 서비스를 사용하려고 합니다. 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (2개를 선택하세요.)
A. Amazon SageMaker 모델을 배포합니다. 추론을 위해 SageMaker 엔드포인트를 생성합니다. 
B. Amazon SageMaker를 사용하여 S3 버킷의 기록 데이터를 사용하여 모델을 교육합니다. 
C. Amazon SageMaker 엔드포인트를 사용하여 입력을 기반으로 예측을 생성하는 함수 URL로 AWS Lambda 함수를 구성합니다. 
D. Amazon Forecast 예측기를 사용하여 입력을 기반으로 예측을 생성하는 함수 URL로 AWS Lambda 함수를 구성합니다. 
E. S3 버킷의 기록 데이터를 사용하여 Amazon Forecast 예측기를 교육합니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q16
한 회사에서 다중 계층 애플리케이션을 온프레미스에서 AWS 클라우드로 이동하여 애플리케이션의 성능을 개선하려고 합니다. 애플리케이션은 RESTful 서비스를 통해 서로 통신하는 애플 리케이션 계층으로 구성됩니다. 한 계층이 과부하되면 트랜잭션이 삭제됩니다. 솔루션 설계자는 이러한 문제를 해결하고 애플리케이션을 현대화하는 솔루션을 설계해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족하고 운영상 가장 효율적입니까?
A. Amazon API Gateway를 사용하고 애플리케이션 계층으로 AWS Lambda 기능에 대한 직접 트랜잭션을 사용하십시오. 애플리케이션 서비스 간의 통신 계층으로 Amazon Simple
Queue Service(Amazon SQS)를 사용합니다.
B. Amazon CloudWatch 지표를 사용하여 애플리케이션 성능 기록을 분석하여 성능 장애 시 서버의 최대 사용률을 결정합니다. 최대 요구 사항을 충족하도록 애플리케이션 서버의
Amazon EC2 인스턴스 크기를 늘립니다.
C. Amazon Simple Notification Service(Amazon SNS)를 사용하여 Auto Scaling 그룹의 Amazon EC2에서 실행되는 애플리케이션 서버 간의 메시징을 처리합니다. Amazon
CloudWatch를 사용하여 SNS 대기열 길이를 모니터링하고 필요에 따라 확장 및 축소합니다.
D. Amazon Simple Queue Service(Amazon SQS)를 사용하여 Auto Scaling 그룹의 Amazon EC2에서 실행되는 애플리케이션 서버 간의 메시징을 처리합니다. Amazon
CloudWatch를 사용하여 SQS 대기열 길이를 모니터링하고 통신 실패가 감지되면 확장합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q17
한 회사가 Amazon EC2 인스턴스에서 레거시 시스템을 운영하고 있습니다. 애플리케이션의 코드는 변경할 수 없으며 하나의 인스턴스에서만 실행되어야 합니다. 솔루션 설계자는 시스템 복 구 시간을 향상시키기 위한 탄력적인 솔루션을 고안해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. EC2 인스턴스에 대한 종료 방지 기능을 활성화합니다. 
B. 다중 AZ 배포를 위해 EC2 인스턴스를 구성합니다. 
C. 장애 발생 시 EC2 인스턴스를 복구하기 위해 Amazon CloudWatch 경보를 생성합니다. 
D. 스토리지 중복성을 위해 RAID 구성을 사용하여 두 개의 Amazon Elastic Block Store(Amazon EBS) 볼륨으로 EC2 인스턴스를 시작합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q18
회사는 동일한 AWS 리전에 있는 Amazon S3 버킷에서 사진을 자주 업로드하고 다운로드해야 하는 사진 처리 애플리케이션을 실행합니다. 솔루션 아키텍트가 데이터 전송 비용의 증가를 발견하고 이러한 비용을 줄이기 위한 솔루션을 구현해야 합니다. 솔루션 설계자는 이 요구 사항을 어떻게 충족할 수 있습니까?
A. Amazon API Gateway를 퍼블릭 서브넷에 배포하고 이를 통해 S3 호출을 라우팅하도록 라우팅 테이블을 조정합니다. 
B. 퍼블릭 서브넷에 NAT 게이트웨이를 배포하고 S3 버킷에 대한 액세스를 허용하는 엔드포인트 정책을 연결합니다. 
C. 애플리케이션을 퍼블릭 서브넷에 배포하고 인터넷 게이트웨이를 통해 라우팅하여 S3 버킷에 액세스하도록 허용합니다. 
D. S3 VPC 게이트웨이 엔드포인트를 VPC에 배포하고 S3 버킷에 대한 액세스를 허용하는 엔드포인트 정책을 연결합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q19
회사의 HTTP 애플리케이션은 NLB(Network Load Balancer) 뒤에 있습니다. NLB의 대상 그룹은 웹 서비스를 실행하는 여러 EC2 인스턴스와 함께 Amazon EC2 Auto Scaling 그 룹을 사용하도록 구성됩니다. 회사는 NLB가 애플리케이션에 대한 HTTP 오류를 감지하지 못한다는 것을 알게 됩니다. 이러한 오류는 웹 서비스를 실행하는 EC2 인스턴스를 수동으로 다시 시작해야 합니다. 회사는 사용 자 지정 스크립트나 코드를 작성하지 않고 애플리케이션의 가용성을 개선해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 회사 애플리케이션의 URL을 제공하여 NLB에서 HTTP 상태 확인을 활성화합니다. 
B. EC2 인스턴스에 cron 작업을 추가하여 1분에 한 번씩 로컬 애플리케이션의 로그를 확인합니다. HTTP 오류가 감지된 경우. 응용 프로그램이 다시 시작됩니다. 
C. NLB를 Application Load Balancer로 교체합니다. 회사 애플리케이션의 URL을 제공하여 HTTP 상태 확인을 활성화합니다. 비정상 인스턴스를 교체하도록 Auto Scaling 작업을
구성합니다.
D. NLB에 대한 UnhealthyHostCount 지표를 모니터링하는 Amazon Cloud Watch 경보를 생성합니다. 경보가 ALARM 상태일 때 비정상 인스턴스를 교체하도록 Auto Scaling 작
업을 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q20
한 회사는 us-east-1 지역에서 사진 호스팅 서비스를 운영하여 다양한 국가의 사용자가 사진을 업로드하고 볼 수 있도록 서비스를 제공합니다. 사진의 시청 기간은 몇 달 동안 많이 본 것부터 일주일 미만 동안 잠깐 본 것까지 다양합니다. 각 사진은 최대 20MB까지 가능하며 애플리케이션은 사진 메타데이터를 사용하여 사용자 액세스를 결정합니다. 가장 비용 효율적인 사용자 액세 스를 제공하는 솔루션은 무엇입니까?
A. Amazon DynamoDB에 사진을 저장합니다. DynamoDB Accelerator(DAX)를 활성화하여 자주 보는 항목을 캐시합니다.
B. Amazon S3 Intelligent-Tiering 스토리지 클래스에 사진을 저장합니다. 사진 메타데이터와 해당 S3 위치를 DynamoDB에 저장합니다.
C. Amazon S3 Standard 스토리지 클래스에 사진을 저장합니다. 30일이 지난 사진을 S3 Standard-Infrequent Access(S3 Standard-IA) 스토리지 클래스로 이동하는 S3 수명
주기 정책을 구현합니다. 메타데이터 관리를 위해 객체 태그를 활용합니다.
D. Amazon S3 Glacier 스토리지 클래스에 사진을 저장합니다. 30일이 지난 사진을 S3 Glacier Deep Archive 스토리지 클래스로 전환하도록 S3 수명 주기 정책을 설정합니다.
Amazon OpenSearch Service에 사진 메타데이터와 해당 S3 위치를 저장합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q21
회사에 Amazon EC2 인스턴스에서 실행되는 애플리케이션이 있습니다. EC2 인스턴스는 관련 정책이 있는 IAM 역할을 사용하여 Amazon RDS 데이터베이스에 연결합니다. 회사는 AWS Systems Manager를 사용하여 실행 중인 애플리케이션을 중단하지 않고 EC2 인스턴스를 패치하려고 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 새로운 IAM 역할을 생성합니다. AmazonSSMManagedInstanceCore 정책을 새 IAM 역할에 연결합니다. 새 IAM 역할을 EC2 인스턴스와 기존 IAM 역할에 연결합니다.
B. IAM 사용자를 생성합니다. AmazonSSMManagedInstanceCore 정책을 IAM 사용자에게 연결합니다. IAM 사용자를 사용하여 EC2 인스턴스를 관리하도록 Systems Manager
를 구성합니다.
C. Systems Manager에서 기본 호스트 구성 관리를 활성화하여 EC2 인스턴스를 관리합니다.
D. 기존 IAM 역할에서 기존 정책을 제거합니다. 기존 IAM 역할에 AmazonSSMManagedInstanceCore 정책을 추가합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q22
IoT 회사는 사용자의 수면에 대한 데이터를 수집하는 센서가 있는 매트리스를 출시하고 있습니다. 센서는 데이터를 Amazon S3 버킷으로 보냅니다. 센서는 각 매트리스에 대해 매일 밤 약 2MB의 데이터를 수집합니다. 회사는 각 매트리스에 대한 데이터를 처리하고 요약해야 합니다. 결과는 가능한 한 빨리 제공되어야 합니다. 데이터 처리에는 1GB의 메모리가 필요하며 30초 이내에 완료됩니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. Scala 작업에 AWS Glue 사용 
B. Apache Spark 스크립트와 함께 Amazon EMR 사용 
C. Python 스크립트와 함께 AWS Lambda 사용 
D. PySpark 작업과 함께 AWS Glue 사용

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q23
한 회사가 여러 소스에서 실시간 스트리(cid:1535) 데이터를 수집할 새로운 데이터 플랫폼을 준비하고 있습니다. 회사는 Amazon S3에 데이터를 쓰기 전에 데이터를 변환해야 합니다. 회사는 SQL을 사용하여 변환된 데이터를 쿼리할 수 있는 기능이 필요합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까? (두 가지를 선택하세요.)
A. Amazon Kinesis Data Streams를 사용하여 데이터를 스트리(cid:1535)합니다. Amazon Kinesis Data Analytics를 사용하여 데이터를 변환합니다. Amazon Kinesis Data Firehose
를 사용하여 Amazon S3에 데이터를 씁니다. Amazon Athena를 사용하여 Amazon S3에서 변환된 데이터를 쿼리합니다.
B. Amazon Managed Streaming for Apache Kafka(Amazon MSK)를 사용하여 데이터를 스트리(cid:1535)합니다. AWS Glue를 사용하여 데이터를 변환하고 데이터를 Amazon S3에
씁니다. Amazon Athena를 사용하여 Amazon S3에서 변환된 데이터를 쿼리합니다.
C. AWS Database Migration Service(AWS DMS)를 사용하여 데이터를 수집합니다. Amazon EMR을 사용하여 데이터를 변환하고 Amazon S3에 데이터를 씁니다. Amazon
Athena를 사용하여 Amazon S3에서 변환된 데이터를 쿼리합니다.
D. Amazon Managed Streaming for Apache Kafka(Amazon MSK)를 사용하여 데이터를 스트리(cid:1535)합니다. Amazon Kinesis Data Analytics를 사용하여 데이터를 변환하고
데이터를 Amazon S3에 씁니다. Amazon RDS 쿼리 편집기를 사용하여 Amazon S3에서 변환된 데이터를 쿼리합니다.
E. Amazon Kinesis Data Streams를 사용하여 데이터를 스트리(cid:1535)합니다. AWS Glue를 사용하여 데이터를 변환합니다. Amazon Kinesis Data Firehose를 사용하여 Amazon
S3에 데이터를 씁니다. Amazon RDS 쿼리 편집기를 사용하여 Amazon S3에서 변환된 데이터를 쿼리합니다.

<details>
<summary>정답 보기</summary>

**AB**
</details>

---

### Q24
회사는 단일 공장에 있는 여러 기계에서 매일 10TB의 계측 데이터를 받습니다. 데이터는 공장 내에 위치한 온프레미스 데이터 센터의 SAN(Storage Area Network)에 저장된 JSON 파 일로 구성됩니다. 이 회사는 이 데이터를 거의 실시간에 가까운 중요한 분석을 제공하는 여러 추가 시스템에서 액세스할 수 있는 Amazon S3로 보내려고 합니다. 데이터가 민감한 것으로 간 주되기 때문에 안전한 전송이 중요합니다. 가장 안정적인 데이터 전송을 제공하는 솔루션은 무엇입니까?
A. 퍼블릭 인터넷을 통한 AWS DataSync 
B. AWS Direct Connect를 통한 AWS DataSync 
C. 퍼블릭 인터넷을 통한 AWS DMS(AWS Database Migration Service) 
D. AWS Direct Connect를 통한 AWS DMS(AWS Database Migration Service)

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q25
회사에는 Microsoft Windows 공유 파일 저장소가 필요한 온-프레미스에서 실행되는 대규모 Microsoft SharePoint 배포가 있습니다. 이 회사는 이 워크로드를 AWS 클라우드로 마이그 레이션하려고 하며 다양한 스토리지 옵션을 고려하고 있습니다. 저장소 솔루션은 액세스 제어를 위해 가용성이 높고 Active Directory와 통합되어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon EFS 스토리지를 구성하고 인증을 위한 Active Directory 도메인을 설정합니다. 
B. 두 가용 영역의 AWS Storage Gateway 파일 게이트웨이에 SMB 파일 공유를 생성합니다. 
C. Amazon S3 버킷을 생성하고 이를 볼륨으로 탑재하도록 Microsoft Windows Server를 구성합니다. 
D. AWS에서 Windows File Server 파일 시스템용 Amazon FSx를 생성하고 인증을 위한 Active Directory 도메인을 설정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q26
한 회사가 다중 계층 온프레미스 애플리케이션을 AWS로 마이그레이션하고 있습니다. 애플리케이션은 단일 노드 MySQL 데이터베이스와 다중 노드 웹 계층으로 구성됩니다. 회사는 마이그 레이션 중에 애플리케이션 변경을 최소화해야 합니다. 회사는 마이그레이션 후 애플리케이션 복원성을 개선하려고 합니다. 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (2개를 선택하세요.)
A. 웹 계층을 Application Load Balancer 뒤에 있는 Auto Scaling 그룹의 Amazon EC2 인스턴스로 마이그레이션합니다. 
B. 데이터베이스를 Network Load Balancer 뒤에 있는 Auto Scaling 그룹의 Amazon EC2 인스턴스로 마이그레이션합니다. 
C. 데이터베이스를 Amazon RDS 다중 AZ 배포로 마이그레이션합니다. 
D. 웹 계층을 AWS Lambda 함수로 마이그레이션합니다. 
E. 데이터베이스를 Amazon DynamoDB 테이블로 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q27
회사는 Amazon Elastic Kubernetes Service(Amazon EKS)를 사용하여 컨테이너 애플리케이션을 실행합니다. EKS 클러스터는 Kubernetes 비밀 객체에 민감한 정보를 저장합니 다. 회사는 정보가 암호화되었는지 확인하려고 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 컨테이너 애플리케이션을 사용하여 AWS Key Management Service(AWS KMS)를 사용하여 정보를 암호화합니다. 
B. AWS Key Management Service(AWS KMS)를 사용하여 EKS 클러스터에서 비밀 암호화를 활성화합니다. 
C. AWS KMS(AWS Key Management Service)를 사용하여 정보를 암호화하는 AWS Lambda 함수를 구현합니다. 
D. AWS Systems Manager Parameter Store를 사용하여 AWS Key Management Service(AWS KMS)를 사용하여 정보를 암호화합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q28
회사에는 동일한 AWS 계정 내의 us-west-2 리전에 위치한 두 개의 VPC가 있습니다. 회사는 이러한 VPC 간의 네트워크 트래픽을 허용해야 합니다. 매월 VPC 간에 약 500GB의 데이터 전송이 발생합니다. 이러한 VPC를 연결하는 가장 비용 효율적인 솔루션은 무엇입니까?
A. AWS Transit Gateway를 구현하여 VPC를 연결합니다. VPC 간 통신에 전송 게이트웨이를 사용하도록 각 VPC의 라우팅 테이블을 업데이트합니다. 
B. VPC 간에 AWS Site-to-Site VPN 터널을 구현합니다. VPC 간 통신에 VPN 터널을 사용하도록 각 VPC의 라우팅 테이블을 업데이트합니다. 
C. VPC 간에 VPC 피어링 연결을 설정합니다. VPC 간 통신에 VPC 피어링 연결을 사용하도록 각 VPC의 라우팅 테이블을 업데이트합니다. 
D. VPC 간에 1GB AWS Direct Connect 연결을 설정합니다. VPC 간 통신에 Direct Connect 연결을 사용하도록 각 VPC의 라우팅 테이블을 업데이트합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q29
연구 회사에서는 온프레미스 장치를 사용하여 분석용 데이터를 생성합니다. 회사는 AWS 클라우드를 사용하여 데이터를 분석하려고 합니다. 장치는 .csv 파일을 생성하고 SMB 파일 공유에 데이터 쓰기를 지원합니다. 회사 분석가는 SQL 명령을 사용하여 데이터를 쿼리할 수 있어야 합니다. 분석가는 하루 종일 주기적으로 쿼리를 실행합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 단계 조합은 무엇입니까? (3개를 선택하세요.)
A. Amazon S3 파일 게이트웨이 모드로 온프레미스에 AWS Storage Gateway를 배포합니다. 
B. Amazon FSx File Gateway를 통해 온프레미스에 AWS Storage Gateway를 배포합니다. 
C. Amazon S3에 있는 데이터를 기반으로 테이블을 생성하도록 AWS Glue 크롤러를 설정합니다. 
D. EMRFS(EMR 파일 시스템)를 사용하여 Amazon EMR 클러스터를 설정하여 Amazon S3에 있는 데이터를 쿼리합니다. 분석가에 대한 액세스를 제공합니다. 
E. Amazon S3에 있는 데이터를 쿼리하도록 Amazon Redshift 클러스터를 설정합니다. 분석가에 대한 액세스를 제공합니다. 
F. Amazon S3에 있는 데이터를 쿼리하도록 Amazon Athena를 설정합니다. 분석가에 대한 액세스를 제공합니다.

<details>
<summary>정답 보기</summary>

**ACF**
</details>

---

### Q30
한 회사가 여러 AWS 계정에서 프로덕션 및 비프로덕션 환경 워크로드를 실행하고 있습니다. 계정은 AWS Organizations의 조직에 있습니다. 회사는 비용 사용 태그의 수정을 방지하는 솔 루션을 설계해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 권한이 부여된 보안 주체 외에는 태그 수정을 방지하기 위해 사용자 지정 AWS Config 규칙을 생성합니다.
B. 태그 수정을 방지하기 위해 AWS CloudTrail에서 사용자 지정 추적을 생성합니다.
C. 인증된 주체 외에는 태그 수정을 방지하기 위해 서비스 제어 정책(SCP)을 생성합니다.
D. 태그 수정을 방지하기 위해 사용자 지정 Amazon CloudWatch 로그를 생성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q31
회사에서 공개적으로 액세스할 수 있는 영화 데이터를 저장하기 위해 SQL 데이터베이스를 사용하고 있습니다. 데이터베이스는 Amazon RDS 단일 AZ DB 인스턴스에서 실행됩니다. 스크 립트는 데이터베이스에 추가된 새 영화의 수를 기록하기 위해 매일 임의의 간격으로 쿼리를 실행합니다. 스크립트는 업무 시간 동안 최종 합계를 보고해야 합니다. 회사의 개발 팀은 스크립트가 실행 중일 때 데이터베이스 성능이 개발 작업에 적합하지 않다는 것을 알게 되었습니다. 솔루션 설계자는 이 문제를 해결하기 위한 솔루션을 추천해야 합니다. 최소한의 운영 오버헤드로 이 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 다중 AZ 배포가 되도록 DB 인스턴스를 수정합니다. 
B. 데이터베이스의 읽기 전용 복제본을 생성합니다. 읽기 전용 복제본만 쿼리하도록 스크립트를 구성합니다. 
C. 개발 팀에게 매일 일과가 끝날 때 데이터베이스의 항목을 수동으로 내보내도록 지시합니다. 
D. Amazon ElastiCache를 사용하여 스크립트가 데이터베이스에 대해 실행하는 일반적인 쿼리를 캐시합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q32
회사는 애플리케이션에 대한 실시간 데이터 수집 아키텍처를 구성해야 합니다. 회사는 API, 데이터가 스트리(cid:1535)될 때 데이터를 변환하는 프로세스, 데이터를 위한 스토리지 솔루션이 필요합니 다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Kinesis 데이터 스트림으로 데이터를 전송하는 API를 호스팅하기 위해 Amazon EC2 인스턴스를 배포합니다. Kinesis 데이터 스트림을 데이터 소스로 사용하는 Amazon
Kinesis Data Firehose 전송 스트림을 생성합니다. AWS Lambda 함수를 사용하여 데이터를 변환합니다. Kinesis Data Firehose 전송 스트림을 사용하여 데이터를 Amazon S3로 보냅니다.
B. AWS Glue로 데이터를 전송하는 API를 호스팅하기 위해 Amazon EC2 인스턴스를 배포합니다. EC2 인스턴스에서 소스/대상 확인을 중지합니다. AWS Glue를 사용하여 데이터를
변환하고 데이터를 Amazon S3로 보냅니다.
C. Amazon Kinesis 데이터 스트림으로 데이터를 전송하도록 Amazon API Gateway API를 구성합니다. Kinesis 데이터 스트림을 데이터 소스로 사용하는 Amazon Kinesis Data
Firehose 전송 스트림을 생성합니다. AWS Lambda 함수를 사용하여 데이터를 변환합니다. Kinesis Data Firehose 전송 스트림을 사용하여 데이터를 Amazon S3로 보냅니다.
D. AWS Glue로 데이터를 전송하도록 Amazon API Gateway API를 구성합니다. AWS Lambda 함수를 사용하여 데이터를 변환합니다. AWS Glue를 사용하여 데이터를 Amazon
S3로 보냅니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q33
회사는 데이터 센터에서 SMB 파일 서버를 실행하고 있습니다. 파일 서버는 파일이 생성된 후 처음 며칠 동안 자주 액세스되는 대용량 파일을 저장합니다. 7일 후에는 파일에 거의 액세스하지 않습니다. 총 데이터 크기는 증가하고 있으며 회사의 총 스토리지 용량에 근접합니다. 솔루션 설계자는 가장 최근에 액세스한 파일에 대한 짧은 대기 시간 액세스를 잃지 않고 회사의 사용 가능한 스토리 지 공간을 늘려야 합니다. 솔루션 설계자는 향후 스토리지 문제를 방지하기 위해 파일 수명 주기 관리도 제공해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS DataSync를 사용하여 SMB 파일 서버에서 AWS로 7일보다 오래된 데이터를 복사합니다. 
B. Amazon S3 File Gateway를 생성하여 회사의 스토리지 공간을 확장합니다. 7일 후에 데이터를 S3 Glacier Deep Archive로 전환하는 S3 수명 주기 정책을 생성합니다. 
C. Amazon FSx for Windows File Server 파일 시스템을 생성하여 회사의 스토리지 공간을 확장합니다. 
D. 각 사용자의 컴퓨터에 유틸리티를 설치하여 Amazon S3에 액세스합니다. 7일 후에 데이터를 S3 Glacier Flexible Retrieval로 전환하는 S3 수명 주기 정책을 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q34
회사에서 AWS Organizations를 사용합니다. 회사는 다른 예산으로 일부 AWS 계정을 운영하려고 합니다. 회사는 특정 기간 동안 할당된 예산 임계값에 도달하면 알림을 받고 AWS 계정 에 추가 리소스 프로비저닝을 자동으로 방지하려고 합니다. 이러한 요구 사항을 충족하는 솔루션 조합은 무엇입니까? (3개를 선택하세요.)
A. AWS 예산을 사용하여 예산을 생성합니다. 필요한 AWS 계정의 비용 및 사용 보고서 섹션에서 예산 금액을 설정합니다. 
B. AWS 예산을 사용하여 예산을 생성합니다. 필요한 AWS 계정의 결제 대시보드에서 예산 금액을 설정합니다. 
C. 필요한 권한으로 예산 작업을 실행하기 위해 AWS 예산에 대한 IAM 사용자를 생성합니다. 
D. 필요한 권한으로 예산 작업을 실행하기 위해 AWS 예산에 대한 IAM 역할을 생성합니다. 
E. 각 계정이 예산 임계값을 충족할 때 회사에 알리는 경고를 추가합니다. 추가 리소스의 프로비저닝을 방지하기 위해 적절한 구성 규칙으로 생성된 IAM 자격 증명을 선택하는 예산 작업을 추
가합니다. F. 각 계정이 예산 임계값을 충족할 때 회사에 알리는 경고를 추가합니다. 추가 리소스의 프로비저닝을 방지하기 위해 적절한 SCP(서비스 제어 정책)로 생성된 IAM 자격 증명을 선택하는 예 산 작업을 추가합니다.

<details>
<summary>정답 보기</summary>

**BDF**
</details>

---

### Q35
회사는 온프레미스 서버를 사용하여 애플리케이션을 호스팅합니다. 회사의 저장 용량이 부족합니다. 애플리케이션은 블록 스토리지와 NFS 스토리지를 모두 사용합니다. 회사는 기존 애플리케 이션을 재설계하지 않고 로컬 캐싱을 지원하는 고성능 솔루션이 필요합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 작업 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. Amazon S3를 온프레미스 서버에 파일 시스템으로 탑재합니다. 
B. NFS 스토리지를 대체할 AWS Storage Gateway 파일 게이트웨이를 배포합니다. 
C. AWS Snowball Edge를 배포하여 온프레미스 서버에 NFS 마운트를 프로비저닝합니다. 
D. 블록 스토리지를 대체할 AWS Storage Gateway 볼륨 게이트웨이를 배포합니다. 
E. Amazon Elastic File System(Amazon EFS) 볼륨을 배포하고 온프레미스 서버에 탑재합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q36
한 회사에서 온프레미스 Microsoft SQL Server Enterprise 에디션 데이터베이스를 AWS로 마이그레이션하려고 합니다. 회사의 온라인 애플리케이션은 데이터베이스를 사용하여 거래를 처리합니다. 데이터 분석 팀은 동일한 프로덕션 데이터베이스를 사용하여 분석 처리를 위한 보고서를 실행합니다. 회사는 가능한 한 관리형 서비스로 전환하여 운영 오버헤드를 줄이고 싶어합 니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Microsoft SOL Server용 Amazon RDS로 마이그레이션하십시오. 보고 목적으로 읽기 복제본 사용 
B. Amazon EC2의 Microsoft SQL Server로 마이그레이션합니다. 보고 목적으로 Always On 읽기 복제본 사용 
C. Amazon DynamoDB로 마이그레이션합니다. 보고 목적으로 DynamoDB 온디맨드 복제본 사용 
D. Amazon Aurora MySQL로 마이그레이션합니다. 보고 목적으로 Aurora 읽기 전용 복제본 사용

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q37
한 회사의 전자상거래 웹사이트에 예측할 수 없는 트래픽이 있으며 AWS Lambda 기능을 사용하여 PostgreSQL용 프라이빗 Amazon RDS DB 인스턴스에 직접 액세스합니다. 회사는 예측 가능한 데이터베이스 성능을 유지하고 Lambda 호출이 너무 많은 연결로 인해 데이터베이스에 과부하가 걸리지 않도록 하려고 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. RDS 사용자 지정 끝점에서 클라이언트 드라이버를 가리킵니다. VPC 내부에 Lambda 함수를 배포합니다. 
B. RDS 프록시 엔드포인트에서 클라이언트 드라이버를 가리킵니다. VPC 내부에 Lambda 함수를 배포합니다. 
C. RDS 사용자 지정 엔드포인트에서 클라이언트 드라이버를 가리킵니다. VPC 외부에 Lambda 함수를 배포합니다. 
D. RDS 프록시 엔드포인트에서 클라이언트 드라이버를 가리킵니다. VPC 외부에 Lambda 함수를 배포합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q38
솔루션 설계자는 VPC의 Amazon EC2 인스턴스에서 Amazon DynamoDB에 대한 API 호출이 인터넷을 통해 이동하지 않도록 해야 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. 엔드포인트에 대한 라우팅 테이블 항목을 생성합니다. 
B. DynamoDB용 게이트웨이 엔드포인트를 생성합니다. 
C. Amazon EC2용 인터페이스 엔드포인트를 생성합니다. 
D. VPC의 각 서브넷에서 끝점에 대한 탄력적 네트워크 인터페이스를 만듭니다. 
E. 엔드포인트의 보안 그룹에 보안 그룹 항목을 생성하여 액세스를 제공합니다.

<details>
<summary>정답 보기</summary>

**AB**
</details>

---

### Q39
전자상거래 애플리케이션은 Amazon EC2 인스턴스에서 실행되는 PostgreSQL 데이터베이스를 사용합니다. 월별 판매 이벤트 중에 데이터베이스 사용량이 증가하고 애플리케이션에 대한 데이터베이스 연결 문제가 발생합니다. 후속 월별 판매 이벤트에 대한 트래픽은 예측할 수 없으며 이는 판매 예측에 영향을 미칩니다. 회사는 예측할 수 없는 트래픽 증가가 있을 때 성능을 유지 해야 합니다. 가장 비용 효과적인 방법으로 이 문제를 해결하는 솔루션은 무엇입니까?
A. PostgreSQL 데이터베이스를 Amazon Aurora Serverless v2로 마이그레이션합니다. 
B. 증가된 사용량을 수용하기 위해 EC2 인스턴스의 PostgreSQL 데이터베이스에 대한 자동 크기 조정을 활성화합니다. 
C. 더 큰 인스턴스 유형을 사용하여 PostgreSQL 데이터베이스를 PostgreSQL용 Amazon RDS로 마이그레이션합니다. 
D. 증가된 사용량을 수용하기 위해 PostgreSQL 데이터베이스를 Amazon Redshift로 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q40
온라인 비디오 게임 회사는 게임 서버에 대해 매우 낮은 대기 시간을 유지해야 합니다. 게임 서버는 Amazon EC2 인스턴스에서 실행됩니다. 회사에는 초당 수백만 건의 UDP 인터넷 트래픽 요청을 처리할 수 있는 솔루션이 필요합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 인터넷 트래픽에 필요한 프로토콜과 포트로 Application Load Balancer를 구성합니다. EC2 인스턴스를 대상으로 지정합니다. 
B. 인터넷 트래픽을 위한 게이트웨이 로드 밸런서를 구성합니다. EC2 인스턴스를 대상으로 지정합니다. 
C. 인터넷 트래픽에 필요한 프로토콜과 포트로 Network Load Balancer를 구성합니다. EC2 인스턴스를 대상으로 지정합니다. 
D. 별도의 AWS 지역에 있는 EC2 인스턴스에서 동일한 게임 서버 세트를 시작합니다. 인터넷 트래픽을 두 EC2 인스턴스 세트로 라우팅합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q41
회사에서 데이터 저장을 위해 Amazon DynamoDB 테이블을 사용할 계획입니다. 회사는 비용 최적화에 관심이 있습니다. 테이블은 대부분의 아침에 사용되지 않습니다. 저녁에는 읽기 및 쓰기 트래픽을 예측할 수 없는 경우가 많습니다. 트래픽 급증이 발생하면 매우 빠르게 발생합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. 온디맨드 용량 모드에서 DynamoDB 테이블을 생성합니다. 
B. 글로벌 보조 인덱스가 있는 DynamoDB 테이블을 생성합니다. 
C. 프로비저닝된 용량과 Auto Scaling으로 DynamoDB 테이블을 생성합니다. 
D. 프로비저닝된 용량 모드에서 DynamoDB 테이블을 생성하고 글로벌 테이블로 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q42
다수의 AWS 계정에서 AWS CloudTrail 로그를 중앙 AWS 계정의 Amazon S3 버킷으로 전송하고, 이 로그를 보존하면서 필요한 때에 언제든지 CloudTrail 로그를 쿼리할 수 있는 솔 루션은 무엇일까요?
A. 중앙 계정의 CloudTrail 이벤트 기록을 사용하여 Amazon Athena 테이블을 생성하고, Athena를 사용하여 CloudTrail 로그를 쿼리합니다. 
B. Amazon Neptune 인스턴스를 구성하여 CloudTrail 로그를 관리하고, Neptune에서 로그를 쿼리합니다. 
C. CloudTrail을 구성하여 로그를 Amazon DynamoDB 테이블로 전송하고, Amazon QuickSight에서 해당 테이블의 로그를 쿼리할 수 있는 대시보드를 생성합니다. 
D. Amazon Athena에서 Athena 노트북을 생성하고, CloudTrail을 노트북으로 전송하여 Athena에서 쿼리를 실행합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q43
회사에서 온프레미스 애플리케이션을 AWS로 마이그레이션하려고 합니다. 이 애플리케이션은 수십 기가바이트에서 수백 테라바이트에 이르는 다양한 크기의 출력 파일을 생성합니다. 애플리 케이션 데이터는 표준 파일 시스템 구조에 저장되어야 합니다. 회사는 자동으로 확장되는 솔루션을 원합니다. 가용성이 높고 최소한의 운영 오버헤드가 필요합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Elastic Container Service(Amazon ECS)에서 컨테이너로 실행되도록 애플리케이션을 마이그레이션합니다. 저장을 위해 Amazon S3를 사용합니다. 
B. Amazon Elastic Kubernetes Service(Amazon EKS)에서 컨테이너로 실행되도록 애플리케이션을 마이그레이션합니다. 저장을 위해 Amazon Elastic Block Store(Amazon
EBS)를 사용합니다.
C. 다중 AZ Auto Scaling 그룹의 Amazon EC2 인스턴스로 애플리케이션을 마이그레이션합니다. 스토리지에 Amazon Elastic File System(Amazon EFS)을 사용합니다. 
D. 다중 AZ Auto Scaling 그룹의 Amazon EC2 인스턴스로 애플리케이션을 마이그레이션합니다. 저장을 위해 Amazon Elastic Block Store(Amazon EBS)를 사용합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q44
한 회사가 3개의 가용 영역에서 작동하는 AWS 클라우드에서 3계층 웹 애플리케이션을 실행합니다. 애플리케이션 아키텍처에는 Application Load Balancer, 사용자 세션 상태를 호스팅 하는 Amazon EC2 웹 서버, EC2 인스턴스에서 실행되는 MySQL 데이터베이스가 있습니다. 회사는 애플리케이션 트래픽이 갑자기 증가할 것으로 예상합니다. 이 회사는 미래의 애플리케 이션 용량 수요를 충족하고 3개의 가용 영역 모두에서 고가용성을 보장하기 위해 확장할 수 있기를 원합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 다중 AZ DB 클러스터 배포를 통해 MySQL 데이터베이스를 MySQL용 Amazon RDS로 마이그레이션합니다. 고가용성 Redis용 Amazon ElastiCache를 사용하여 세션 데이터
를 저장하고 읽기를 캐시하십시오. 세 개의 가용 영역에 있는 Auto Scaling 그룹으로 웹 서버를 마이그레이션합니다.
B. 다중 AZ DB 클러스터 배포를 통해 MySQL 데이터베이스를 MySQL용 Amazon RDS로 마이그레이션합니다. 고가용성 Memcached용 Amazon ElastiCache를 사용하여 세션
데이터를 저장하고 읽기를 캐시하십시오. 세 개의 가용 영역에 있는 Auto Scaling 그룹으로 웹 서버를 마이그레이션합니다.
C. MySQL 데이터베이스를 Amazon DynamoDB로 마이그레이션 DynamoDB Accelerator(DAX)를 사용하여 읽기를 캐시합니다. DynamoDB에 세션 데이터를 저장합니다. 세 개
의 가용 영역에 있는 Auto Scaling 그룹으로 웹 서버를 마이그레이션합니다.
D. 단일 가용 영역에서 MySQL 데이터베이스를 MySQL용 Amazon RDS로 마이그레이션합니다. 고가용성 Redis용 Amazon ElastiCache를 사용하여 세션 데이터를 저장하고 읽기
를 캐시하십시오. 세 개의 가용 영역에 있는 Auto Scaling 그룹으로 웹 서버를 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q45
한 회사에서 300개 이상의 글로벌 웹사이트와 애플리케이션을 호스팅합니다. 이 회사는 매일 30TB 이상의 클릭스트림 데이터를 분석할 플랫폼이 필요합니다. 솔루션 설계자는 클릭 스트림 데이터를 전송하고 처리하기 위해 무엇을 해야 합니까?
A. 데이터를 Amazon S3 버킷에 보관하고 데이터로 Amazon EMR 클러스터를 실행하여 분석을 생성하도록 AWS Data Pipeline을 설계합니다. 
B. Amazon EC2 인스턴스의 Auto Scaling 그룹을 생성하여 데이터를 처리하고 Amazon Redshift가 분석에 사용할 수 있도록 Amazon S3 데이터 레이크로 보냅니다. 
C. 데이터를 Amazon CloudFront에 캐시합니다. 데이터를 Amazon S3 버킷에 저장합니다. 객체가 S3 버킷에 추가될 때. AWS Lambda 함수를 실행하여 분석을 위해 데이터를 처리
합니다.
D. Amazon Kinesis Data Streams에서 데이터를 수집합니다. Amazon Kinesis Data Firehose를 사용하여 데이터를 Amazon S3 데이터 레이크로 전송합니다. 분석을 위해
Amazon Redshift에 데이터를 로드합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q46
회사에서 AWS Lambda와 함께 이벤트 기반 프로그래(cid:1535) 모델을 사용하려고 합니다. 회사는 Java 11에서 실행되는 Lambda 함수의 시작 지연 시간을 줄이려고 합니다. 회사는 애플리케이 션에 대한 엄격한 지연 시간 요구 사항이 없습니다. 이 회사는 함수가 확장될 때 콜드 스타트와 이상치 대기 시간을 줄이려고 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. Lambda 프로비저닝된 동시성을 구성합니다. 
B. Lambda 함수의 제한 시간을 늘립니다. 
C. Lambda 함수의 메모리를 늘립니다. 
D. Lambda SnapStart를 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q47
한 회사에서 Amazon DynamoDB를 데이터베이스 계층으로 사용하는 서버리스 애플리케이션을 배포했습니다. 응용 프로그램의 사용자가 크게 증가했습니다. 이 회사는 데이터베이스 응답 시간을 밀리초에서 마이크로초로 개선하고 데이터베이스에 대한 요청을 캐시하기를 원합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. DynamoDB 가속기(DAX)를 사용합니다. 
B. 데이터베이스를 Amazon Redshift로 마이그레이션합니다. 
C. 데이터베이스를 Amazon RDS로 마이그레이션합니다. 
D. Redis용 Amazon ElastiCache를 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q48
한 병원은 최근 Amazon API Gateway 및 AWS Lambda와 함께 RESTful API를 배포했습니다. 병원은 API 게이트웨이와 Lambda를 사용하여 PDF 형식과 JPEG 형식의 보고서 를 업로드합니다. 병원은 보고서에서 보호 건강 정보(PHI)를 식별하기 위해 Lambda 코드를 수정해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 기존 Python 라이브러리를 사용하여 보고서에서 텍스트를 추출하고 추출된 텍스트에서 PHI를 식별합니다. 
B. Amazon Textract를 사용하여 보고서에서 텍스트를 추출합니다. Amazon SageMaker를 사용하여 추출된 텍스트에서 PHI를 식별합니다. 
C. Amazon Textract를 사용하여 보고서에서 텍스트를 추출합니다. Amazon Comprehend Medical을 사용하여 추출된 텍스트에서 PHI를 식별합니다. 
D. Amazon Rekognition을 사용하여 보고서에서 텍스트를 추출합니다. Amazon Comprehend Medical을 사용하여 추출된 텍스트에서 PHI를 식별합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q49
한 제조 회사가 AWS에서 보고서 생성 애플리케이션을 실행하고 있습니다. 애플리케이션은 약 20분 안에 각 보고서를 생성합니다. 애플리케이션은 단일 Amazon EC2 인스턴스에서 실행되 는 모놀리스로 구축되었습니다. 애플리케이션에는 긴밀하게 결합된 모듈을 자주 업데이트해야 합니다. 회사에서 새로운 기능을 추가하면 애플리케이션을 유지 관리하기가 복잡해집니다. 회사에서 소프트웨어 모듈을 패치할 때마다 애플리케이션에 가동 중지 시간이 발생합니다. 보고서 생성은 중단된 후에 처음부터 다시 시작되어야 합니다. 회사는 애플리케이션이 유연하고 확장 가능하며 점진적으로 개선될 수 있도록 애플리케이션을 재설계하려고 합니다. 회사는 애플리케이션 가동 중지 시간을 최소화하려고 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS Lambda에서 최대 프로비저닝 동시성을 갖춘 단일 함수로 애플리케이션을 실행합니다. 
B. 스팟 집합 기본 할당 전략을 사용하여 Amazon EC2 스팟 인스턴스에서 애플리케이션을 마이크로서비스로 실행합니다. 
C. 서비스 자동 조정을 통해 Amazon Elastic Container Service(Amazon ECS)에서 애플리케이션을 마이크로서비스로 실행합니다. 
D. 일괄 배포 전략을 사용하여 AWS Elastic Beanstalk에서 애플리케이션을 단일 애플리케이션 환경으로 실행합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q50
애플리케이션은 Amazon RDS MySQL DB 인스턴스를 사용합니다. RDS 데이터베이스의 디스크 공간이 부족해지고 있습니다. 솔루션 설계자는 다운타임 없이 디스크 공간을 늘리고 싶어 합니다. 최소한의 노력으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. RDS에서 스토리지 자동 확장 활성화
B. RDS 데이터베이스 인스턴스 크기 늘리기
C. RDS 데이터베이스 인스턴스 스토리지 유형을 프로비저닝된 IOPS로 변경
D. RDS 데이터베이스 백업, 저장 용량 증가, 데이터베이스 복원 및 이전 인스턴스 중지

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q51
회사는 AWS에서 인프라를 실행하고 문서 관리 애플리케이션에 대해 700,000명의 등록된 사용자 기반을 가지고 있습니다. 회사는 대용량 .pdf 파일을 .jpg 이미지 파일로 변환하는 제품을 만들려고 합니다. .pdf 파일의 평균 크기는 5MB입니다. 회사는 원본 파일과 변환된 파일을 보관해야 합니다. 솔루션 설계자는 시간이 지남에 따라 빠르게 증가할 수요를 수용할 수 있는 확장 가능한 솔루션을 설계해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. .pdf 파일을 Amazon S3에 저장합니다. 파일을 .jpg 형식으로 변환하고 Amazon S3에 다시 저장하는 AWS Lambda 함수를 호출하도록 S3 PUT 이벤트를 구성합니다. 
B. .pdf 파일을 Amazon Dynamo에 저장합니다DynamoDB Streams 기능을 사용하여 AWS Lambda 함수를 호출하여 파일을 .jpg 형식으로 변환하고 다시 DynamoDB에 저장합
니다.
C. Amazon EC2 인스턴스, Amazon Elastic Block Store(Amazon EBS) 스토리지 및 Auto Scaling 그룹을 포함하는 AWS Elastic Beanstalk 애플리케이션에 .pdf 파일을 업
로드합니다. EC2 인스턴스의 프로그램을 사용하여 파일을 .jpg 형식으로 변환합니다. .pdf 파일과 .jpg 파일을 EBS 스토어에 저장합니다.
D. Amazon EC2 인스턴스, Amazon Elastic File System(Amazon EFS) 스토리지 및 Auto Scaling 그룹이 포함된 AWS Elastic Beanstalk 애플리케이션에 .pdf 파일을 업로
드합니다. EC2 인스턴스의 프로그램을 사용하여 파일을 .jpg 형식으로 변환합니다. .pdf 파일과 .jpg 파일을 EBS 스토어에 저장합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q52
게임 회사는 Amazon DynamoDB를 사용하여 지리적 위치, 플레이어 데이터 및 순위표와 같은 사용자 정보를 저장합니다. 회사는 최소한의 코딩으로 Amazon S3 버킷에 대한 지속적인 백업을 구성해야 합니다. 백업은 애플리케이션의 가용성에 영향을 미치지 않아야 하며 테이블에 대해 정의된 읽기 용량 단위(RCU)에 영향을 주지 않아야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon EMR 클러스터를 사용하십시오. Apache Hive 작업을 생성하여 Amazon S3에 데이터를 백업합니다. 
B. 연속 백업을 통해 DynamoDB에서 Amazon S3로 직접 데이터를 내보냅니다. 테이블에 대해 지정 시간 복구를 설정합니다. 
C. Amazon DynamoDB 스트림을 구성합니다. 스트림을 사용하고 데이터를 Amazon S3 버킷으로 내보내는 AWS Lambda 함수를 생성합니다. 
D. 정기적으로 데이터베이스 테이블에서 Amazon S3로 데이터를 내보내는 AWS Lambda 함수를 생성합니다. 테이블에 대해 지정 시간 복구를 설정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q53
회사의 동적 웹 사이트는 미국의 온프레미스 서버를 사용하여 호스팅됩니다. 이 회사는 유럽에서 제품을 출시하고 있으며 새로운 유럽 사용자를 위해 사이트 로드 시간을 최적화하려고 합니다. 사이트의 백엔드는 미국에 남아 있어야 합니다. 이 제품은 며칠 안에 출시되며 즉각적인 솔루션이 필요합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. us-east-1에서 Amazon EC2 인스턴스를 시작하고 사이트를 여기로 마이그레이션합니다. 
B. 웹사이트를 Amazon S3로 이동합니다. 리전 간 교차 리전 복제를 사용합니다. 
C. 온프레미스 서버를 가리키는 사용자 지정 오리진과 함께 Amazon CloudFront를 사용합니다. 
D. 온프레미스 서버를 가리키는 Amazon Route 53 지리 근접 라우팅 정책을 사용합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q54
회사는 Amazon S3를 사용하여 기밀 감사 문서를 저장합니다. S3 버킷은 버킷 정책을 사용하여 최소 권한 원칙에 따라 감사 팀 IAM 사용자 자격 증명에 대한 액세스를 제한합니다. 회사 관 리자는 S3 버킷의 문서를 실수로 삭제하는 것에 대해 걱정하고 보다 안전한 솔루션을 원합니다. 솔루션 설계자는 감사 문서를 보호하기 위해 무엇을 해야 합니까?
A. S3 버킷에서 버전 관리 및 MFA 삭제 기능을 활성화합니다. 
B. 각 감사 팀 IAM 사용자 계정의 IAM 사용자 자격 증명에서 다중 요소 인증(MFA)을 활성화합니다. 
C. 감사 날짜 동안 s3:DeleteObject 작업을 거부하도록 감사 팀의 IAM 사용자 계정에 S3 수명 주기 정책을 추가합니다. 
D. AWS Key Management Service(AWS KMS)를 사용하여 S3 버킷을 암호화하고 감사 팀 IAM 사용자 계정이 KMS 키에 액세스하지 못하도록 제한합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q55
회사에서 인프라 모니터링 서비스를 실행합니다. 이 회사는 서비스가 고객 AWS 계정의 데이터를 모니터링할 수 있는 새로운 기능을 구축하고 있습니다. 새로운 기능은 고객 계정에서 AWS API를 호출하여 Amazon EC2 인스턴스를 설명하고 Amazon CloudWatch 지표를 읽습니다. 회사는 가장 안전한 방법으로 고객 계정에 대한 액세스 권한을 얻기 위해 무엇을 해야 합니까?
A. 고객이 회사 계정에 대한 읽기 전용 EC2 및 CloudWatch 권한과 신뢰 정책을 사용하여 계정에 IAM 역할을 생성하는지 확인하십시오. 
B. 토큰 판매기를 구현하는 서버리스 API를 생성하여 읽기 전용 EC2 및 CloudWatch 권한이 있는 역할에 대한 임시 AWS 자격 증명을 제공합니다. 
C. 고객이 자신의 계정에서 읽기 전용 EC2 및 CloudWatch 권한을 가진 IAM 사용자를 생성하는지 확인합니다. 비밀 관리 시스템에서 고객 액세스 및 비밀 키를 암호화하고 저장합니다. 
D. 고객이 자신의 계정에 Amazon Cognito 사용자를 생성하여 읽기 전용 EC2 및 CloudWatch 권한이 있는 IAM 역할을 사용하는지 확인합니다. 암호 관리 시스템에서 Amazon
Cognito 사용자 및 암호를 암호화하고 저장합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q56
솔루션 설계자가 애플리케이션을 위한 새로운 Amazon CloudFront 배포를 생성하고 있습니다. 사용자가 제출한 정보 중 일부는 민감한 정보입니다. 애플리케이션은 HTTPS를 사용하지만 다른 보안 계층이 필요합니다. 민감한 정보는 전체 애플리케이션 스택에서 보호되어야 하며 정보에 대한 액세스는 특정 애플리케이션으로 제한되어야 합니다. 솔루션 설계자는 어떤 조치를 취해야 합니까?
A. CloudFront를 구성하고 뷰어 프로토콜 정책에 대해 오리진 프로토콜 정책 설정을 HTTPS 전용으로 설정합니다.
B. CloudFront 서명 URL을 구성합니다.
C. CloudFront 필드 수준 암호화 프로필을 구성합니다.
D. CloudFront 서명 쿠키를 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q57
회사에는 매주 금요일 저녁에 실행되는 대규모 워크로드가 있습니다. 워크로드는 us-east-1 리전의 두 가용 영역에 있는 Amazon EC2 인스턴스에서 실행됩니다. 일반적으로 회사는 항상 두 개 이상의 인스턴스를 실행하지 않아야 합니다. 그러나 회사는 정기적으로 반복되는 증가된 워크로드를 처리하기 위해 금요일마다 최대 6개의 인스턴스로 확장하려고 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon EventBridge에서 미리 알림을 생성하여 인스턴스를 확장하십시오. 
B. 예약된 작업이 있는 Auto Scaling 그룹을 생성합니다. 
C. 수동 조정을 사용하는 Auto Scaling 그룹을 생성합니다. 
D. 자동 조정을 사용하는 Auto Scaling 그룹을 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q58
회사에는 회사 데이터 센터에서 us-east-1 지역의 VPC까지 AWS Direct Connect 연결이 있습니다. 여러 개의 VPC와 eu-west-2 지역에 대한 Direct Connect 연결을 갖춘 다른 회 사를 인수한 후에는 두 지역과 데이터 센터 간의 연결을 설정해야 합니다. VPC의 CIDR 블록은 겹치지 않습니다. 목표는 운영 오버헤드를 최소화하면서 확장 가능한 연결을 보장하는 것입니 다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. us-east-1의 VPC와 eu-west-2의 VPC 간에 리전 간 VPC 피어링을 설정합니다. 
B. us-east-1의 Direct Connect 연결에서 eu-west-2의 VPC로 프라이빗 가상 인터페이스를 생성합니다. 
C. Amazon EC2에서 호스팅하는 완전히 메시된 VPN 네트워크에 VPN 어플라이언스를 배포합니다. AWS VPN CloudHub를 사용하여 데이터 센터와 각 VPC 간의 데이터 교환을 촉
진합니다.
D. 기존 Direct Connect 연결을 Direct Connect 게이트웨이에 연결합니다. 각 리전에 있는 VPC의 가상 프라이빗 게이트웨이에서 Direct Connect 게이트웨이로 트래픽을 라우팅합니
다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q59
회사에는 사용자가 웹 인터페이스 또는 모바일 앱을 통해 문서를 업로드하는 프로덕션 웹 애플리케이션이 있습니다. 새로운 규제 요구 사항에 따라. 새 문서는 저장된 후에 수정하거나 삭제할 수 없습니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. S3 버전 관리 및 S3 객체 잠금이 활성화된 Amazon S3 버킷에 업로드된 문서를 저장합니다. 
B. 업로드된 문서를 Amazon S3 버킷에 저장합니다. 문서를 주기적으로 보관하도록 S3 수명 주기 정책을 구성합니다. 
C. 업로드된 문서를 S3 버전 관리가 활성화된 Amazon S3 버킷에 저장합니다. 모든 액세스를 읽기 전용으로 제한하도록 ACL을 구성합니다. 
D. 업로드된 문서를 Amazon Elastic File System(Amazon EFS) 볼륨에 저장합니다. 읽기 전용 모드로 볼륨을 마운트하여 데이터에 액세스하십시오.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q60
솔루션 설계자는 여러 서브넷을 포함하는 VPC 아키텍처를 개발하고 있습니다. 이 아키텍처는 Amazon EC2 인스턴스와 Amazon RDS DB 인스턴스를 사용하는 애플리케이션을 호스팅 합니다. 아키텍처는 2개의 가용 영역에 있는 6개의 서브넷으로 구성됩니다. 각 가용 영역에는 퍼블릭 서브넷, 프라이빗 서브넷 및 데이터베이스 전용 서브넷이 포함됩니다. 프라이빗 서브넷에 서 실행되는 EC2 인스턴스만 RDS 데이터베이스에 액세스할 수 있습니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 퍼블릭 서브넷의 CIDR 블록에 대한 경로를 제외하는 새 경로 테이블을 만듭니다. 경로 테이블을 데이터베이스 서브넷과 연결합니다. 
B. 퍼블릭 서브넷의 인스턴스에 할당된 보안 그룹에서 인바운드 트래픽을 거부하는 보안 그룹을 생성합니다. 보안 그룹을 DB 인스턴스에 연결합니다. 
C. 프라이빗 서브넷의 인스턴스에 할당된 보안 그룹에서 인바운드 트래픽을 허용하는 보안 그룹을 생성합니다. 보안 그룹을 DB 인스턴스에 연결합니다. 
D. 퍼블릭 서브넷과 프라이빗 서브넷 간에 새 피어링 연결을 만듭니다. 프라이빗 서브넷과 데이터베이스 서브넷 간에 다른 피어링 연결을 만듭니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q61
회사에는 원치 않는 콘텐츠가 포함된 사진이 회사의 웹 애플리케이션에 업로드되는 것을 방지하는 솔루션이 필요합니다. 솔루션에는 기계 학습(ML) 모델 교육이 포함되어서는 안 됩니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon SageMaker Autopilot을 사용하여 모델을 생성하고 배포합니다. 새 사진이 업로드될 때 웹 애플리케이션이 호출하는 실시간 엔드포인트를 만듭니다. 
B. Amazon Rekognition을 사용하여 원치 않는 콘텐츠를 감지하는 AWS Lambda 함수를 생성합니다. 새 사진이 업로드될 때 웹 애플리케이션이 호출하는 Lambda 함수 URL을 생성
합니다.
C. Amazon Comprehend를 사용하여 원치 않는 콘텐츠를 감지하는 Amazon CloudFront 함수를 생성합니다. 기능을 웹 애플리케이션과 연결합니다. 
D. Amazon Rekognition Video를 사용하여 원치 않는 콘텐츠를 감지하는 AWS Lambda 함수를 생성합니다. 새 사진이 업로드될 때 웹 애플리케이션이 호출하는 Lambda 함수 URL
을 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q62
한 회사가 AWS에서 여러 Windows 워크로드를 실행합니다. 회사 직원은 두 개의 Amazon EC2 인스턴스에서 호스팅되는 Windows 파일 공유를 사용합니다. 파일 공유는 서로 간에 데 이터를 동기화하고 복제본을 유지합니다. 회사는 사용자가 현재 파일에 액세스하는 방식을 보존하는 가용성이 높고 내구성이 뛰어난 스토리지 솔루션을 원합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 모든 데이터를 Amazon S3로 마이그레이션합니다. 사용자가 파일에 액세스할 수 있도록 IAM 인증을 설정합니다. 
B. Amazon S3 파일 게이트웨이를 설정합니다. 기존 EC2 인스턴스에 S3 File Gateway를 탑재합니다. 
C. 다중 AZ 구성을 사용하여 파일 공유 환경을 Windows 파일 서버용 Amazon FSx로 확장합니다. 모든 데이터를 FSx for Windows File Server로 마이그레이션합니다. 
D. 다중 AZ 구성을 사용하여 파일 공유 환경을 Amazon Elastic File System(Amazon EFS)으로 확장합니다. 모든 데이터를 Amazon EFS로 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q63
한 회사는 AWS 클라우드에서 긴밀하게 결합된 고성능 컴퓨팅(HPC) 환경을 설계하고 있습니다. 이 회사는 네트워킹 및 스토리지를 위해 HPC 환경을 최적화하는 것을 목표로 합니다. 이러 한 요구 사항을 충족하는 솔루션 조합은 무엇입니까? (2개 선택)
A. AWS Global Accelerator에서 액셀러레이터를 생성합니다. 가속기에 대한 사용자 지정 라우팅을 구성합니다. 
B. Lustre 파일 시스템용 Amazon FSx를 생성합니다. 스크래치 스토리지로 파일 시스템을 구성합니다. 
C. Amazon CloudFront 배포판을 생성합니다. 뷰어 프로토콜 정책을 HTTP 및 HTTPS로 구성합니다. 
D. Amazon EC2 인스턴스를 시작합니다. EFA(Elastic Fabric Adapter)를 인스턴스에 연결합니다. 
E. 환경을 관리하기 위해 AWS Elastic Beanstalk 배포를 생성합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q64
한 회사가 AWS에서 실시간 데이터 수집 솔루션을 실행하고 있습니다. 이 솔루션은 최신 버전의 Amazon Managed Streaming for Apache Kafka(Amazon MSK)로 구성됩니다. 이 솔루션은 3개의 가용 영역에 걸쳐 프라이빗 서브넷의 VPC에 배포됩니다. 솔루션 설계자는 인터넷을 통해 공개적으로 사용할 수 있도록 데이터 수집 솔루션을 재설계해야 합니다. 전송 중인 데이터도 암호화되어야 합니다. 가장 효율적인 운영 효율성으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 기존 VPC에서 퍼블릭 서브넷을 구성합니다. 퍼블릭 서브넷에 MSK 클러스터를 배포합니다. 상호 TLS 인증을 활성화하려면 MSK 클러스터 보안 설정을 업데이트하세요. 
B. 퍼블릭 서브넷이 있는 새 VPC를 생성합니다. 퍼블릭 서브넷에 MSK 클러스터를 배포합니다. 상호 TLS 인증을 활성화하려면 MSK 클러스터 보안 설정을 업데이트하세요. 
C. 프라이빗 서브넷을 사용하는 ALB(Application Load Balancer)를 배포합니다. HTTPS 프로토콜에 대한 VPC CIDR 블록의 인바운드 트래픽을 허용하도록 ALB 보안 그룹 인바운
드 규칙을 구성합니다.
D. 프라이빗 서브넷을 사용하는 NLB(Network Load Balancer)를 배포합니다. 인터넷을 통한 HTTPS 통신을 위해 NLB 수신기를 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q65
한 회사는 데이터 센터에서 SMB 파일 서버를 운영하고 있습니다. 파일서버는 회사가 자주 접속하는 대용량 파일을 파일 생성일로부터 최대 7일까지 저장합니다. 7일이 지나면 회사는 최대 24시간의 검색 시간으로 파일에 액세스할 수 있어야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS DataSync를 사용하여 SMB 파일 서버에서 AWS로 7일보다 오래된 데이터를 복사합니다. 
B. 회사의 저장 공간을 늘리려면 Amazon S3 파일 게이트웨이를 생성하십시오. 7일 후에 데이터를 S3 Glacier Deep Archive로 전환하는 S3 수명 주기 정책을 생성합니다. 
C. 회사의 저장 공간을 늘리기 위해 Amazon FSx 파일 게이트웨이를 생성합니다. 7일 후에 데이터를 전환하는 Amazon S3 수명 주기 정책을 생성합니다. 
D. 각 사용자에 대해 Amazon S3에 대한 액세스를 구성합니다. 7일 후에 데이터를 S3 Glacier 유연한 검색으로 전환하는 S3 수명 주기 정책을 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q66
회사는 회사 데이터 센터의 대규모 NAS(Network-Attached Storage) 시스템에 700테라바이트의 데이터를 저장하고 있습니다. 이 회사는 10Gbps AWS Direct Connect 연결을 사 용하는 하이브리드 환경을 보유하고 있습니다. 규제 기관의 감사 후 회사는 90일 이내에 데이터를 클라우드로 옮길 수 있습니다. 회사는 데이터를 중단 없이 효율적으로 이동해야 합니다. 회사는 여전히 이전 기간 동안 데이터에 액세스하고 데이터를 업데이트할 수 있어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 회사 데이터 센터에서 AWS DataSync 에이전트를 생성합니다. 데이터 전송 작업 생성 Amazon S3 버킷으로의 전송을 시작합니다. 
B. 데이터를 AWS Snowball Edge Storage Optimized 디바이스에 백업합니다. 디바이스를 AWS 데이터 센터로 배송합니다. 온프레미스 파일 시스템에 대상 Amazon S3 버킷을 탑
재합니다.
C. rsync를 사용하여 Direct Connect 연결을 통해 로컬 스토리지에서 지정된 Amazon S3 버킷으로 데이터를 직접 복사합니다. 
D. 테이프에 데이터를 백업합니다. 테이프를 AWS 데이터 센터로 배송합니다. 온프레미스 파일 시스템에 대상 Amazon S3 버킷을 탑재합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q67
한 회사가 Amazon Route 53에 도메인 이름을 등록했습니다. 이 회사는 ca-central-1 리전의 Amazon API Gateway를 백엔드 마이크로서비스 API용 퍼블릭 인터페이스로 사용합니 다. 타사 서비스는 API를 안전하게 사용합니다. 회사는 타사 서비스가 HTTPS를 사용할 수 있도록 회사의 도메인 이름과 해당 인증서로 API 게이트웨이 URL을 설계하려고 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. API Gateway에서 Name="Endpoint-URL" 및 Value="Company Domain Name"으로 단계 변수를 생성하여 기본 URL을 덮어씁니다. 회사 도메인 이름과 연결된 공인 인증서
를 AWS Certificate Manager(ACM)로 가져옵니다.
B. 회사의 도메인 이름으로 Route 53 DNS 레코드를 생성합니다. 별칭 레코드가 지역 API 게이트웨이 단계 엔드포인트를 가리킵니다. 회사 도메인 이름과 연결된 공인 인증서를 us-east-
1 리전의 AWS Certificate Manager(ACM)로 가져옵니다.
C. 지역 API 게이트웨이 엔드포인트를 생성합니다. API Gateway 끝점을 회사의 도메인 이름과 연결합니다. 회사 도메인 이름과 연결된 공인 인증서를 동일한 리전의 AWS Certificate
Manager(ACM)로 가져옵니다. API Gateway 엔드포인트에 인증서를 연결합니다. 트래픽을 API 게이트웨이 엔드포인트로 라우팅하도록 Route 53을 구성합니다.
D. 지역 API 게이트웨이 엔드포인트를 생성합니다. API Gateway 끝점을 회사의 도메인 이름과 연결합니다. 회사 도메인 이름과 연결된 공인 인증서를 us-east-1 리전의 AWS
Certificate Manager(ACM)로 가져옵니다. API Gateway API에 인증서를 연결합니다. 회사의 도메인 이름으로 Route 53 DNS 레코드를 생성합니다. A 레코드가 회사의 도메인 이름을 가리킵니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q68
회사에는 AWS Organizations 조직의 일부로 5개의 조직 단위(OU)가 있습니다. 각 OU는 회사가 소유한 5개 비즈니스와 연관되어 있습니다. 회사의 연구개발(R&D) 사업이 회사에서 분 리되어 자체 조직이 필요할 것입니다. 솔루션 설계자는 이 목적을 위해 별도의 새 관리 계정을 생성합니다. 솔루션 설계자는 새 마스터 계정에서 다음에 무엇을 수행해야 합니까?
A. 전환하는 동안 R&D AWS 계정이 두 조직의 일부가 되도록 하십시오. 
B. R&D AWS 계정이 이전 조직을 떠난 후 R&D AWS 계정을 새 조직의 일부로 초대합니다. 
C. 새 조직에 새 R&D AWS 계정을 생성합니다. 이전 R&D AWS 계정의 리소스를 새 R&D AWS 계정으로 마이그레이션합니다. 
D. R&D AWS 계정이 새 조직에 가입하도록 합니다. 새 마스터 계정을 이전 조직의 구성원으로 만드세요.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q69
솔루션 설계자는 다음 JSON 텍스트를 자격 증명 기반 정책으로 사용하여 특정 권한을 부여하려고 합니다. 솔루션 설계자가 이 정책을 연결할 수 있는 IAM 보안 주체는 무엇입니까? (두 가지를 선택하세요.)
A. 역할
B. 그룹
C. 조직
D. Amazon Elastic Container Service(Amazon ECS) 리소스
E. Amazon EC2 리소스

<details>
<summary>정답 보기</summary>

**AB**
</details>

---

### Q70
회사는 Auto Scaling 그룹의 Application Load Balancer(ALB) 뒤에 있는 Amazon EC2 인스턴스에서 전자상거래 웹 사이트를 운영합니다. 사이트에서 IP 주소가 변경되는 불법 외부 시스템의 높은 요청 비율과 관련된 성능 문제가 발생하고 있습니다. 보안 팀은 웹 사이트에 대한 잠재적인 DDoS 공격에 대해 걱정하고 있습니다. 회사는 합법적인 사용자에게 최소한의 영향 을 미치는 방식으로 불법적으로 들어오는 요청을 차단해야 합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. Amazon Inspector를 배포하고 ALB와 연결합니다. 
B. AWS WAF를 배포하고 ALB와 연결하고 속도 제한 규칙을 구성합니다. 
C. 들어오는 트래픽을 차단하기 위해 ALB와 연결된 네트워크 ACL에 규칙을 배포합니다. 
D. Amazon GuardDuty를 배포하고 GuardDuty를 구성할 때 속도 제한 보호를 활성화합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q71
회사는 Application Load Balancer 뒤의 Amazon Linux Amazon EC2 인스턴스에서 다중 계층 웹 애플리케이션을 호스팅합니다. 인스턴스는 여러 가용 영역의 Auto Scaling 그룹 에서 실행됩니다. 이 회사는 애플리케이션의 최종 사용자가 대량의 정적 웹 콘텐츠에 액세스할 때 Auto Scaling 그룹이 더 많은 온디맨드 인스턴스를 시작하는 것을 관찰합니다. 회사는 비용 을 최적화하려고 합니다. 애플리케이션을 가장 비용 효율적으로 재설계하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. 온디맨드 인스턴스 대신 예약 인스턴스를 사용하도록 Auto Scaling 그룹을 업데이트합니다. 
B. 온디맨드 인스턴스 대신 스팟 인스턴스를 시작하여 조정하도록 Auto Scaling 그룹을 업데이트합니다. 
C. Amazon S3 버킷에서 정적 웹 콘텐츠를 호스팅할 Amazon CloudFront 배포를 만듭니다. 
D. Amazon API Gateway API 뒤에 AWS Lambda 함수를 생성하여 정적 웹 사이트 콘텐츠를 호스팅합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q72
한 회사에서 사용자가 작은 파일을 Amazon S3에 업로드하는 애플리케이션을 설계하고 있습니다. 사용자가 파일을 업로드한 후 파일은 나중에 분석할 수 있도록 데이터를 변환하고 데이터를 JSON 형식으로 저장하는 일회성 간단한 처리가 필요합니다. 각 파일은 업로드된 후 가능한 한 빨리 처리되어야 합니다. 수요는 다양할 것입니다. 어떤 날에는 사용자가 많은 수의 파일을 업로드합니다. 다른 날에는 사용자가 몇 개의 파일을 업로드하거나 파일을 전혀 업로드하지 않습니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon S3에서 텍스트 파일을 읽도록 Amazon EMR을 구성합니다. 처리 스크립트를 실행하여 데이터를 변환합니다. 결과 JSON 파일을 Amazon Aurora DB 클러스터에 저장합
니다.
B. 이벤트 알림을 Amazon Simple Queue Service(Amazon SQS) 대기열로 보내도록 Amazon S3를 구성합니다. Amazon EC2 인스턴스를 사용하여 대기열에서 읽고 데이터를
처리합니다. 결과 JSON 파일을 Amazon DynamoDB에 저장합니다.
C. 이벤트 알림을 Amazon Simple Queue Service(Amazon SQS) 대기열로 보내도록 Amazon S3를 구성합니다. AWS Lambda 함수를 사용하여 대기열에서 읽고 데이터를 처
리합니다. 결과 JSON 파일을 Amazon DynamoDB에 저장합니다.
D. 새 파일이 업로드되면 Amazon Kinesis Data Streams로 이벤트를 보내도록 Amazon EventBridge(Amazon CloudWatch Events)를 구성합니다. AWS Lambda 함수를
사용하여 스트림에서 이벤트를 소비하고 데이터를 처리합니다. 결과 JSON 파일을 Amazon Aurora DB 클러스터에 저장합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q73
회사는 월 단위로 통화 기록 파일을 저장합니다. 사용자는 통화 후 1년 이내에 임의로 파일에 액세스하지만 1년 후에는 드물게 파일에 액세스합니다. 이 회사는 사용자에게 1년 미만의 파일을 가능한 한 빨리 쿼리하고 검색할 수 있는 기능을 제공하여 솔루션을 최적화하려고 합니다. 이전 파일 검색 지연은 허용됩니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. Amazon S3 Glacier Instant Retrieval에 태그가 있는 개별 파일을 저장합니다. 태그를 쿼리하여 S3 Glacier Instant Retrieval에서 파일을 검색합니다. 
B. Amazon S3 Intelligent-Tiering에 개별 파일을 저장합니다. S3 수명 주기 정책을 사용하여 1년 후 파일을 S3 Glacier Flexible Retrieval로 이동합니다. Amazon Athena를 사
용하여 Amazon S3에 있는 파일을 쿼리하고 검색합니다. S3 Glacier Select를 사용하여 S3 Glacier에 있는 파일을 쿼리하고 검색합니다.
C. Amazon S3 Standard 스토리지에 태그가 있는 개별 파일을 저장합니다. Amazon S3 Standard 스토리지의 각 아카이브에 대한 검색 메타데이터를 저장합니다. S3 수명 주기 정책
을 사용하여 1년 후 파일을 S3 Glacier Instant Retrieval로 이동합니다. Amazon S3에서 메타데이터를 검색하여 파일을 쿼리하고 검색합니다.
D. Amazon S3 Standard 스토리지에 개별 파일을 저장합니다. S3 수명 주기 정책을 사용하여 1년 후 파일을 S3 Glacier Deep Archive로 이동합니다. Amazon RDS에 검색 메타
데이터를 저장합니다. Amazon RDS에서 파일을 쿼리합니다. S3 Glacier Deep Archive에서 파일을 검색합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q74
회사는 1Gbps AWS Direct Connect 연결 비용을 최소화해야 합니다. 회사의 평균 연결 사용률은 10% 미만입니다. 솔루션 설계자는 보안을 손상시키지 않으면서 비용을 절감할 솔루션을 추천해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 새로운 1Gbps Direct Connect 연결을 설정합니다. 다른 AWS 계정과 연결을 공유합니다. 
B. AWS Management Console에서 새로운 200Mbps Direct Connect 연결을 설정합니다. 
C. 1Gbps 연결을 주문하려면 AWS Direct Connect 파트너에게 문의하십시오. 다른 AWS 계정과 연결을 공유합니다. 
D. 기존 AWS 계정에 대한 200Mbps 호스팅 연결을 주문하려면 AWS Direct Connect 파트너에게 문의하십시오.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q75
한 회사가 AWS에서 웹 애플리케이션을 설계하고 있습니다. 애플리케이션은 회사의 기존 데이터 센터와 회사의 VPC 간의 VPN 연결을 사용합니다. 이 회사는 DNS 서비스로 Amazon Route 53을 사용합니다. 애플리케이션은 프라이빗 DNS 레코드를 사용하여 VPC에서 온프레미스 서비스와 통신해야 합니다. 가장 안전한 방식으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Route 53 Resolver 아웃바운드 엔드포인트를 생성합니다. 해석기 규칙을 만듭니다. 해석기 규칙을 VPC와 연결합니다. 
B. Route 53 Resolver 인바운드 엔드포인트를 생성합니다. 해석기 규칙을 만듭니다. 해석기 규칙을 VPC와 연결합니다. 
C. Route 53 프라이빗 호스팅 영역을 생성합니다. 프라이빗 호스팅 영역을 VPC와 연결합니다. 
D. Route 53 퍼블릭 호스팅 영역을 생성합니다. 서비스 통신을 허용하려면 각 서비스에 대한 레코드를 만듭니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q76
회사에서 Amazon EC2 인스턴스에 새 애플리케이션을 배포하고 있습니다. 애플리케이션은 Amazon Elastic Block Store(Amazon EBS) 볼륨에 데이터를 씁니다. 회사는 EBS 볼륨 에 기록된 모든 데이터가 유휴 상태에서 암호화되도록 해야 합니다. 이 요구 사항을 충족하는 솔루션은 무엇입니까?
A. EBS 암호화를 지정하는 IAM 역할을 생성합니다. 역할을 EC2 인스턴스에 연결합니다. 
B. EBS 볼륨을 암호화된 볼륨으로 생성합니다. EBS 볼륨을 EC2 인스턴스에 연결합니다. 
C. 키가 Encrypt이고 값이 True인 EC2 인스턴스 태그를 생성합니다. EBS 수준에서 암호화가 필요한 모든 인스턴스에 태그를 지정합니다. 
D. 계정에서 EBS 암호화를 시행하는 AWS Key Management Service(AWS KMS) 키 정책을 생성합니다. 키 정책이 활성 상태인지 확인하십시오.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q77
회사에서 전자상거래 애플리케이션을 구축 중이며 중요한 고객 정보를 저장해야 합니다. 회사는 고객이 웹사이트에서 구매 거래를 완료할 수 있는 기능을 제공해야 합니다. 회사는 또한 민감한 고객 데이터를 데이터베이스 관리자로부터 보호해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon Elastic Block Store(Amazon EBS) 볼륨에 민감한 데이터를 저장합니다. EBS 암호화를 사용하여 데이터를 암호화합니다. IAM 인스턴스 역할을 사용하여 액세스를 제한
합니다.
B. MySQL용 Amazon RDS에 민감한 데이터를 저장합니다. AWS Key Management Service(AWS KMS) 클라이언트 측 암호화를 사용하여 데이터를 암호화합니다.
C. 민감한 데이터를 Amazon S3에 저장합니다. AWS Key Management Service(AWS KMS) 서버 측 암호화를 사용하여 데이터를 암호화합니다. S3 버킷 정책을 사용하여 액세스
를 제한하십시오.
D. 민감한 데이터를 Windows Server용 Amazon FSx에 저장합니다. 응용 프로그램 서버에 파일 공유를 탑재합니다. Windows 파일 권한을 사용하여 액세스를 제한하십시오.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q78
한 회사는 회사의 온프레미스 데이터 센터에서 MySQL DB 인스턴스용 Amazon RDS로 MySQL 데이터베이스를 마이그레이션했습니다. 회사는 회사의 일일 평균 워크로드를 충족하도록 RDS DB 인스턴스의 크기를 조정했습니다. 한 달에 한 번 회사에서 보고서에 대한 쿼리를 실행할 때 데이터베이스 성능이 느려집니다. 회사는 보고서를 실행하고 일일 작업 부하의 성능을 유 지 관리할 수 있는 기능을 원합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 데이터베이스의 읽기 전용 복제본을 생성합니다. 쿼리를 읽기 전용 복제본으로 보냅니다. 
B. 데이터베이스 백업을 생성합니다. 백업을 다른 DB 인스턴스로 복원합니다. 쿼리를 새 데이터베이스로 보냅니다. 
C. 데이터를 Amazon S3로 내보냅니다. Amazon Athena를 사용하여 S3 버킷을 쿼리합니다. 
D. 추가 워크로드를 수용할 수 있도록 DB 인스턴스의 크기를 조정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q79
회사는 AWS에서 애플리케이션을 실행합니다. 애플리케이션이 일관되지 않은 사용량을 수신합니다. 애플리케이션은 AWS Direct Connect를 사용하여 온프레미스 MySQL 호환 데이터베 이스에 연결합니다. 온프레미스 데이터베이스는 지속적으로 최소 2GiB의 메모리를 사용합니다. 회사는 온프레미스 데이터베이스를 관리형 AWS 서비스로 마이그레이션하려고 합니다. 회사는 자동 확장 기능을 사용하여 예기치 않은 작업 부하 증가를 관리하려고 합니다. 최소한의 관리 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 기본 읽기 및 쓰기 용량 설정으로 Amazon DynamoDB 데이터베이스를 프로비저닝합니다. 
B. 최소 용량이 1 Aurora 용량 단위(ACU)인 Amazon Aurora 데이터베이스를 프로비저닝합니다. 
C. 최소 용량이 1 Aurora 용량 단위(ACU)인 Amazon Aurora Serverless v2 데이터베이스를 프로비저닝합니다. 
D. 2GiB의 메모리로 Amazon RDS for MySQL 데이터베이스를 프로비저닝합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q80
한 회사에서 Amazon Elastic Container Service(Amazon ECS) 클러스터와 Amazon RDS DB 인스턴스를 사용하여 결제 처리 애플리케이션을 구축하고 실행하려고 합니다. 회사 는 규정 준수를 위해 온프레미스 데이터 센터에서 애플리케이션을 실행합니다. 솔루션 아키텍트는 AWS Outposts를 솔루션의 일부로 사용하려고 합니다. 솔루션 설계자는 회사의 운영 팀과 협력하여 애플리케이션을 구축하고 있습니다. 회사 운영팀에서는 어떤 활동을 담당하나요? (3개를 선택하세요.)
A. Outposts 랙에 탄력적인 전원 및 네트워크 연결 제공
B. Outposts에서 실행되는 가상화 하이퍼바이저, 스토리지 시스템 및 AWS 서비스 관리
C. 데이터센터 환경의 물리적 보안 및 접근통제
D. Outposts 랙 내의 전원 공급 장치, 서버 및 네트워킹 장비를 포함한 Outposts 인프라의 가용성
E. Outposts 구성 요소의 물리적 유지 관리
F. 서버 오류 및 유지 관리 이벤트를 완화하기 위해 Amazon ECS 클러스터에 추가 용량 제공

<details>
<summary>정답 보기</summary>

**ACE**
</details>

---

### Q81
회사에 새로운 모바일 앱이 있습니다. 세계 어디에서나 사용자는 자신이 선택한 주제에 대한 지역 뉴스를 볼 수 있습니다. 사용자는 앱 내부에서 사진과 비디오를 게시할 수도 있습니다. 사용자 는 콘텐츠가 게시된 후 처음 몇 분 안에 콘텐츠에 액세스하는 경우가 많습니다. 새로운 콘텐츠가 이전 콘텐츠를 빠르게 대체한 다음 이전 콘텐츠는 사라집니다. 뉴스의 지역적 특성은 사용자가 뉴스가 업로드되는 AWS 지역 내에서 콘텐츠의 90%를 소비한다는 것을 의미합니다. 콘텐츠 업로드에 가장 짧은 지연 시간을 제공하여 사용자 경험을 최적화하는 솔루션은 무엇입니까?
A. Amazon S3에 콘텐츠를 업로드하고 저장합니다. 업로드에는 Amazon CloudFront를 사용하십시오. 
B. Amazon S3에 콘텐츠를 업로드하고 저장합니다. 업로드에는 S3 Transfer Acceleration을 사용하십시오. 
C. 사용자에게 가장 가까운 지역의 Amazon EC2 인스턴스에 콘텐츠를 업로드합니다. 데이터를 Amazon S3에 복사합니다. 
D. 사용자에게 가장 가까운 지역의 Amazon S3에 콘텐츠를 업로드하고 저장합니다. Amazon CloudFront의 여러 배포판을 사용하십시오.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q82
회사에는 1,000개의 Amazon EC2 Linux 인스턴스에서 실행되는 프로덕션 워크로드가 있습니다. 워크로드는 타사 소프트웨어로 구동됩니다. 회사는 중요한 보안 취약성을 수정하기 위해 가능한 한 빨리 모든 EC2 인스턴스에서 타사 소프트웨어를 패치해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 모든 EC2 인스턴스에 패치를 적용할 AWS Lambda 함수를 생성합니다. 
B. 모든 EC2 인스턴스에 패치를 적용하도록 AWS Systems Manager Patch Manager를 구성합니다. 
C. 모든 EC2 인스턴스에 패치를 적용하도록 AWS Systems Manager 유지 관리 기간을 예약합니다. 
D. AWS Systems Manager Run Command를 사용하여 패치를 모든 EC2 인스턴스에 적용하는 사용자 지정 명령을 실행합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q83
조사 회사는 미국 지역에서 몇 년 동안 데이터를 수집했습니다. 회사는 크기가 3TB이고 계속 증가하는 Amazon S3 버킷에서 데이터를 호스팅합니다. 회사는 S3 버킷을 보유한 유럽 마케팅 회사와 데이터를 공유하기 시작했습니다. 회사는 데이터 전송 비용이 가능한 한 낮게 유지되기를 원합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 회사의 S3 버킷에서 요청자 지불 기능을 구성합니다. 
B. 회사의 S3 버킷에서 마케팅 회사의 S3 버킷 중 하나로 S3 교차 리전 복제를 구성합니다. 
C. 마케팅 회사가 회사의 S3 버킷에 액세스할 수 있도록 마케팅 회사에 대한 교차 계정 액세스를 구성합니다. 
D. S3 Intelligent-Tiering을 사용하도록 회사의 S3 버킷을 구성합니다. 마케팅 회사의 S3 버킷 중 하나에 S3 버킷을 동기화합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q84
회사에는 VPC의 Amazon EC2 인스턴스에서 실행되는 애플리케이션이 있습니다. 애플리케이션 중 하나는 Amazon S3 API를 호출하여 객체를 저장하고 읽어야 합니다. 회사의 보안 정 책은 애플리케이션에서 인터넷에 연결된 모든 트래픽을 제한합니다. 이러한 요구 사항을 충족하고 보안을 유지하는 조치는 무엇입니까?
A. S3 인터페이스 엔드포인트를 구성합니다. 
B. S3 게이트웨이 엔드포인트를 구성합니다. 
C. 프라이빗 서브넷에 S3 버킷을 생성합니다. 
D. EC2 인스턴스와 동일한 지역에 S3 버킷을 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q85
한 회사에서 인기 있는 소셜 미디어 웹사이트를 운영하고 있습니다. 웹사이트는 사용자에게 이미지를 업로드하여 다른 사용자와 공유할 수 있는 기능을 제공합니다. 회사는 이미지에 부적절한 콘텐츠가 포함되어 있지 않은지 확인하려고 합니다. 회사는 개발 노력을 최소화하는 솔루션이 필요합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Amazon Comprehend를 사용하여 부적절한 콘텐츠를 감지합니다. 신뢰도가 낮은 예측에는 사람의 검토를 사용하세요. 
B. Amazon Rekognition을 사용하여 부적절한 콘텐츠를 감지합니다. 신뢰도가 낮은 예측에는 사람의 검토를 사용하세요. 
C. Amazon SageMaker를 사용하여 부적절한 콘텐츠를 감지합니다. 신뢰도가 낮은 예측에 라벨을 지정하려면 Ground Truth를 사용하세요. 
D. AWS Fargate를 사용하여 사용자 지정 기계 학습 모델을 배포하여 부적절한 콘텐츠를 탐지합니다. 신뢰도가 낮은 예측에 라벨을 지정하려면 Ground Truth를 사용하세요.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q86
회사는 AWS 클라우드에서 애플리케이션을 호스팅합니다. 이 애플리케이션은 Amazon DynamoDB 테이블과 함께 Auto Scaling 그룹의 Elastic Load Balancer 뒤에 있는 Amazon EC2 인스턴스에서 실행됩니다. 회사는 다운타임을 최소화하면서 다른 AWS 리전에서 애플리케이션을 사용할 수 있기를 원합니다. 가동 중지 시간을 최소화하면서 이러한 요구 사항을 충족하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 재해 복구 지역에 Auto Scaling 그룹과 로드 밸런서를 생성합니다. DynamoDB 테이블을 전역 테이블로 구성합니다. 새 재해 복구 리전의 로드 밸런서를 가리키도록 DNS 장애 조치를
구성합니다.
B. 필요할 때 시작할 EC2 인스턴스, 로드 밸런서 및 DynamoDB 테이블을 생성하기 위해 AWS CloudFormation 템플릿을 생성합니다. 새 재해 복구 리전의 로드 밸런서를 가리키도록
DNS 장애 조치를 구성합니다.
C. AWS CloudFormation 템플릿을 생성하여 EC2 인스턴스와 필요할 때 실행할 로드 밸런서를 생성합니다. DynamoDB 테이블을 전역 테이블로 구성합니다. 새 재해 복구 리전의 로
드 밸런서를 가리키도록 DNS 장애 조치를 구성합니다.
D. 재해 복구 지역에서 Auto Scaling 그룹 및 로드 밸런서를 생성합니다. DynamoDB 테이블을 전역 테이블로 구성합니다. 재해 복구 로드 밸런서를 가리키는 Amazon Route 53을 업
데이트하는 AWS Lambda 함수를 트리거하는 Amazon CloudWatch 경보를 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q87
회사의 웹사이트는 대중에게 제품을 판매하는 데 사용됩니다. 이 사이트는 ALB(Application Load Balancer) 뒤에 있는 Auto Scaling 그룹의 Amazon EC2 인스턴스에서 실행됩니다. Amazon CloudFront 배포판도 있으며 AWS WAF는 SQL 주입 공격으로부터 보호하는 데 사용되고 있습니다. ALB는 CloudFront 배포의 오리진입니다. 최근 보안 로그를 검토한 결과 , 해당 웹사이트에 대한 접근을 차단해야 할 외부 악성 IP가 발견되었습니다. 솔루션 설계자는 애플리케이션을 보호하기 위해 무엇을 해야 합니까?
A. CloudFront 배포의 네트워크 ACL을 수정하여 악성 IP 주소에 대한 거부 규칙을 추가합니다.
B. AWS WAF 구성을 수정하여 악성 IP 주소를 차단하는 IP 일치 조건을 추가합니다.
C. ALB 뒤의 대상 그룹에 있는 EC2 인스턴스에 대한 네트워크 ACL을 수정하여 악성 IP 주소를 거부합니다.
D. 악성 IP 주소를 거부하도록 ALB 뒤의 대상 그룹에 있는 EC2 인스턴스에 대한 보안 그룹을 수정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q88
한 회사에서 AI(인공 지능)를 사용하여 고객 서비스 통화 품질을 확인하려고 합니다. 회사는 현재 영어를 포함하여 4개 언어로 통화를 관리합니다. 회사는 앞으로 새로운 언어를 제공할 것입니 다. 회사는 기계 학습(ML) 모델을 정기적으로 유지 관리할 리소스가 없습니다. 회사는 고객 서비스 통화 녹음에서 서면 감정 분석 보고서를 작성해야 합니다. 고객 서비스 통화 녹음 텍스트는 영어로 번역되어야 합니다. 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (3개를 선택하세요.)
A. Amazon Comprehend를 사용하여 오디오 녹음을 영어로 번역하십시오.
B. Amazon Lex를 사용하여 작성된 감정 분석 보고서를 생성합니다.
C. Amazon Polly를 사용하여 오디오 녹음을 텍스트로 변환합니다.
D. Amazon Transcribe를 사용하여 모든 언어의 오디오 녹음을 텍스트로 변환합니다.
E. Amazon Translate를 사용하여 모든 언어의 텍스트를 영어로 번역합니다.
F. Amazon Comprehend를 사용하여 감정 분석 보고서를 생성합니다.

<details>
<summary>정답 보기</summary>

**DEF**
</details>

---

### Q89
한 회사에서 여러 Microsoft Windows Server 워크로드를 us-west-1 리전에서 실행되는 Amazon EC2 인스턴스로 마이그레이션했습니다. 회사는 필요에 따라 이미지를 생성하기 위해 워크로드를 수동으로 백업합니다. us-west-1 리전에서 자연 재해가 발생한 경우 회사는 us-west-2 리전에서 워크로드를 신속하게 복구하기를 원합니다. 회사는 EC2 인스턴스에서 24시간 이상의 데이터 손실을 원하지 않습 니다. 회사는 또한 EC2 인스턴스의 모든 백업을 자동화하려고 합니다. 최소한의 관리 노력으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까? (두 가지를 선택하세요.)
A. Amazon EC2 지원 Amazon 머신 이미지(AMI) 수명 주기 정책을 생성하여 태그 기반 백업을 생성합니다. 하루에 두 번 실행되도록 백업을 예약합니다. 필요에 따라 이미지를 복사합니
다.
B. Amazon EC2 지원 Amazon 머신 이미지(AMI) 수명 주기 정책을 생성하여 태그 기반 백업을 생성합니다. 하루에 두 번 실행되도록 백업을 예약합니다. us-west-2 리전에 대한 복사
본을 구성합니다.
C. AWS Backup을 사용하여 us-west-1 및 us-west-2에 백업 볼트를 생성합니다. 태그 값을 기반으로 EC2 인스턴스에 대한 백업 계획을 생성합니다. 백업 데이터를 us-west-2에 복
사하기 위해 예약된 작업으로 실행할 AWS Lambda 함수를 생성합니다.
D. AWS Backup을 사용하여 백업 볼트를 생성합니다. AWS Backup을 사용하여 태그 값을 기반으로 EC2 인스턴스에 대한 백업 계획을 생성합니다. 사본의 대상을 us-west-2로 정의
합니다. 하루에 두 번 실행할 백업 일정을 지정합니다.
E. AWS Backup을 사용하여 백업 볼트를 생성합니다. AWS Backup을 사용하여 태그 값을 기반으로 EC2 인스턴스에 대한 백업 계획을 생성합니다. 하루에 두 번 실행할 백업 일정을
지정합니다. 요청 시 us-west-2에 복사합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q90
보안 감사 결과 Amazon EC2 인스턴스가 정기적으로 패치되지 않는 것으로 나타났습니다. 솔루션 설계자는 대규모 EC2 인스턴스 전체에 대해 정기적인 보안 스캔을 실행할 솔루션을 제공 해야 합니다. 또한 솔루션은 정기적으로 EC2 인스턴스를 패치하고 각 인스턴스의 패치 상태에 대한 보고서를 제공해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. EC2 인스턴스에서 소프트웨어 취약성을 스캔하도록 Amazon Macie를 설정합니다. 각 EC2 인스턴스에서 cron 작업을 설정하여 정기적인 일정에 따라 인스턴스를 패치합니다. 
B. 계정에서 Amazon GuardDuty를 켭니다. 소프트웨어 취약성에 대해 EC2 인스턴스를 스캔하도록 GuardDuty를 구성합니다. 정기적인 일정에 따라 EC2 인스턴스를 패치하도록
AWS Systems Manager Session Manager를 설정합니다.
C. 소프트웨어 취약성에 대해 EC2 인스턴스를 스캔하도록 Amazon Detective를 설정합니다. 정기적인 일정에 따라 EC2 인스턴스를 패치하도록 Amazon EventBridge 예약 규칙을
설정합니다.
D. 계정에서 Amazon Inspector를 켭니다. 소프트웨어 취약성에 대해 EC2 인스턴스를 스캔하도록 Amazon Inspector를 구성합니다. 정기적인 일정에 따라 EC2 인스턴스를 패치하도
록 AWS Systems Manager Patch Manager를 설정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q91
회사에 여행 발권을 위한 웹 애플리케이션이 있습니다. 이 애플리케이션은 북미 지역의 단일 데이터 센터에서 실행되는 데이터베이스를 기반으로 합니다. 회사는 글로벌 사용자 기반에 서비스 를 제공하기 위해 응용 프로그램을 확장하려고 합니다. 회사는 애플리케이션을 여러 AWS 리전에 배포해야 합니다. 예약 데이터베이스 업데이트 시 평균 대기 시간은 1초 미만이어야 합니다. 이 회사는 여러 지역에 걸쳐 웹 플랫폼을 별도로 배포하려고 합니다. 그러나 회사는 전 세계적으로 일관된 단일 기본 예약 데이터베이스를 유지해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 어떤 솔루션을 권장해야 합니까?
A. Amazon DynamoDB를 사용하도록 애플리케이션을 변환합니다. 중앙 예약 테이블에 전역 테이블을 사용합니다. 각 지역 배포에서 올바른 지역 엔드포인트를 사용합니다. 
B. 데이터베이스를 Amazon Aurora MySQL 데이터베이스로 마이그레이션합니다. 각 지역에 Aurora 읽기 전용 복제본을 배포합니다. 데이터베이스에 액세스하려면 각 지역 배포에서 올
바른 지역 엔드포인트를 사용하세요.
C. 데이터베이스를 Amazon RDS for MySQL 데이터베이스로 마이그레이션합니다. 각 리전에 MySQL 읽기 전용 복제본을 배포합니다. 데이터베이스에 액세스하려면 각 지역 배포에서
올바른 지역 엔드포인트를 사용하세요.
D. 애플리케이션을 Amazon Aurora Serverless 데이터베이스로 마이그레이션합니다. 각 지역에 데이터베이스 인스턴스를 배포합니다. 각 지역 배포에서 올바른 지역 엔드포인트를 사용
하여 데이터베이스에 액세스합니다. AWS Lambda 함수를 사용하여 각 리전에서 이벤트 스트림을 처리하여 데이터베이스를 동기화합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q92
회사에 보고서를 생성하는 재무 응용 프로그램이 있습니다. 보고서 크기는 평균 50KB이며 Amazon S3에 저장됩니다. 보고서는 생산 후 첫 주 동안 자주 액세스되며 몇 년 동안 저장해야 합 니다. 보고서는 6시간 이내에 검색할 수 있어야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. S3 Standard를 사용합니다. S3 수명 주기 규칙을 사용하여 7일 후에 보고서를 S3 Glacier로 전환합니다.
B. S3 Standard를 사용합니다. S3 수명 주기 규칙을 사용하여 7일 후에 보고서를 S3 Standard-Infrequent Access(S3 Standard-IA)로 전환합니다.
C. S3 Intelligent-Tiering을 사용합니다. 보고서를 S3 Standard-Infrequent Access(S3 Standard-IA) 및 S3 Glacier로 전환하도록 S3 Intelligent-Tiering을 구성합니다.
D. S3 Standard를 사용합니다. S3 수명 주기 규칙을 사용하여 7일 후에 보고서를 S3 Glacier Deep Archive로 전환합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q93
회사는 서로 다른 위치에 데이터 수집 센서를 가지고 있습니다. 데이터 수집 센서는 대량의 데이터를 회사로 스트리(cid:1535)합니다. 이 회사는 대용량 스트리(cid:1535) 데이터를 수집하고 처리하기 위해 AWS에서 플랫폼을 설계하려고 합니다. 솔루션은 확장 가능해야 하며 거의 실시간으로 데이터 수집을 지원해야 합니다. 회사는 향후 보고를 위해 데이터를 Amazon S3에 저장해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Kinesis Data Firehose를 사용하여 스트리(cid:1535) 데이터를 Amazon S3에 전달합니다. 
B. AWS Glue를 사용하여 스트리(cid:1535) 데이터를 Amazon S3에 전달합니다. 
C. AWS Lambda를 사용하여 스트리(cid:1535) 데이터를 전달하고 데이터를 Amazon S3에 저장합니다. 
D. AWS DMS(AWS Database Migration Service)를 사용하여 스트리(cid:1535) 데이터를 Amazon S3에 전달합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q94
AWS 클라우드에 호스팅된 한 회사의 웹 애플리케이션은 최근 인기를 얻었지만 증가하는 트래픽을 처리하는 데 어려움을 겪고 있습니다. 애플리케이션은 현재 퍼블릭 서브넷 내의 단일 Amazon EC2 인스턴스에 있습니다. 이 문제를 해결하기 위해 회사는 애플리케이션을 다시 작성할 필요 없이 고가용성과 확장성을 갖춘 솔루션을 찾고 있습니다. 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (2개를 선택하세요.)
A. EC2 인스턴스를 더 큰 컴퓨팅 최적화 인스턴스로 교체하십시오. 
B. 프라이빗 서브넷의 여러 가용 영역으로 Amazon EC2 Auto Scaling을 구성합니다. 
C. 웹 요청을 처리하기 위해 퍼블릭 서브넷에 NAT 게이트웨이를 구성합니다. 
D. EC2 인스턴스를 더 큰 메모리 최적화 인스턴스로 교체합니다. 
E. 웹 트래픽을 분산시키기 위해 퍼블릭 서브넷에 Application Load Balancer를 구성합니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q95
한 회사가 AWS에서 2계층 웹 애플리케이션을 개발하고 있습니다. 이 회사의 개발자는 백엔드 Amazon RDS 데이터베이스에 직접 연결되는 Amazon EC2 인스턴스에 애플리케이션을 배포했습니다. 회사는 애플리케이션에 데이터베이스 자격 증명을 하드코딩해서는 안 됩니다. 또한 회사는 정기적으로 데이터베이스 자격 증명을 자동으로 교체하는 솔루션을 구현해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 인스턴스 메타데이터에 데이터베이스 자격 증명을 저장합니다. Amazon EventBridge(Amazon CloudWatch Events) 규칙을 사용하여 RDS 자격 증명과 인스턴스 메타데이터를
동시에 업데이트하는 예약된 AWS Lambda 함수를 실행합니다.
B. 암호화된 Amazon S3 버킷의 구성 파일에 데이터베이스 자격 증명을 저장합니다. Amazon EventBridge(Amazon CloudWatch Events) 규칙을 사용하여 RDS 자격 증명과 구
성 파일의 자격 증명을 동시에 업데이트하는 예약된 AWS Lambda 함수를 실행합니다. S3 버전 관리를 사용하여 이전 값으로 폴백할 수 있습니다.
C. 데이터베이스 자격 증명을 AWS Secrets Manager에 비밀로 저장합니다. 보안 비밀에 대해 자동 회전을 켭니다. 암호에 대한 액세스 권한을 부여하려면 EC2 역할에 필요한 권한을 연
결합니다.
D. 데이터베이스 자격 증명을 AWS Systems Manager Parameter Store에 암호화된 파라미터로 저장합니다. 암호화된 매개변수에 대해 자동 회전을 켭니다. 암호화된 매개변수에 대
한 액세스 권한을 부여하려면 필요한 권한을 EC2 역할에 연결하십시오.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q96
회사는 사용자를 비용 센터에 매핑하는 Amazon RDS 데이터베이스를 유지 관리합니다. 회사는 AWS Organizations의 조직에 계정을 가지고 있습니다. 회사에는 조직의 특정 AWS 계 정에서 생성된 모든 리소스에 태그를 지정하는 솔루션이 필요합니다. 솔루션은 리소스를 생성한 사용자의 비용 센터 ID로 각 리소스에 태그를 지정해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 특정 AWS 계정을 마스터 계정에서 조직의 새로운 조직 단위(OU)로 이동합니다. 리소스가 생성되기 전에 모든 기존 리소스에 올바른 비용 센터 태그가 있어야 하는 서비스 제어 정책
(SCP)을 생성합니다. 새 OU에 SCP를 적용합니다.
B. Lambda 함수가 RDS 데이터베이스에서 적절한 비용 센터를 조회한 후 리소스에 태그를 지정하는 AWS Lambda 함수를 생성합니다. AWS CloudTrail 이벤트에 반응하여
Lambda 함수를 호출하는 Amazon EventBridge 규칙을 구성합니다.
C. AWS CloudFormation 스택을 생성하여 AWS Lambda 함수를 배포합니다. RDS 데이터베이스에서 적절한 비용 센터를 조회하고 리소스에 태그를 지정하도록 Lambda 함수를 구
성합니다. CloudFormation 스택을 호출하는 Amazon EventBridge 예약 규칙을 생성합니다.
D. 기본값으로 리소스에 태그를 지정하는 AWS Lambda 함수를 생성합니다. 리소스에 비용 센터 태그가 누락된 경우 AWS CloudTrail 이벤트에 반응하여 Lambda 함수를 호출하는
Amazon EventBridge 규칙을 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q97
회사의 웹 사이트는 항목 카탈로그에 Amazon EC2 인스턴스 스토어를 사용합니다. 회사는 카탈로그의 가용성이 높고 카탈로그가 안정적인 위치에 저장되기를 원합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Redis용 Amazon ElastiCache로 카탈로그를 이동합니다. 
B. 더 큰 인스턴스 저장소가 있는 더 큰 EC2 인스턴스를 배포합니다. 
C. 인스턴스 스토어에서 Amazon S3 Glacier Deep Archive로 카탈로그를 이동합니다. 
D. 카탈로그를 Amazon Elastic File System(Amazon EFS) 파일 시스템으로 이동합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q98
한 회사가 AWS Fargate 클러스터를 사용하여 Amazon Elastic Kubernetes Service(Amazon EKS)에 새 애플리케이션을 배포하고 있습니다. 애플리케이션에는 데이터 지속성을 위 한 스토리지 솔루션이 필요합니다. 솔루션은 가용성이 높고 내결함성이 있어야 합니다. 또한 솔루션은 여러 애플리케이션 컨테이너 간에 공유되어야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. EKS 작업자 노드가 배치된 동일한 가용 영역에 Amazon Elastic Block Store(Amazon EBS) 볼륨을 생성합니다. EKS 클러스터의 StorageClass 객체에 볼륨을 등록합니다.
EBS 다중 연결을 사용하여 컨테이너 간에 데이터를 공유합니다.
B. Amazon Elastic File System(Amazon EFS) 파일 시스템을 생성합니다. EKS 클러스터의 StorageClass 객체에 파일 시스템을 등록합니다. 모든 컨테이너에 동일한 파일 시스
템을 사용합니다.
C. Amazon Elastic Block Store(Amazon EBS) 볼륨을 생성합니다. EKS 클러스터의 StorageClass 객체에 볼륨을 등록합니다. 모든 용기에 동일한 용량을 사용하십시오. 
D. EKS 작업자 노드가 배치된 동일한 가용 영역에 Amazon Elastic File System(Amazon EFS) 파일 시스템을 생성합니다. EKS 클러스터의 StorageClass 객체에 파일 시스템을
등록합니다. 파일 시스템 간에 데이터를 동기화하는 AWS Lambda 함수를 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q99
회사는 NFS를 사용하여 온프레미스 네트워크 연결 스토리지에 대용량 비디오 파일을 저장합니다. 각 비디오 파일의 크기는 1MB에서 500GB까지입니다. 총 스토리지는 70TB이며 더 이상 증가하지 않습니다. 회사는 비디오 파일을 Amazon S3로 마이그레이션하기로 결정합니다. 회사는 최소한의 네트워크 대역폭을 사용하면서 가능한 한 빨리 비디오 파일을 마이그레이션해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. S3 버킷을 생성합니다. S3 버킷에 쓸 수 있는 권한이 있는 IAM 역할을 생성합니다. AWS CLI를 사용하여 모든 파일을 S3 버킷에 로컬로 복사합니다. 
B. AWS Snowball Edge 작업을 생성합니다. 온프레미스에서 Snowball Edge 디바이스를 받습니다. Snowball Edge 클라이언트를 사용하여 데이터를 디바이스로 전송합니다. AWS
가 데이터를 Amazon S3로 가져올 수 있도록 장치를 반환하십시오.
C. 온프레미스에 S3 파일 게이트웨이를 배포합니다. S3 파일 게이트웨이에 연결할 공용 서비스 엔드포인트를 생성합니다. S3 버킷을 생성합니다. S3 File Gateway에서 새 NFS 파일 공
유를 생성합니다. 새 파일 공유가 S3 버킷을 가리키도록 합니다. 기존 NFS 파일 공유에서 S3 파일 게이트웨이로 데이터를 전송합니다.
D. 온프레미스 네트워크와 AWS 간에 AWS Direct Connect 연결을 설정합니다. 온프레미스에 S3 파일 게이트웨이를 배포합니다. S3 파일 게이트웨이에 연결할 퍼블릭 가상 인터페이스
(VIF)를 생성합니다. S3 버킷을 생성합니다. S3 File Gateway에서 새 NFS 파일 공유를 생성합니다. 새 파일 공유가 S3 버킷을 가리키도록 합니다. 기존 NFS 파일 공유에서 S3 파 일 게이트웨이로 데이터를 전송합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q100
회사에는 온프레미스 파일 시스템이 SFTP를 통해 매일 수신하는 보고서 파일을 분석하는 야간 일괄 처리 루틴이 있습니다. 회사는 솔루션을 AWS 클라우드로 이전하려고 합니다. 솔루션은 가용성과 복원력이 높아야 합니다. 또한 솔루션은 운영 노력을 최소화해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. SFTP용 AWS 전송 및 스토리지용 Amazon Elastic File System(Amazon EFS) 파일 시스템을 배포합니다. 예약된 조정 정책이 있는 Auto Scaling 그룹의 Amazon EC2 인
스턴스를 사용하여 배치 작업을 실행합니다.
B. Linux 및 SFTP 서비스를 실행하는 Amazon EC2 인스턴스를 배포합니다. 저장에는 Amazon Elastic Block Store(Amazon EBS) 볼륨을 사용하십시오. 최소 인스턴스 수와 원
하는 인스턴스 수를 1로 설정한 Auto Scaling 그룹을 사용합니다.
C. Linux 및 SFTP 서비스를 실행하는 Amazon EC2 인스턴스를 배포합니다. 저장을 위해 Amazon Elastic File System(Amazon EFS) 파일 시스템을 사용합니다. 최소 인스턴스
수와 원하는 인스턴스 수를 1로 설정한 Auto Scaling 그룹을 사용합니다.
D. SFTP용 AWS 전송과 저장용 Amazon S3 버킷을 배포합니다. 처리를 위해 Amazon S3에서 Amazon EC2 인스턴스로 배치 파일을 가져오도록 애플리케이션을 수정합니다. 예약
된 조정 정책이 있는 Auto Scaling 그룹의 EC2 인스턴스를 사용하여 일괄 작업을 실행합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q101
한 회사는 동시성이 높은 AWS Lambda 함수를 사용하여 마케팅 이벤트 중에 메시지 대기열에서 지속적으로 증가하는 메시지 수를 처리합니다. Lambda 함수는 CPU 집약적인 코드를 사 용하여 메시지를 처리합니다. 회사는 컴퓨팅 비용을 줄이고 고객의 서비스 대기 시간을 유지하기를 원합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Lambda 함수에 대해 예약된 동시성을 구성합니다. Lambda 함수에 할당된 메모리를 줄입니다. 
B. Lambda 함수에 대한 예약된 동시성을 구성합니다. AWS Compute Optimizer 권장 사항에 따라 메모리를 늘리십시오. 
C. Lambda 함수에 대해 프로비저닝된 동시성을 구성합니다. Lambda 함수에 할당된 메모리를 줄입니다. 
D. Lambda 함수에 대해 프로비저닝된 동시성을 구성합니다. AWS Compute Optimizer 권장 사항에 따라 메모리를 늘리십시오.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q102
한 회사에서 대량의 데이터를 병렬로 처리하는 애플리케이션을 배포하고 있습니다. 회사는 워크로드에 Amazon EC2 인스턴스를 사용할 계획입니다. 노드 그룹이 동일한 기본 하드웨어를 공 유하지 못하도록 네트워크 아키텍처를 구성할 수 있어야 합니다. 이러한 요구 사항을 충족하는 네트워킹 솔루션은 무엇입니까?
A. 분산 배치 그룹에서 EC2 인스턴스를 실행합니다. 
B. EC2 인스턴스를 별도의 계정으로 그룹화합니다. 
C. 전용 테넌시로 EC2 인스턴스를 구성합니다. 
D. 공유 테넌시로 EC2 인스턴스를 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q103
한 회사는 AWS 클라우드에서 실험적인 워크로드를 실행할 계획이며 클라우드 지출에 예산을 할당했습니다. 회사의 CFO는 각 부서의 지출 책임을 추적하는 데 관심이 있으며 지출이 예산의 60%에 도달하면 알림을 받기를 원합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS 리소스의 비용 할당 태그를 사용하여 소유자에게 레이블을 지정합니다. AWS 예산에서 사용 예산을 생성합니다. 지출이 예산의 60%를 초과할 때 알림을 받도록 경고 임계값을 설
정합니다.
B. AWS Cost Explorer 예측을 사용하여 리소스 소유자를 결정합니다. 지출이 예산의 60%를 초과하면 AWS 비용 이상 탐지를 활용하여 경고 알림을 생성합니다. 
C. AWS 리소스에 대한 비용 할당 태그를 사용하여 리소스 소유자에게 레이블을 지정합니다. 지출이 예산의 60%를 초과할 때 경고 알림을 생성하려면 AWS Trusted Advisor 내에서
AWS Support API를 사용하십시오.
D. AWS Cost Explorer 예측을 사용하여 리소스 소유자를 결정합니다. AWS 예산에서 사용 예산을 설정하고 지출이 예산의 60%를 초과할 때 알림을 받도록 경고 임계값을 설정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q104
회사는 대상 그룹이 있는 Auto Scaling 그룹의 Amazon EC2 인스턴스에서 웹 애플리케이션을 실행합니다. 회사는 더 나은 사용자 경험을 위해 세션 선호도(고정 세션)와 함께 작동하도록 애플리케이션을 설계했습니다. 애플리케이션은 인터넷을 통해 공개적으로 엔드포인트로 사용할 수 있어야 합니다. 추가 보안을 위해 엔드포인트에 WAF를 적용해야 합니다. 세션 선호도(고정 세션)는 엔드포인트에서 구성 되어야 합니다. 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (2개를 선택하세요.)
A. 공용 Network Load Balancer를 생성합니다. 적용 대상 그룹을 지정합니다.
B. 게이트웨이 로드 밸런서를 생성합니다. 적용 대상 그룹을 지정합니다.
C. 공개 Application Load Balancer를 생성합니다. 적용 대상 그룹을 지정합니다.
D. 두 번째 대상 그룹을 생성합니다. EC2 인스턴스에 탄력적 IP 주소를 추가합니다.
E. AWS WAF에서 웹 ACL을 생성합니다. 웹 ACL을 엔드포인트와 연결합니다.

<details>
<summary>정답 보기</summary>

**CE**
</details>

---

### Q105
소셜 미디어 회사는 ALB(Application Load Balancer) 뒤의 Amazon EC2 인스턴스에서 애플리케이션을 실행합니다. ALB는 Amazon CloudFront 배포의 오리진입니다. 이 애플리 케이션은 Amazon S3 버킷에 10억 개 이상의 이미지가 저장되어 있으며 초당 수천 개의 이미지를 처리합니다. 회사는 이미지 크기를 동적으로 조정하고 고객에게 적절한 형식을 제공하기를 원합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. EC2 인스턴스에 외부 이미지 관리 라이브러리를 설치합니다. 이미지 관리 라이브러리를 사용하여 이미지를 처리합니다. 
B. CloudFront 오리진 요청 정책을 생성합니다. 정책을 사용하여 자동으로 이미지 크기를 조정하고 요청의 User-Agent HTTP 헤더를 기반으로 적절한 형식을 제공합니다. 
C. 외부 이미지 관리 라이브러리와 함께 Lambda@Edge 함수를 사용합니다 . Lambda@Edge 함수를 이미지를 제공하는 CloudFront 동작과 연결합니다 . 
D. CloudFront 응답 헤더 정책을 생성합니다. 정책을 사용하여 자동으로 이미지 크기를 조정하고 요청의 User-Agent HTTP 헤더를 기반으로 적절한 형식을 제공합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q106
전자상거래 회사에서 계절별 온라인 세일을 진행하고 있습니다. 이 회사는 여러 가용 영역에 걸쳐 있는 Amazon EC2 인스턴스에서 웹 사이트를 호스팅합니다. 회사는 자사 웹사이트에서 세 일 기간 동안 급격한 트래픽 증가를 관리할 수 있기를 원합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 최대 트래픽 로드를 처리할 수 있을 만큼 큰 Auto Scaling 그룹을 생성합니다. Amazon EC2 인스턴스의 절반을 중지합니다. 트래픽이 증가하면 중지된 인스턴스를 사용하여 확장하도
록 Auto Scaling 그룹을 구성합니다.
B. 웹 사이트에 대한 Auto Scaling 그룹을 생성합니다. 확장할 필요 없이 높은 트래픽 볼륨을 처리할 수 있도록 Auto Scaling 그룹의 최소 크기를 설정합니다. 
C. Amazon CloudFront 및 Amazon ElastiCache를 사용하여 Auto Scaling 그룹이 원본으로 설정된 동적 콘텐츠를 캐시합니다. CloudFront 및 ElastiCache를 채우는 데 필요한
인스턴스로 Auto Scaling 그룹을 구성합니다. 캐시가 완전히 채워진 후 규모를 축소합니다.
D. 트래픽 증가에 따라 확장되도록 Auto Scaling 그룹을 구성합니다. 사전 구성된 Amazon 머신 이미지(AMI)에서 새 인스턴스를 시작하기 위한 시작 템플릿을 생성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q107
회사에는 각각 크기가 약 5MB인 많은 수의 파일을 생성하는 응용 프로그램이 있습니다. 파일은 Amazon S3에 저장됩니다. 회사 정책에 따라 파일은 삭제되기 전에 4년 동안 저장되어야 합 니다. 파일에는 재현하기 어려운 중요한 비즈니스 데이터가 포함되어 있으므로 즉각적인 액세스 가능성이 항상 필요합니다. 파일은 개체 생성 후 처음 30일 동안 자주 액세스되지만 처음 30일 이후에는 거의 액세스되지 않습니다. 가장 비용 효율적인 스토리지 솔루션은 무엇입니까?
A. 객체 생성 30일 후에 S3 Standard에서 S3 Glacier로 파일을 이동하는 S3 버킷 수명 주기 정책을 생성합니다. 객체 생성 후 4년이 지나면 파일을 삭제하십시오. 
B. S3 Standard에서 S3 One Zone-Infrequent Access(S3 One Zone-IA)로 객체 생성 30일 후에 파일을 이동하는 S3 버킷 수명 주기 정책을 생성합니다. 객체 생성 후 4년이 지
나면 파일을 삭제하십시오.
C. 객체 생성 30일 후에 S3 Standard에서 S3 Standard-Infrequent Access(S3 Standard-IA)로 파일을 이동하는 S3 버킷 수명 주기 정책을 생성합니다. 객체 생성 후 4년이 지나
면 파일을 삭제하십시오.
D. 객체 생성 30일 후에 S3 Standard에서 S3 Standard-Infrequent Access(S3 Standard-IA)로 파일을 이동하는 S3 버킷 수명 주기 정책을 생성합니다. 객체 생성 4년 후 파일을
S3 Glacier로 이동합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q108
글로벌 마케팅 회사에는 ap-southeast-2 지역 및 eu-west-1 지역에서 실행되는 애플리케이션이 있습니다. eu-west-1의 VPC에서 실행되는 애플리케이션은 ap-southeast-2의 VPC 에서 실행되는 데이터베이스와 안전하게 통신해야 합니다. 이러한 요구 사항을 충족하는 네트워크 설계는 무엇입니까?
A. eu-west-1 VPC와 ap-southeast-2 VPC 간에 VPC 피어링 연결을 생성합니다. ap-southeast-2 보안 그룹의 데이터베이스 서버 IP 주소에서 오는 트래픽을 허용하는 인바운드 규
칙을 eu-west-1 애플리케이션 보안 그룹에 생성합니다.
B. ap-southeast-2 VPC와 eu-west-1 VPC 간에 VPC 피어링 연결을 구성합니다. 서브넷 경로 테이블을 업데이트합니다. eu-west-1에 있는 애플리케이션 서버의 보안 그룹 ID를 참
조하는 ap-southeast-2 데이터베이스 보안 그룹에서 인바운드 규칙을 생성합니다.
C. ap-southeast-2 VPC와 eu-west-1 VPC 간에 VPC 피어링 연결을 구성합니다. 서브넷 경로 테이블을 업데이트합니다. ap-southeast-2 데이터베이스 보안 그룹에서 eu-west-1
애플리케이션 서버 IP 주소의 트래픽을 허용하는 인바운드 규칙을 생성합니다.
D. eu-west-1 VPC와 ap-southeast-2 VPC 간에 피어링 연결이 있는 전송 게이트웨이를 생성합니다. 전송 게이트웨이가 올바르게 피어링되고 라우팅이 구성되면 eu-west-1에 있는 애
플리케이션 서버의 보안 그룹 ID를 참조하는 데이터베이스 보안 그룹에 인바운드 규칙을 생성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q109
보안 요구 사항을 충족하려면 회사는 Amazon RDS MySQL DB 인스턴스와 통신하는 동안 전송 중인 모든 애플리케이션 데이터를 암호화해야 합니다. 최근 보안 감사에서는 AWS Key Management Service(AWS KMS)를 사용하여 저장 데이터 암호화가 활성화되어 있지만 전송 중인 데이터는 활성화되지 않은 것으로 나타났습니다. 솔루션 설계자는 보안 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 데이터베이스에서 IAM 데이터베이스 인증을 활성화합니다. 
B. 자체 서명된 인증서를 제공합니다. RDS 인스턴스에 대한 모든 연결에 인증서를 사용하십시오. 
C. RDS 인스턴스의 스냅샷을 찍습니다. 암호화가 활성화된 새 인스턴스로 스냅샷을 복원합니다. 
D. AWS에서 제공하는 루트 인증서를 다운로드합니다. RDS 인스턴스에 대한 모든 연결에 인증서를 제공하십시오.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q110
회사는 자사의 애플리케이션을 Amazon EC2 인스턴스에서 실행합니다. 회사는 주기적으로 AWS 비용을 평가하고 있으며, 최근에 이상한 지출을 발견했습니다. 회사는 이상한 지출을 방지 할 솔루션이 필요하며, 비정상적인 지출이 발생한 경우 해당 이해 관계자에게 알림을 보내야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족시킬까요?
A. AWS 예산 템플릿을 사용하여 제로 지출 예산을 생성합니다.
B. AWS 비용 및 비용 관리 콘솔에서 AWS 비용 이상 탐지 모니터를 생성합니다.
C. 현재 실행 중인 워크로드 가격 세부 정보를 위해 AWS 가격 계산기 견적을 생성합니다.
D. 비용을 모니터링하고 이상한 지출을 식별하기 위해 Amazon CloudWatch를 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q111
회사의 도메인 이름 레코드를 호스팅하는 DNS 공급자가 AWS에서 실행되는 웹 사이트의 서비스 중단을 초래하는 중단을 겪고 있습니다. 회사는 보다 탄력적인 관리형 DNS 서비스로 마이 그레이션해야 하며 해당 서비스가 AWS에서 실행되기를 원합니다. DNS 호스팅 서비스를 신속하게 마이그레이션하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 도메인 이름에 대한 Amazon Route 53 퍼블릭 호스팅 영역을 생성합니다. 이전 공급자가 호스팅하는 도메인 레코드가 포함된 영역 파일을 가져옵니다.
B. 도메인 이름에 대한 Amazon Route 53 프라이빗 호스팅 영역을 생성합니다. 이전 공급자가 호스팅하는 도메인 레코드가 포함된 영역 파일을 가져옵니다.
C. AWS에서 Simple AD 디렉터리를 생성합니다. 도메인 레코드에 대해 DNS 공급자와 Microsoft Active Directory용 AWS Directory Service 간의 영역 전송을 활성화합니다.
D. VPC에 Amazon Route 53 Resolver 인바운드 엔드포인트를 생성합니다. 공급자의 DNS가 DNS 쿼리를 전달할 IP 주소를 지정합니다. 도메인에 대한 DNS 쿼리를 인바운드 엔드
포인트에 지정된 IP 주소로 전달하도록 공급자의 DNS를 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q112
한 회사가 최근 애플리케이션 마이그레이션 이니셔티브를 지원하기 위해 AWS MSP(Managed Service Provider) 파트너와 계약을 체결했습니다. 솔루션 설계자는 기존 AWS 계정의 Amazon Machine Image(AMI)를 MSP 파트너의 AWS 계정과 공유해야 합니다. AMI는 Amazon Elastic Block Store(Amazon EBS)에서 지원하며 AWS Key Management Service(AWS KMS) 고객 관리형 키를 사용하여 EBS 볼륨 스냅샷을 암호화합니다. 솔루션 설계자가 AMI를 MSP 파트너의 AWS 계정과 공유할 수 있는 가장 안전한 방법은 무엇입니까?
A. 암호화된 AMI와 스냅샷을 공개적으로 사용 가능하게 만드십시오. MSP 파트너의 AWS 계정이 키를 사용할 수 있도록 키 정책을 수정합니다. 
B. AMI의 launchPermission 속성을 수정합니다. MSP 파트너의 AWS 계정과만 AMI를 공유합니다. MSP 파트너의 AWS 계정이 키를 사용할 수 있도록 키 정책을 수정합니다. 
C. AMI의 launchPermission 속성을 수정합니다. MSP 파트너의 AWS 계정과만 AMI를 공유합니다. 암호화를 위해 MSP 파트너가 소유한 새 KMS 키를 신뢰하도록 키 정책을 수정합
니다.
D. 소스 계정에서 MSP 파트너의 AWS 계정에 있는 Amazon S3 버킷으로 AMI를 내보내고 MSP 파트너가 소유한 새 KMS 키로 S3 버킷을 암호화합니다. MSP 파트너의 AWS 계정
에서 AMI를 복사하고 시작합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q113
한 회사에 AWS에서 호스팅되는 웹사이트가 있습니다. 웹사이트는 HTTP와 HTTPS를 별도로 처리하도록 구성된 ALB(Application Load Balancer) 뒤에 있습니다. 회사는 요청이 HTTPS를 사용하도록 모든 요청을 웹 사이트로 전달하려고 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. HTTPS 트래픽만 허용하도록 ALB의 네트워크 ACL을 업데이트합니다. 
B. URL의 HTTP를 HTTPS로 바꾸는 규칙을 만듭니다. 
C. ALB에서 리스너 규칙을 생성하여 HTTP 트래픽을 HTTPS로 리디렉션합니다. 
D. ALB를 SNI(Server Name Indication)를 사용하도록 구성된 Network Load Balancer로 교체합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q114
서버리스 애플리케이션은 Amazon API Gateway, AWS Lambda 및 Amazon DynamoDB를 사용합니다. Lambda 함수에는 DynamoDB 테이블을 읽고 쓸 수 있는 권한이 필요합 니다. DynamoDB 테이블에 대한 Lambda 함수 액세스를 가장 안전하게 제공하는 솔루션은 무엇입니까?
A. Lambda 함수에 프로그래(cid:1535) 방식으로 액세스할 수 있는 IAM 사용자를 생성합니다. DynamoDB 테이블에 대한 읽기 및 쓰기 액세스를 허용하는 정책을 사용자에게 연결합니다.
access_key_id 및 secret_access_key 파라미터를 Lambda 환경 변수의 일부로 저장합니다. 다른 AWS 사용자에게 Lambda 함수 구성에 대한 읽기 및 쓰기 액세스 권한이 없는 지 확인하십시오.
B. Lambda를 신뢰할 수 있는 서비스로 포함하는 IAM 역할을 생성합니다. DynamoDB 테이블에 대한 읽기 및 쓰기 액세스를 허용하는 역할에 정책을 연결합니다. 새 역할을 실행 역할로
사용하도록 Lambda 함수의 구성을 업데이트합니다.
C. Lambda 함수에 프로그래(cid:1535) 방식으로 액세스할 수 있는 IAM 사용자를 생성합니다. DynamoDB 테이블에 대한 읽기 및 쓰기 액세스를 허용하는 정책을 사용자에게 연결합니다. AWS
Systems Manager Parameter Store에 access_key_id 및 secret_access_key 파라미터를 보안 문자열 파라미터로 저장합니다. DynamoDB 테이블에 연결하기 전에 보안 문자열 파라미터를 검색하도록 Lambda 함수 코드를 업데이트합니다.
D. DynamoDB를 신뢰할 수 있는 서비스로 포함하는 IAM 역할을 생성합니다. Lambda 함수에서 읽기 및 쓰기 액세스를 허용하는 역할에 정책을 연결합니다. 새 역할에 실행 역할로 연결
되도록 Lambda 함수의 코드를 업데이트합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q115
회사는 1주일 동안 지속되는 예정된 이벤트를 위해 특정 AWS 리전에 있는 3개의 특정 가용 영역에서 보장된 Amazon EC2 용량이 필요합니다. 회사는 EC2 용량을 보장하기 위해 무엇을 해야 합니까?
A. 필요한 리전을 지정하는 예약 인스턴스를 구매합니다. 
B. 필요한 리전을 지정하는 온디맨드 용량 예약을 생성합니다. 
C. 필요한 리전과 3개의 가용 영역을 지정하는 예약 인스턴스를 구입합니다. 
D. 필요한 리전 및 세 개의 가용 영역을 지정하는 온디맨드 용량 예약을 생성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q116
한 회사는 승인된 콘텐츠 개발자가 비디오를 업로드할 수 있도록 전 세계적으로 주문형 교육 비디오를 제공하는 애플리케이션을 운영하고 있습니다. 데이터는 us-east-2 리전의 Amazon S3 버킷에 저장됩니다. 이 회사는 eu-west-2 및 ap-southeast-1 지역에 S3 버킷을 생성했으며 개발자와 학생 모두의 지연 시간을 최소화하면서 이러한 새 버킷에 데이터를 복제하는 것을 목표로 합니다. 애플리케이션을 가장 적게 변경하여 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (2개를 선택하세요.)
A. us-east-2 S3 버킷에서 eu-west-2 S3 버킷으로 단방향 복제를 구성합니다. us-east-2 S3 버킷에서 ap-southeast-1 S3 버킷으로의 단방향 복제를 구성합니다. 
B. us-east-2 S3 버킷에서 eu-west-2 S3 버킷으로 단방향 복제를 구성합니다. eu-west-2 S3 버킷에서 ap-southeast-1 S3 버킷으로의 단방향 복제를 구성합니다. 
C. 세 지역 모두에 있는 S3 버킷 간에 양방향(양방향) 복제를 구성합니다. 
D. S3 다중 지역 액세스 포인트를 생성합니다. 비디오 스트리(cid:1535)을 위해 다중 지역 액세스 포인트의 Amazon 리소스 이름(ARN)을 사용하도록 애플리케이션을 수정합니다. 비디오 업로드용
애플리케이션을 수정하지 마십시오.
E. S3 다중 지역 액세스 포인트를 생성합니다. 비디오 스트리(cid:1535) 및 업로드를 위해 다중 지역 액세스 포인트의 Amazon 리소스 이름(ARN)을 사용하도록 애플리케이션을 수정합니다.

<details>
<summary>정답 보기</summary>

**AE**
</details>

---

### Q117
회사는 온프레미스 NAS(Network Attached Storage) 시스템을 사용하여 HPC(고성능 컴퓨팅) 워크로드에 파일 공유를 제공합니다. 회사는 지연 시간에 민감한 HPC 워크로드와 스토리 지를 AWS 클라우드로 마이그레이션하려고 합니다. 회사는 파일 시스템에서 NFS 및 SMB 다중 프로토콜 액세스를 제공할 수 있어야 합니다. 가장 짧은 대기 시간으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까? (2개를 선택하세요.)
A. 컴퓨팅 최적화 EC2 인스턴스를 클러스터 배치 그룹에 배포합니다.
B. 컴퓨팅 최적화 EC2 인스턴스를 파티션 배치 그룹에 배포합니다.
C. EC2 인스턴스를 Amazon FSx for Lustre 파일 시스템에 연결합니다.
D. EC2 인스턴스를 Amazon FSx for OpenZFS 파일 시스템에 연결합니다.
E. EC2 인스턴스를 NetApp ONTAP 파일 시스템용 Amazon FSx에 연결합니다.

<details>
<summary>정답 보기</summary>

**AE**
</details>

---

### Q118
회사에는 Amazon API Gateway에서 호출하는 AWS Lambda 함수에서 실행되는 상태 비저장 웹 애플리케이션이 있습니다. 회사는 지역 장애 조치 기능을 제공하기 위해 여러 AWS 지 역에 애플리케이션을 배포하려고 합니다. 트래픽을 여러 지역으로 라우팅하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 각 지역에 대해 Amazon Route 53 상태 확인을 생성합니다. 활성-활성 장애 조치 구성을 사용합니다.
B. 각 리전의 오리진을 사용하여 Amazon CloudFront 배포를 생성합니다. CloudFront 상태 확인을 사용하여 트래픽을 라우팅합니다.
C. 전송 게이트웨이를 생성합니다. Transit Gateway를 각 리전의 API Gateway 엔드포인트에 연결합니다. 요청을 라우팅하도록 전송 게이트웨이를 구성합니다.
D. 기본 지역에서 Application Load Balancer를 생성합니다. 각 리전의 API 게이트웨이 엔드포인트 호스트 이름을 가리키도록 대상 그룹을 설정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q119
회사는 회사의 Amazon RDS 데이터베이스에 연결되는 애플리케이션을 AWS에서 실행합니다. 애플리케이션은 주말과 연중 피크 시간대에 확장됩니다. 회사는 데이터베이스에 연결하는 애 플리케이션에 대해 데이터베이스를 보다 효과적으로 확장하려고 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 데이터베이스에 대한 대상 그룹 구성과 함께 연결 풀링과 함께 Amazon DynamoDB를 사용하십시오. DynamoDB 엔드포인트를 사용하도록 애플리케이션을 변경합니다. 
B. 데이터베이스의 대상 그룹과 함께 Amazon RDS Proxy를 사용하십시오. RDS Proxy 엔드포인트를 사용하도록 애플리케이션을 변경합니다. 
C. Amazon EC2에서 실행되는 사용자 지정 프록시를 데이터베이스의 중개자로 사용합니다. 사용자 정의 프록시 엔드포인트를 사용하도록 애플리케이션을 변경하십시오. 
D. AWS Lambda 함수를 사용하여 데이터베이스에 대한 대상 그룹 구성과 함께 연결 풀링을 제공합니다. Lambda 함수를 사용하도록 애플리케이션을 변경합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q120
회사는 ALB(Application Load Balancer)를 사용하여 애플리케이션을 온라인에 선보입니다. 최근 회사는 애플리케이션 전체에서 불규칙한 트래픽 패턴을 발견했습니다. 이러한 이상 현상 을 더 잘 이해하려면 솔루션 설계자가 인프라 가시성을 효율적으로 향상해야 합니다. 이러한 요구 사항을 충족하는 데 운영상 가장 효율적인 솔루션은 무엇입니까?
A. Amazon Athena에서 AWS CloudTrail 로그용 테이블을 생성합니다. 관련 정보를 추출하는 쿼리를 개발합니다. 
B. Amazon S3에 대한 ALB 액세스 로깅을 활성화합니다. Amazon Athena에서 테이블을 설정하고 로그를 쿼리합니다. 
C. Amazon S3에 대한 ALB 액세스 로깅을 활성화합니다. 텍스트 편집기에서 각 파일을 수동으로 검사하고 관련 정보를 검색합니다. 
D. 전용 Amazon EC2 인스턴스에서 Amazon EMR을 활용하여 ALB에 트래픽 액세스 로그 정보를 직접 쿼리합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q121
한 회사는 맞춤형 보고서 작성 프로그램을 사용하여 주로 매월 마지막 주에 수행되는 모바일 앱 사용을 추적하는 보고서를 효율적으로 생성하는 것을 목표로 합니다. 프로그램의 생성 프로세스 는 각 보고서당 10분 미만이 소요될 정도로 신속합니다. 이 기간 외에는 자주 사용되지 않는 회사는 요청 시 신속한 보고서 생성을 위한 비용 효율적인 솔루션을 찾고 있습니다. 이러한 요구 사항을 가장 잘 충족하는 솔루션은 무엇입니까?
A. Amazon EC2 온디맨드 인스턴스를 사용하여 프로그램을 실행하십시오. 보고서가 요청될 때 EC2 인스턴스를 트리거하는 Amazon EventBridge 규칙을 설정합니다. 매월 마지막 주
에만 EC2 인스턴스를 지속적으로 운영합니다.
B. AWS Lambda를 사용하여 프로그램을 실행합니다. 보고서가 요청되면 Lambda 함수를 트리거하는 Amazon EventBridge 규칙을 생성합니다. 
C. Amazon Elastic Container Service(Amazon ECS) 내에서 프로그램을 운영하고 보고서 요청 시 실행되도록 예약합니다. 
D. Amazon EC2 스팟 인스턴스를 활용하여 프로그램을 실행합니다. 보고서가 요청되면 EC2 인스턴스를 시작하는 Amazon EventBridge 규칙을 생성합니다. 매월 마지막 주 동안
EC2 인스턴스를 지속적으로 실행하도록 유지합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q122
한 회사가 Amazon EC2 인스턴스에서 실행되는 애플리케이션을 단일 가용 영역에서 호스팅하고 있습니다. 이 애플리케이션은 Open Systems Interconnection (OSI) 모델의 전송 계 층을 사용하여 접근할 수 있습니다. 회사는 이 애플리케이션 아키텍처가 높은 가용성을 갖도록해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 조합은 다음 중 어느 것입니까? (두 가지 선택)
A. 다른 가용 영역에서 새로운 EC2 인스턴스를 구성합니다. Amazon Route 53을 사용하여 모든 인스턴스로 트래픽을 라우팅합니다.
B. EC2 인스턴스 앞에 Network Load Balancer (NLB)를 구성합니다.
C. 인스턴스로의 TCP 트래픽을 위해 Network Load Balancer를 구성하고, HTTP 및 HTTPS 트래픽을 위해 인스턴스로의 트래픽을 Application Load Balancer에 구성합니다.
D. EC2 인스턴스를 위한 Auto Scaling 그룹을 생성하고, 여러 가용 영역을 사용하도록 Auto Scaling 그룹을 구성하고, 인스턴스에서 애플리케이션 상태 확인을 실행하도록 구성합니다.
E. Amazon CloudWatch 경고를 생성하고, 중지 상태로 전환된 EC2 인스턴스를 다시 시작하도록 경고를 구성합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q123
회사는 MySQL 데이터베이스로 구동되는 온프레미스 애플리케이션을 실행합니다. 회사는 애플리케이션의 탄력성과 가용성을 높이기 위해 애플리케이션을 AWS로 마이그레이션하고 있습니 다. 현재 아키텍처는 정상 작동 시간 동안 데이터베이스에서 과도한 읽기 활동을 보여줍니다. 회사의 개발 팀은 4시간마다 프로덕션 데이터베이스의 전체 내보내기를 가져와 스테이징 환경에서 데 이터베이스를 채웁니다. 이 기간 동안 사용자는 허용할 수 없는 애플리케이션 대기 시간을 경험합니다. 개발팀은 절차가 완료될 때까지 스테이징 환경을 사용할 수 없습니다. 솔루션 설계자는 애플리케이션 대기 시간 문제를 완화하는 대체 아키텍처를 권장해야 합니다. 대체 아키텍처는 또한 개발 팀이 스테이징 환경을 지체 없이 계속 사용할 수 있는 기능을 제공해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 프로덕션을 위해 다중 AZ Aurora 복제본과 함께 Amazon Aurora MySQL을 사용하십시오. mysqldump 유틸리티를 사용하는 백업 및 복원 프로세스를 구현하여 스테이징 데이터베
이스를 채웁니다.
B. 프로덕션을 위해 다중 AZ Aurora 복제본과 함께 Amazon Aurora MySQL을 사용합니다. 데이터베이스 복제를 사용하여 필요에 따라 스테이징 데이터베이스를 생성합니다.
C. 다중 AZ 배포와 함께 Amazon RDS for MySQL을 사용하고 프로덕션용 읽기 전용 복제본을 사용합니다. 스테이징 데이터베이스에 대기 인스턴스를 사용하십시오.
D. 다중 AZ 배포와 함께 Amazon RDS for MySQL을 사용하고 프로덕션용 읽기 전용 복제본을 사용합니다. mysqldump 유틸리티를 사용하는 백업 및 복원 프로세스를 구현하여 스테
이징 데이터베이스를 채웁니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q124
회사에서 AWS에 새로운 퍼블릭 웹 애플리케이션을 배포하고 있습니다. 애플리케이션은 ALB(Application Load Balancer) 뒤에서 실행됩니다. 외부 인증 기관(CA)에서 발급한 SSL/ TLS 인증서를 사용하여 에지에서 애플리케이션을 암호화해야 합니다. 인증서는 만료되기 전에 매년 교체해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS Certificate Manager(ACM)를 사용하여 SSL/TLS 인증서를 발급합니다. ALB에 인증서를 적용합니다. 관리형 갱신 기능을 사용하여 인증서를 자동으로 교체하십시오. 
B. AWS Certificate Manager(ACM)를 사용하여 SSL/TLS 인증서를 발급합니다. 인증서에서 키 자료를 가져옵니다. 인증서를 AL에 적용관리형 갱신 기능을 사용하여 인증서를 자동
으로 교체하십시오.
C. AWS Certificate Manager(ACM) 사설 인증 기관을 사용하여 루트 CA에서 SSL/TLS 인증서를 발급합니다. ALB에 인증서를 적용합니다. 관리형 갱신 기능을 사용하여 인증서를
자동으로 교체하십시오.
D. AWS Certificate Manager(ACM)를 사용하여 SSL/TLS 인증서를 가져옵니다. ALB에 인증서를 적용합니다. 인증서 만료가 가까워지면 Amazon EventBridge(Amazon
CloudWatch Events)를 사용하여 알림을 보냅니다. 인증서를 수동으로 교체하십시오.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q125
한 회사가 Amazon S3에서 데이터 레이크를 호스팅하고 있습니다. 데이터 레이크는 다양한 데이터 소스에서 Apache Parquet 형식으로 데이터를 수집합니다. 회사는 수집된 데이터를 준 비하기 위해 여러 변환 단계를 사용합니다. 이 단계에는 이상 항목 필터링, 데이터를 표준 날짜 및 시간 값으로 정규화, 분석을 위한 집계 생성이 포함됩니다. 회사는 변환된 데이터를 데이터 분 석가가 액세스하는 S3 버킷에 저장해야 합니다. 회사에는 코드가 필요하지 않은 데이터 변환을 위해 사전 구축된 솔루션이 필요합니다. 솔루션은 데이터 계보 및 데이터 프로파일링을 제공해야 합니다. 회사는 회사 전체의 직원과 데이터 변환 단계를 공유해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 데이터를 변환하도록 AWS Glue Studio 시각적 캔버스를 구성합니다. AWS Glue 작업을 사용하여 직원과 변환 단계를 공유하십시오. 
B. 데이터를 변환하도록 Amazon EMR Serverless를 구성합니다. EMR 서버리스 작업을 사용하여 전환 단계를 직원과 공유하세요. 
C. 데이터를 변환하도록 AWS Glue DataBrew를 구성합니다. DataBrew 레시피를 사용하여 직원들과 변환 단계를 공유하세요. 
D. 데이터용 Amazon Athena 테이블을 생성합니다. Athena SQL 쿼리를 작성하여 데이터를 변환합니다. Athena SQL 쿼리를 직원과 공유하세요.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q126
회사의 인프라는 단일 AWS 리전에 있는 Amazon EC2 인스턴스와 Amazon RDS DB 인스턴스로 구성됩니다. 회사는 별도의 리전에 데이터를 백업하려고 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Backup을 사용하여 EC2 백업과 RDS 백업을 별도의 리전에 복사합니다. 
B. Amazon Data Lifecycle Manager(Amazon DLM)를 사용하여 EC2 백업 및 RDS 백업을 별도의 리전에 복사합니다. 
C. EC2 인스턴스의 Amazon 머신 이미지(AMI)를 생성합니다. AMI를 별도의 리전에 복사합니다. 별도의 리전에서 RDS DB 인스턴스에 대한 읽기 전용 복제본을 생성합니다. 
D. Amazon Elastic Block Store(Amazon EBS) 스냅샷을 생성합니다. EBS 스냅샷을 별도의 리전에 복사합니다. RDS 스냅샷을 생성합니다. RDS 스냅샷을 Amazon S3로 내보
냅니다. S3 CRR(Cross-Region Replication)을 별도의 리전에 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q127
솔루션 아키텍트는 Amazon S3 버킷의 파일을 Amazon Elastic File System(Amazon EFS) 파일 시스템과 다른 S3 버킷으로 복사해야 합니다. 파일은 계속해서 복사되어야 합니다. 새 파일은 원본 S3 버킷에 지속적으로 추가됩니다. 복사된 파일은 원본 파일이 변경된 경우에만 덮어써야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 대상 S3 버킷과 EFS 파일 시스템 모두에 대한 AWS DataSync 위치를 생성합니다. 대상 S3 버킷 및 EFS 파일 시스템에 대한 작업을 생성합니다. 변경된 데이터만 전송하도록 전송
모드를 설정하세요.
B. AWS Lambda 함수를 생성합니다. 파일 시스템을 함수에 마운트합니다. Amazon S3에서 파일이 생성되고 변경될 때 함수를 호출하도록 S3 이벤트 알림을 설정합니다. 파일 시스템과
대상 S3 버킷에 파일을 복사하는 기능을 구성합니다.
C. 대상 S3 버킷과 EFS 파일 시스템 모두에 대한 AWS DataSync 위치를 생성합니다. 대상 S3 버킷 및 EFS 파일 시스템에 대한 작업을 생성합니다. 모든 데이터를 전송하려면 전송 모
드를 설정하세요.
D. 파일 시스템과 동일한 VPC에서 Amazon EC2 인스턴스를 시작합니다. 파일 시스템을 마운트합니다. 원본 S3 버킷에서 변경된 모든 객체를 대상 S3 버킷 및 탑재된 파일 시스템과 정
기적으로 동기화하는 스크립트를 만듭니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q128
회사는 회계 기록을 Amazon S3에 저장해야 합니다. 기록은 1년 동안 즉시 액세스할 수 있어야 하며 추가 9년 동안 보관해야 합니다. 관리 사용자 및 루트 사용자를 포함하여 회사의 그 누구 도 전체 10년 기간 동안 레코드를 삭제할 수 없습니다. 기록은 최대한 탄력적으로 저장해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 전체 10년 동안 S3 Glacier에 레코드를 저장합니다. 액세스 제어 정책을 사용하여 10년 동안 레코드 삭제를 거부합니다. 
B. S3 Intelligent-Tiering을 사용하여 레코드를 저장합니다. IAM 정책을 사용하여 레코드 삭제를 거부합니다. 10년 후 삭제를 허용하도록 IAM 정책을 변경합니다. 
C. S3 수명 주기 정책을 사용하여 1년 후 레코드를 S3 Standard에서 S3 Glacier Deep Archive로 전환합니다. 10년 동안 규정 준수 모드에서 S3 객체 잠금을 사용합니다. 
D. S3 수명 주기 정책을 사용하여 1년 후 레코드를 S3 Standard에서 S3 One Zone-Infrequent Access(S3 One Zone-IA)로 전환합니다. 10년 동안 거버넌스 모드에서 S3 객체
잠금을 사용합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q129
회사는 의료 애플리케이션의 데이터를 저장해야 합니다. 애플리케이션의 데이터는 자주 변경됩니다. 새로운 규정은 저장된 데이터의 모든 수준에서 감사 액세스를 요구합니다. 회사는 스토리지 용량이 부족한 온프레미스 인프라에서 애플리케이션을 호스팅합니다. 솔루션 설계자는 새로운 규정을 만족하면서 기존 데이터를 AWS로 안전하게 마이그레이션해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS DataSync를 사용하여 기존 데이터를 Amazon S3로 이동합니다. AWS CloudTrail을 사용하여 데이터 이벤트를 기록합니다. 
B. AWS Snowcone을 사용하여 기존 데이터를 Amazon S3로 이동합니다. AWS CloudTrail을 사용하여 관리 이벤트를 기록합니다. 
C. Amazon S3 Transfer Acceleration을 사용하여 기존 데이터를 Amazon S3로 이동합니다. AWS CloudTrail을 사용하여 데이터 이벤트를 기록합니다. 
D. AWS Storage Gateway를 사용하여 기존 데이터를 Amazon S3로 이동합니다. AWS CloudTrail을 사용하여 관리 이벤트를 기록합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q130
회사는 사용자 트랜잭션 데이터를 Amazon DynamoDB 테이블에 보관해야 합니다. 회사는 데이터를 7년간 보관해야 합니다. 이러한 요구 사항을 충족하는 운영상 가장 효율적인 솔루션은 무엇입니까?
A. DynamoDB point-in-time recovery를 사용하여 테이블을 지속적으로 백업하십시오. 
B. AWS Backup을 사용하여 테이블에 대한 백업 일정 및 보존 정책을 생성합니다. 
C. DynamoDB 콘솔을 사용하여 테이블의 온디맨드 백업을 생성합니다. Amazon S3 버킷에 백업을 저장합니다. S3 버킷에 대한 S3 수명 주기 구성을 설정합니다. 
D. AWS Lambda 함수를 호출하는 Amazon EventBridge(Amazon CloudWatch Events) 규칙을 생성합니다. 테이블을 백업하고 백업을 Amazon S3 버킷에 저장하도록
Lambda 함수를 구성합니다. S3 버킷에 대한 S3 수명 주기 구성을 설정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q131
회사에는 트랜잭션 데이터를 처리하는 온프레미스 MySQL 데이터베이스가 있습니다. 회사는 데이터베이스를 AWS 클라우드로 마이그레이션하고 있습니다. 마이그레이션된 데이터베이스는 데이터베이스를 사용하는 회사의 애플리케이션과 호환성을 유지해야 합니다. 마이그레이션된 데이터베이스는 또한 수요가 증가하는 기간 동안 자동으로 확장되어야 합니다. 이러한 요구 사항을 충족하는 마이그레이션 솔루션은 무엇입니까?
A. 기본 MySQL 도구를 사용하여 데이터베이스를 MySQL용 Amazon RDS로 마이그레이션합니다. 탄력적 스토리지 확장을 구성합니다. 
B. mysqldump 유틸리티를 사용하여 데이터베이스를 Amazon Redshift로 마이그레이션합니다. Amazon Redshift 클러스터에 대해 Auto Scaling을 켭니다. 
C. AWS Database Migration Service(AWS DMS)를 사용하여 데이터베이스를 Amazon Aurora로 마이그레이션합니다. Aurora Auto Scaling을 켭니다. 
D. AWS Database Migration Service(AWS DMS)를 사용하여 데이터베이스를 Amazon DynamoDB로 마이그레이션합니다. Auto Scaling 정책을 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q132
회사는 Amazon API Gateway API에 의해 호출되는 AWS Lambda 함수에서 애플리케이션을 호스팅합니다. Lambda 함수는 고객 데이터를 Amazon Aurora MySQL 데이터베이스 에 저장합니다. 회사에서 데이터베이스를 업그레이드할 때마다 Lambda 함수는 업그레이드가 완료될 때까지 데이터베이스 연결을 설정하지 못합니다. 그 결과 일부 이벤트에 대해 고객 데이 터가 기록되지 않습니다. 솔루션 설계자는 데이터베이스 업그레이드 중에 생성된 고객 데이터를 저장하는 솔루션을 설계해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Lambda 함수와 데이터베이스 사이에 위치하도록 Amazon RDS 프록시를 프로비저닝합니다. RDS 프록시에 연결하도록 Lambda 함수를 구성합니다. 
B. Lambda 함수의 실행 시간을 최대로 늘립니다. 데이터베이스에 고객 데이터를 저장하는 코드에서 재시도 메커니즘을 만듭니다. 
C. 고객 데이터를 Lambda 로컬 스토리지에 유지합니다. 고객 데이터를 데이터베이스에 저장하기 위해 로컬 스토리지를 스캔하도록 새로운 Lambda 함수를 구성합니다. 
D. 고객 데이터를 Amazon Simple Queue Service(Amazon SQS) FIFO 대기열에 저장합니다. 대기열을 폴링하고 고객 데이터를 데이터베이스에 저장하는 새 Lambda 함수를 생
성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q133
회사에 TCP 및 UDP 멀티플레이어 게임 기능이 있는 온라인 게임 응용 프로그램이 있습니다. 이 회사는 Amazon Route 53을 사용하여 애플리케이션 트래픽이 서로 다른 AWS 리전에 있 는 여러 NLB(Network Load Balancer)를 가리키도록 합니다. 회사는 사용자 증가에 대비하여 애플리케이션 성능을 개선하고 온라인 게임의 지연 시간을 줄여야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. NLB 앞에 Amazon CloudFront 배포를 추가합니다. Cache-Control max-age 매개변수를 늘리십시오. 
B. NLB를 ALB(Application Load Balancer)로 교체합니다. 지연 시간 기반 라우팅을 사용하도록 Route 53을 구성합니다. 
C. NLB 앞에 AWS Global Accelerator를 추가합니다. 올바른 수신기 포트를 사용하도록 Global Accelerator 끝점을 구성합니다. 
D. NLB 뒤에 Amazon API Gateway 엔드포인트를 추가합니다. API 캐싱을 활성화합니다. 다른 단계에 대한 메서드 캐싱을 재정의합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q134
이미지 처리 회사에는 사용자가 이미지를 업로드하는 데 사용하는 웹 애플리케이션이 있습니다. 애플리케이션은 이미지를 Amazon S3 버킷에 업로드합니다. 회사는 객체 생성 이벤트를 Amazon Simple Queue Service(Amazon SQS) 표준 대기열에 게시하도록 S3 이벤트 알림을 설정했습니다. SQS 대기열은 이미지를 처리하고 이메일을 통해 사용자에게 결과를 보 내는 AWS Lambda 함수의 이벤트 소스 역할을 합니다. 사용자는 업로드된 모든 이미지에 대해 여러 개의 이메일 메시지를 받고 있다고 보고합니다. 솔루션 아키텍트는 SQS 메시지가 Lambda 함수를 두 번 이상 호출하여 여러 이메일 메시지가 생 성되었음을 확인합니다. 최소한의 운영 오버헤드로 이 문제를 해결하려면 솔루션 설계자가 무엇을 해야 합니까?
A. ReceiveMessage 대기 시간을 30초로 늘려 SQS 대기열에서 긴 폴링을 설정합니다. 
B. SQS 표준 대기열을 SQS FIFO 대기열로 변경합니다. 중복 메시지를 삭제하려면 메시지 중복 제거 ID를 사용하십시오. 
C. SQS 대기열의 가시성 제한 시간을 기능 제한 시간과 배치 창 제한 시간의 합계보다 큰 값으로 늘립니다. 
D. 처리하기 전에 메시지를 읽은 직후 SQS 대기열에서 각 메시지를 삭제하도록 Lambda 함수를 수정합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q135
회사는 AWS Organizations 설정을 사용하여 다양한 애플리케이션이 포함된 여러 AWS 계정을 관리합니다. 그들은 조직 내에 전용 모니터링 회원 계정을 설정했습니다. 이 회사는 Amazon CloudWatch를 사용하여 이러한 계정 전체의 관측 가능성 데이터에 액세스하고 시각화하는 것을 목표로 합니다. 이러한 요구 사항에 가장 적합한 솔루션은 무엇입니까?
A. 모니터링 계정에 대해 CloudWatch 교차 계정 관찰 기능을 활성화합니다. 모니터링 계정에서 제공하는 AWS CloudFormation 템플릿을 각 AWS 계정에 배포하여 모니터링 계정과
데이터를 공유합니다.
B. 조직의 루트 조직 단위(OU) 아래 모니터링 계정에서 CloudWatch에 대한 액세스 권한을 부여하도록 서비스 제어 정책(SCP)을 설정합니다. 
C. 모니터링 계정에 새 IAM 사용자를 구성합니다. 각 AWS 계정에서 CloudWatch 데이터 쿼리 및 시각화를 허용하는 IAM 정책을 설정합니다. 이 새 IAM 정책을 새 IAM 사용자에게 연
결합니다.
D. 모니터링 계정에 새 IAM 사용자를 생성합니다. 각 AWS 계정에 교차 계정 IAM 정책을 설정합니다. 이러한 IAM 정책을 새 IAM 사용자에게 연결합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q136
회사의 데이터 플랫폼은 Amazon Aurora MySQL 데이터베이스를 사용합니다. 데이터베이스에는 여러 가용 영역에 걸쳐 여러 읽기 전용 복제본과 여러 DB 인스턴스가 있습니다. 사용자는 최근 데이터베이스에서 너무 많은 연결이 있음을 나타내는 오류를 보고했습니다. 이 회사는 읽기 복제본이 기본 작성자로 승격될 때 장애 조치 시간을 20% 줄이려고 합니다. 이 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 다중 AZ 클러스터 배포를 통해 Aurora에서 Amazon RDS로 전환합니다.
B. Aurora 데이터베이스 앞에서 Amazon RDS Proxy를 사용합니다.
C. 읽기 연결을 위해 DAX(DynamoDB Accelerator)가 있는 Amazon DynamoDB로 전환합니다.
D. 재배치 기능이 있는 Amazon Redshift로 전환합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q137
회사는 두 개의 AWS 리전에서 3계층 애플리케이션을 실행 중입니다. 웹 티어, 애플리케이션 티어 및 데이터베이스 티어는 Amazon EC2 인스턴스에서 실행됩니다. 회사는 데이터베이스 티 어에 대해 Amazon RDS for Microsoft SQL Server Enterprise를 사용하고 있으며, 주간 및 월간 보고서를 실행할 때 데이터베이스 티어에 높은 부하가 걸립니다. 회사는 데이터베이스 티어의 부하를 줄이고자 합니다. 가장 적은 관리 작업으로 이러한 요구 사항을 충족시키는 솔루션은 무엇입니까?
A. 읽기 복제본을 만들고 보고서를 새로운 읽기 복제본을 사용하도록 구성합니다. 
B. RDS 데이터베이스를 Amazon DynamoDB로 변환하고 보고서를 DynamoDB를 사용하도록 구성합니다. 
C. 기존 RDS DB 인스턴스를 수정하여 더 큰 인스턴스 크기를 선택합니다. 
D. 기존 RDS DB 인스턴스를 수정하고 인스턴스를 Auto Scaling 그룹으로 넣습니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q138
회사는 VPC의 프라이빗 서브넷에 있는 Amazon EC2 인스턴스에 배포된 웹 애플리케이션을 실행합니다. 퍼블릭 서브넷에서 확장되는 ALB(Application Load Balancer)는 웹 트래픽 을 EC2 인스턴스로 보냅니다. 회사는 ALB에서 EC2 인스턴스로의 인바운드 트래픽을 제한하는 동시에 EC2 인스턴스의 프라이빗 서브넷 내부 또는 외부의 다른 소스로부터의 액세스를 방 지하는 새로운 보안 조치를 구현하려고 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 인터넷에서 EC2 인스턴스의 프라이빗 IP 주소로 트래픽을 보내도록 라우팅 테이블의 경로를 구성합니다. 
B. ALB의 보안 그룹에서 오는 트래픽만 허용하도록 EC2 인스턴스의 보안 그룹을 구성합니다. 
C. EC2 인스턴스를 퍼블릭 서브넷으로 이동합니다. EC2 인스턴스에 탄력적 IP 주소 집합을 제공합니다. 
D. 모든 포트에서 모든 TCP 트래픽을 허용하도록 ALB에 대한 보안 그룹을 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q139
회사에서 AWS에서 웹 애플리케이션을 구축하려고 합니다. 웹 사이트에 대한 클라이언트 액세스 요청은 예측할 수 없으며 오랫동안 유휴 상태일 수 있습니다. 가입비를 지불한 고객만이 웹 애 플리케이션에 로그인하고 사용할 수 있습니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 단계 조합은 무엇입니까? (3개를 선택하세요.)
A. Amazon DynamoDB에서 사용자 정보를 검색하는 AWS Lambda 함수를 생성합니다. RESTful API를 수락할 Amazon API Gateway 엔드포인트를 생성합니다. API 호출을
Lambda 함수로 보냅니다.
B. Application Load Balancer 뒤에 Amazon Elastic Container Service(Amazon ECS) 서비스를 생성하여 Amazon RDS에서 사용자 정보를 검색합니다. RESTful API를
수락할 Amazon API Gateway 엔드포인트를 생성합니다. API 호출을 Lambda 함수로 보냅니다.
C. 사용자를 인증하기 위해 Amazon Cognito 사용자 풀을 생성합니다. 
D. 사용자를 인증하기 위해 Amazon Cognito 자격 증명 풀을 생성합니다. 
E. AWS Amplify를 사용하여 HTML, CSS 및 JS로 프런트엔드 웹 콘텐츠를 제공합니다. 통합 Amazon CloudFront 구성을 사용합니다. 
F. PHP, CSS 및 JS와 함께 Amazon S3 정적 웹 호스팅을 사용합니다. Amazon CloudFront를 사용하여 프런트엔드 웹 콘텐츠를 제공합니다.

<details>
<summary>정답 보기</summary>

**ACE**
</details>

---

### Q140
회사는 AWS로 마이그레이션하고 애플리케이션에 Amazon EC2 온디맨드 인스턴스를 사용할 계획입니다. 마이그레이션 테스트 단계에서 기술 팀은 애플리케이션이 실행되고 메모리를 로 드하여 완전한 생산성을 발휘하는 데 오랜 시간이 걸린다는 사실을 관찰했습니다. 다음 테스트 단계에서 애플리케이션 실행 시간을 단축할 솔루션은 무엇입니까?
A. 두 개 이상의 EC2 온디맨드 인스턴스를 시작합니다. Auto Scaling 기능을 활성화하고 다음 테스트 단계에서 EC2 온디맨드 인스턴스를 사용할 수 있도록 하십시오. 
B. EC2 스팟 인스턴스를 시작하여 애플리케이션을 지원하고 다음 테스트 단계에서 사용할 수 있도록 애플리케이션을 확장합니다. 
C. 최대 절전 모드를 활성화한 상태에서 EC2 온디맨드 인스턴스를 시작합니다. 다음 테스트 단계에서 EC2 Auto Scaling 웜 풀을 구성합니다. 
D. 용량 예약을 통해 EC2 온디맨드 인스턴스를 시작합니다. 다음 테스트 단계에서 추가 EC2 인스턴스를 시작하십시오.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q141
회사는 Amazon API Gateway 및 AWS Lambda를 사용하여 AWS에서 RESTful 서버리스 웹 애플리케이션을 구축하고 있습니다. 이 웹 애플리케이션의 사용자는 지리적으로 분산되 며 회사는 이러한 사용자에 대한 API 요청 대기 시간을 줄이려고 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 어떤 유형의 엔드포인트를 사용해야 합니까?
A. 프라이빗 엔드포인트 
B. 지역 종점 
C. 인터페이스 VPC 엔드포인트 
D. 엣지 최적화 엔드포인트

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q142
회사는 Amazon EC2 인스턴스에서 실행되는 응용 프로그램을 보유하고 있으며, 이 인스턴스는 Amazon Elastic Block Store (Amazon EBS)로 지원됩니다. EC2 인스턴스는 가장 최신의 Amazon Linux 릴리스를 실행합니다. 회사의 직원들이 25GB 이상의 파일을 저장하고 검색할 때 응용 프로그램은 가용성 문제를 겪고 있습니다. 회사는 파일을 EC2 인스턴스 간에 전송할 필요가 없는 솔루션을 원하며 파일은 여러 EC2 인스턴스 및 여러 가용 영역에서 사용 가능해야 합니다. 이러한 요구 사항을 충족하는 가장 적합한 솔루션은 무엇인가요?
A. 모든 파일을 Amazon S3 버킷으로 마이그레이션합니다. 직원들에게 S3 버킷에서 파일에 액세스하도록 지시합니다. 
B. 기존 EBS 볼륨의 스냅샷을 찍습니다. 스냅샷을 EBS 볼륨으로 여러 EC2 인스턴스에 마운트합니다. 직원들에게 EC2 인스턴스에서 파일에 액세스하도록 지시합니다. 
C. 모든 EC2 인스턴스에서 Amazon Elastic File System (Amazon EFS) 파일 시스템을 마운트합니다. 직원들에게 EC2 인스턴스에서 파일에 액세스하도록 지시합니다. 
D. EC2 인스턴스에서 Amazon Machine Image (AMI)를 만듭니다. AMI에서 인스턴스 스토어 볼륨을 사용하는 새 EC2 인스턴스를 구성합니다. 직원들에게 EC2 인스턴스에서 파일
에 액세스하도록 지시합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q143
솔루션 아키텍트가 2계층 웹 애플리케이션을 설계하고 있습니다. 이 애플리케이션은 퍼블릭 서브넷의 Amazon EC2에서 호스팅되는 퍼블릭 웹 계층으로 구성됩니다. 데이터베이스 계층은 프라이빗 서브넷의 Amazon EC2에서 실행되는 Microsoft SQL Server로 구성됩니다. 보안은 회사의 최우선 순위입니다. 이 상황에서 보안 그룹을 어떻게 구성해야 합니까? (두 가지를 선택하세요.)
A. 0.0.0.0/0에서 포트 443의 인바운드 트래픽을 허용하도록 웹 계층에 대한 보안 그룹을 구성합니다. 
B. 0.0.0.0/0의 포트 443에서 아웃바운드 트래픽을 허용하도록 웹 계층에 대한 보안 그룹을 구성합니다. 
C. 웹 계층의 보안 그룹에서 포트 1433의 인바운드 트래픽을 허용하도록 데이터베이스 계층의 보안 그룹을 구성합니다. 
D. 웹 계층의 보안 그룹에 대한 포트 443 및 1433의 아웃바운드 트래픽을 허용하도록 데이터베이스 계층의 보안 그룹을 구성합니다. 
E. 웹 계층에 대한 보안 그룹의 포트 443 및 1433에서 인바운드 트래픽을 허용하도록 데이터베이스 계층에 대한 보안 그룹을 구성합니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q144
솔루션 설계자는 엔지니어링 도면을 저장하고 보는 데 사용되는 새 웹 애플리케이션의 스토리지 아키텍처를 설계하고 있습니다. 모든 애플리케이션 구성 요소는 AWS 인프라에 배포됩니다. 응용 프로그램 디자인은 사용자가 엔지니어링 도면이 로드될 때까지 기다리는 시간을 최소화하기 위해 캐싱을 지원해야 합니다. 애플리케이션은 페타바이트의 데이터를 저장할 수 있어야 합니 다. 솔루션 설계자는 어떤 스토리지 및 캐싱 조합을 사용해야 합니까?
A. Amazon CloudFront를 사용하는 Amazon S3 
B. Amazon ElastiCache를 사용하는 Amazon S3 Glacier 
C. Amazon CloudFront를 사용하는 Amazon Elastic Block Store(Amazon EBS) 볼륨 
D. Amazon ElastiCache를 사용하는 AWS Storage Gateway

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q145
회사에는 온프레미스에 여러 Windows 파일 서버가 있습니다. 이 회사는 파일을 Windows File Server 파일 시스템용 Amazon FSx로 마이그레이션하고 통합하려고 합니다. 액세스 권 한이 변경되지 않도록 하려면 파일 권한을 보존해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까? (두 가지를 선택하세요.)
A. 온프레미스에 AWS DataSync 에이전트를 배포합니다. 데이터를 FSx for Windows 파일 서버 파일 시스템으로 전송하도록 DataSync 작업을 예약합니다. 
B. AWS CLI를 사용하여 각 파일 서버의 공유를 Amazon S3 버킷에 복사합니다. 데이터를 FSx for Windows File Server 파일 시스템으로 전송하도록 AWS DataSync 작업을 예
약합니다.
C. 각 파일 서버에서 드라이브를 제거합니다. Amazon S3로 가져오기 위해 드라이브를 AWS로 배송합니다. 데이터를 FSx for Windows File Server 파일 시스템으로 전송하도록
AWS DataSync 작업을 예약합니다.
D. AWS Snowcone 디바이스를 주문합니다. 장치를 온프레미스 네트워크에 연결합니다. 디바이스에서 AWS DataSync 에이전트를 시작합니다. 데이터를 FSx for Windows 파일 서
버 파일 시스템으로 전송하도록 DataSync 작업을 예약합니다.
E. AWS Snowball Edge Storage Optimized 디바이스를 주문합니다. 장치를 온프레미스 네트워크에 연결합니다. AWS CLI를 사용하여 디바이스에 데이터를 복사합니다. Amazon
S3로 가져오기 위해 디바이스를 AWS로 반송합니다. 데이터를 FSx for Windows File Server 파일 시스템으로 전송하도록 AWS DataSync 작업을 예약합니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q146
회사에서 새로운 AWS 계정을 개설했습니다. 계정이 새로 프로비저닝되었으며 기본 설정이 변경되지 않았습니다. 회사는 AWS 계정 루트 사용자의 보안을 우려하고 있습니다. 루트 사용자를 보호하려면 어떻게 해야 합니까?
A. 일상적인 관리 작업을 위해 IAM 사용자를 생성합니다. 루트 사용자를 비활성화합니다. 
B. 일상적인 관리 작업을 위한 IAM 사용자를 생성합니다. 루트 사용자에 대해 다단계 인증을 활성화합니다. 
C. 루트 사용자에 대한 액세스 키를 생성합니다. AWS Management Console 대신 일일 관리 작업에 액세스 키를 사용하세요. 
D. 최고 수석 솔루션 설계자에게 루트 사용자 자격 증명을 제공합니다. 솔루션 설계자가 일상적인 관리 작업에 루트 사용자를 사용하도록 하세요.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q147
회사에 스토리지 용량이 부족한 온프레미스 데이터 센터가 있습니다. 회사는 대역폭 비용을 최소화하면서 스토리지 인프라를 AWS로 마이그레이션하려고 합니다. 솔루션은 추가 비용 없이 데 이터를 즉시 검색할 수 있어야 합니다. 이러한 요구 사항을 어떻게 충족할 수 있습니까?
A. Amazon S3 Glacier Vault를 배포하고 빠른 검색을 활성화합니다. 워크로드에 대해 프로비저닝된 검색 용량을 활성화합니다. 
B. 캐시된 볼륨을 사용하여 AWS Storage Gateway를 배포합니다. Storage Gateway를 사용하면 자주 액세스하는 데이터 하위 집합의 복사본을 로컬에 보관하면서 Amazon S3에
데이터를 저장할 수 있습니다.
C. 저장된 볼륨을 사용하여 AWS Storage Gateway를 배포하여 데이터를 로컬에 저장합니다. Storage Gateway를 사용하여 데이터의 특정 시점 스냅샷을 Amazon S3에 비동기식으
로 백업합니다.
D. AWS Direct Connect를 배포하여 온프레미스 데이터 센터에 연결합니다. 데이터를 로컬에 저장하도록 AWS Storage Gateway를 구성합니다. Storage Gateway를 사용하여 데
이터의 특정 시점 스냅샷을 Amazon S3에 비동기식으로 백업합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q148
회사에는 JSON 문서를 처리하고 그 결과를 온프레미스 SQL 데이터베이스에 출력하는 작은 Python 애플리케이션이 있습니다. 이 애플리케이션은 매일 수천 번 실행됩니다. 회사는 애플리 케이션을 AWS 클라우드로 이동하려고 합니다. 이 회사는 확장성을 최대화하고 운영 오버헤드를 최소화하는 고가용성 솔루션이 필요합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. JSON 문서를 Amazon S3 버킷에 넣습니다. 여러 Amazon EC2 인스턴스에서 Python 코드를 실행하여 문서를 처리합니다. 결과를 Amazon Aurora DB 클러스터에 저장합니다
.
B. JSON 문서를 Amazon S3 버킷에 넣습니다. 문서가 S3 버킷에 도착하면 이를 처리하기 위해 Python 코드를 실행하는 AWS Lambda 함수를 생성합니다. 결과를 Amazon
Aurora DB 클러스터에 저장합니다.
C. JSON 문서를 Amazon Elastic Block Store(Amazon EBS) 볼륨에 넣습니다. EBS 다중 연결 기능을 사용하여 볼륨을 여러 Amazon EC2 인스턴스에 연결합니다. EC2 인스턴
스에서 Python 코드를 실행하여 문서를 처리합니다. Amazon RDS DB 인스턴스에 결과를 저장합니다.
D. JSON 문서를 Amazon Simple Queue Service(Amazon SQS) 대기열에 메시지로 배치합니다. Amazon EC2 시작 유형으로 구성된 Amazon Elastic Container Service
(Amazon ECS) 클러스터에 Python 코드를 컨테이너로 배포합니다. 컨테이너를 사용하여 SQS 메시지를 처리합니다. Amazon RDS DB 인스턴스에 결과를 저장합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q149
미디어 회사는 연령에 따라 다양한 영화 수요에 따라 구매 후 5분 이내에 스트리(cid:1535) 콘텐츠를 제공하여 사용자 요구를 충족해야 합니다. 이에 따라 회사는 호스팅 서비스 비용을 최소화하는 것을 목표로 합니다. 이러한 요구 사항에 맞는 솔루션은 무엇입니까?
A. 모든 미디어 콘텐츠를 Amazon S3에 저장합니다. 영화에 대한 수요가 감소함에 따라 S3 수명 주기 정책을 사용하여 미디어 데이터를 자주 액세스하지 않는 계층으로 전환합니다.
B. 최신 영화 비디오 파일은 S3 Standard에 저장하고 이전 영화 비디오 파일은 S3 Standard-Infrequent Access(S3 Standard-IA)에 저장합니다. 표준 검색을 사용하여 오래된 영화
의 비디오 파일을 검색합니다.
C. S3 Intelligent-Tiering에 최신 영화 비디오 파일을 저장합니다. 오래된 영화 비디오 파일의 경우 유연한 검색 기능이 있는 S3 Glacier를 사용하십시오. 신속 검색을 사용하여 오래된 영
화의 비디오 파일을 검색합니다.
D. 최신 영화 비디오 파일은 S3 Standard에 저장하고 이전 영화 비디오 파일은 유연한 검색을 통해 S3 Glacier에 저장합니다. 대량 검색을 사용하여 오래된 영화의 비디오 파일을 검색합
니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q150
연구 회사는 시뮬레이션 응용 프로그램과 시각화 응용 프로그램으로 구동되는 실험을 실행합니다. 시뮬레이션 애플리케이션은 Linux에서 실행되며 5분마다 NFS 공유에 중간 데이터를 출력 합니다. 시각화 응용 프로그램은 시뮬레이션 출력을 표시하고 SMB 파일 시스템이 필요한 Windows 데스크톱 응용 프로그램입니다. 회사는 두 개의 동기화된 파일 시스템을 유지 관리합니다. 이 전략은 데이터 중복 및 비효율적인 리소스 사용을 유발합니다. 회사는 애플리케이션에 코드를 변경하지 않고 애플리케이션을 AWS로 마이그레이션해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 두 애플리케이션을 모두 AWS Lambda로 마이그레이션합니다. 애플리케이션 간에 데이터를 교환할 Amazon S3 버킷을 생성합니다.
B. 두 애플리케이션을 모두 Amazon Elastic Container Service(Amazon ECS)로 마이그레이션합니다. 스토리지용 Amazon FSx 파일 게이트웨이를 구성합니다.
C. 시뮬레이션 애플리케이션을 Linux Amazon EC2 인스턴스로 마이그레이션합니다. 시각화 애플리케이션을 Windows EC2 인스턴스로 마이그레이션합니다. 애플리케이션 간에 데이터
를 교환하도록 Amazon Simple Queue Service(Amazon SQS)를 구성합니다.
D. 시뮬레이션 애플리케이션을 Linux Amazon EC2 인스턴스로 마이그레이션합니다. 시각화 애플리케이션을 Windows EC2 인스턴스로 마이그레이션합니다. 스토리지용 NetApp
ONTAP용 Amazon FSx를 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q151
회사에서 외부 감사인과 회계 데이터를 공유하려고 합니다. 데이터는 프라이빗 서브넷에 상주하는 Amazon RDS DB 인스턴스에 저장됩니다. 감사자는 자체 AWS 계정이 있으며 자체 데이 터베이스 사본이 필요합니다. 회사가 감사자와 데이터베이스를 공유하는 가장 안전한 방법은 무엇입니까?
A. 데이터베이스의 읽기 전용 복제본을 생성합니다. 감사자 액세스 권한을 부여하도록 IAM 표준 데이터베이스 인증을 구성합니다.
B. 데이터베이스 내용을 텍스트 파일로 내보냅니다. 파일을 Amazon S3 버킷에 저장합니다. 감사자를 위한 새 IAM 사용자를 생성합니다. 사용자에게 S3 버킷에 대한 액세스 권한을 부여
합니다.
C. 데이터베이스의 스냅샷을 Amazon S3 버킷에 복사합니다. IAM 사용자를 생성합니다. 사용자의 키를 감사자와 공유하여 S3 버킷의 객체에 대한 액세스 권한을 부여합니다.
D. 데이터베이스의 암호화된 스냅샷을 생성합니다. 감사자와 스냅샷을 공유합니다. AWS Key Management Service(AWS KMS) 암호화 키에 대한 액세스를 허용합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q152
회사는 Amazon EC2 인스턴스와 Amazon Elastic Block Store(Amazon EBS) 볼륨을 사용하여 애플리케이션을 실행합니다. 회사는 규정 준수 요구 사항을 충족하기 위해 매일 각 EBS 볼륨에 대해 하나의 스냅샷을 생성합니다. 회사는 EBS 볼륨 스냅샷이 실수로 삭제되는 것을 방지하는 아키텍처를 구현하려고 합니다. 솔루션은 스토리지 관리자 사용자의 관리 권한을 변경해서는 안 됩니다. 최소한의 관리 노력으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 스냅샷 삭제 권한이 있는 IAM 역할을 생성합니다. 새 EC2 인스턴스에 역할을 연결합니다. 스냅샷을 삭제하려면 새 EC2 인스턴스에서 AWS CLI를 사용하세요. 
B. 스냅샷 삭제를 거부하는 IAM 정책을 생성합니다. 스토리지 관리자 사용자에게 정책을 연결합니다. 
C. 스냅샷에 태그를 추가합니다. 태그가 있는 EBS 스냅샷에 대해 휴지통에 보관 규칙을 만듭니다. 
D. 삭제를 방지하기 위해 EBS 스냅샷을 잠급니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q153
Amazon EC2 관리자는 여러 사용자를 포함하는 IAM 그룹과 연결된 다음 정책을 생성했습니다. 이 정책의 효과는 무엇입니까?
A. 사용자는 us-east-1을 제외한 모든 AWS 리전에서 EC2 인스턴스를 종료할 수 있습니다. 
B. 사용자는 us-east-1 지역에서 IP 주소가 10.100.100.1인 EC2 인스턴스를 종료할 수 있습니다. 
C. 사용자의 소스 IP가 10.100.100.254인 경우 사용자는 us-east-1 지역에서 EC2 인스턴스를 종료할 수 있습니다. 
D. 사용자의 소스 IP가 10.100.100.254인 경우 사용자는 us-east-1 지역에서 EC2 인스턴스를 종료할 수 없습니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q154
회사에서 AWS에 새로운 퍼블릭 웹 애플리케이션을 배포하고 있습니다. 애플리케이션은 ALB(Application Load Balancer) 뒤에서 실행됩니다. 외부 인증 기관(CA)에서 발급한 SSL/ TLS 인증서를 사용하여 에지에서 애플리케이션을 암호화해야 합니다. 인증서는 만료되기 전에 매년 교체해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS Certificate Manager(ACM)를 사용하여 SSL/TLS 인증서를 발급합니다. ALB에 인증서를 적용합니다. 관리형 갱신 기능을 사용하여 인증서를 자동으로 교체하십시오. 
B. AWS Certificate Manager(ACM)를 사용하여 SSL/TLS 인증서를 발급합니다. 인증서에서 키 자료를 가져옵니다. 인증서를 AL에 적용관리형 갱신 기능을 사용하여 인증서를 자동
으로 교체하십시오.
C. AWS Certificate Manager(ACM) 사설 인증 기관을 사용하여 루트 CA에서 SSL/TLS 인증서를 발급합니다. ALB에 인증서를 적용합니다. 관리형 갱신 기능을 사용하여 인증서를
자동으로 교체하십시오.
D. AWS Certificate Manager(ACM)를 사용하여 SSL/TLS 인증서를 가져옵니다. ALB에 인증서를 적용합니다. 인증서 만료가 가까워지면 Amazon EventBridge(Amazon
CloudWatch Events)를 사용하여 알림을 보냅니다. 인증서를 수동으로 교체하십시오.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q155
회사는 서로 다른 제품군에 대해 AWS에서 여러 애플리케이션을 호스팅합니다. 애플리케이션은 Amazon EC2 인스턴스 및 Application Load Balancer를 비롯한 다양한 컴퓨팅 리소스 를 사용합니다. 애플리케이션은 여러 AWS 리전의 AWS Organizations에서 동일한 조직의 다른 AWS 계정에서 실행됩니다. 각 제품군의 팀은 개별 계정의 각 컴퓨팅 리소스에 태그를 지 정했습니다. 회사는 조직의 통합 청구 기능에서 각 제품군의 비용에 대한 자세한 정보를 원합니다. 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (두 가지를 선택하세요.)
A. AWS 결제 콘솔에서 특정 AWS 생성 태그를 선택합니다. 
B. AWS 결제 콘솔에서 특정 사용자 정의 태그를 선택합니다. 
C. AWS 리소스 그룹 콘솔에서 특정 사용자 정의 태그를 선택합니다. 
D. 각 AWS 계정에서 선택한 태그를 활성화합니다. 
E. 조직 마스터 계정에서 선택한 태그를 활성화합니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q156
소매 회사는 퍼블릭 REST API에 지역 Amazon API Gateway API를 사용합니다. API Gateway 엔드포인트는 Amazon Route 53 별칭 레코드를 가리키는 사용자 지정 도메인 이름 입니다. 솔루션 아키텍트는 고객에게 최소한의 영향을 미치고 데이터 손실을 최소화하는 솔루션을 생성하여 새 버전의 API를 릴리스해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. API 게이트웨이에 대한 카나리아 릴리스 배포 단계를 생성합니다. 최신 API 버전을 배포합니다. 트래픽의 적절한 비율을 카나리아 단계로 지정합니다. API 검증 후 카나리아 단계를 프로
덕션 단계로 승격합니다.
B. OpenAPI YAML 파일 형식의 새 API 버전으로 새 API 게이트웨이 엔드포인트를 생성합니다. API Gateway의 API에 병합 모드에서 가져오기-업데이트 작업을 사용합니다. API의 새
버전을 프로덕션 단계에 배포합니다.
C. OpenAPI JSON 파일 형식의 새 API 버전으로 새 API 게이트웨이 엔드포인트를 생성합니다. 덮어쓰기 모드에서 업데이트로 가져오기 작업을 API Gateway의 API에 사용합니다.
API의 새 버전을 프로덕션 단계에 배포합니다.
D. API 정의의 새 버전으로 새 API 게이트웨이 엔드포인트를 생성합니다. 새 API Gateway API에 대한 사용자 지정 도메인 이름을 생성합니다. Route 53 별칭 레코드가 새 API
Gateway API 사용자 지정 도메인 이름을 가리키도록 합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q157
한 회사에 Amazon DynamoDB 테이블을 저장용으로 사용하는 애플리케이션이 있습니다. 솔루션 설계자는 테이블에 대한 많은 요청이 최신 데이터를 반환하지 않는다는 것을 발견했습니다 . 회사 사용자는 데이터베이스 성능과 관련된 다른 문제를 보고하지 않았습니다. 지연 시간이 허용 가능한 범위 내에 있습니다. 솔루션 설계자는 어떤 디자인 변경을 권장해야 합니까?
A. 테이블에 읽기 전용 복제본을 추가합니다. 
B. 글로벌 보조 인덱스(GSI)를 사용합니다. 
C. 테이블에 대해 강력하게 일관된 읽기를 요청합니다. 
D. 테이블에 대한 최종적 일관된 읽기를 요청합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q158
회사는 수백 개의 AWS 계정에 걸쳐 있는 us-east-1 리전의 여러 VPC를 연결해야 합니다. 회사의 네트워킹 팀에는 클라우드 네트워크를 관리하기 위한 자체 AWS 계정이 있습니다. VPC를 연결하기 위한 운영상 가장 효율적인 솔루션은 무엇입니까?
A. 각 VPC 간에 VPC 피어링 연결을 설정합니다. 연결된 각 서브넷의 경로 테이블 업데이트 
B. 인터넷을 통해 각 VPC를 연결하기 위해 각 VPC에 NAT 게이트웨이와 인터넷 게이트웨이를 구성합니다. 
C. 네트워킹 팀의 AWS 계정에서 AWS Transit Gateway를 생성합니다. 각 VPC에서 정적 경로를 구성합니다. 
D. 각 VPC에 VPN 게이트웨이를 배포합니다. 네트워킹 팀의 AWS 계정에 전송 VPC를 생성하여 각 VPC에 연결합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q159
한 회사에서 3계층 애플리케이션을 온프레미스에서 AWS로 마이그레이션하려고 합니다. 웹 계층과 애플리케이션 계층은 타사 VM(가상 머신)에서 실행됩니다. 데이터베이스 계층은 MySQL에서 실행됩니다. 회사는 아키텍처를 최소한으로 변경하여 애플리케이션을 마이그레이션해야 합니다. 또한 회사에는 데이터를 특정 시점으로 복원할 수 있는 데이터베이스 솔루션이 필요합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 웹 계층과 애플리케이션 계층을 프라이빗 서브넷의 Amazon EC2 인스턴스로 마이그레이션합니다. 데이터베이스 계층을 프라이빗 서브넷의 MySQL용 Amazon RDS로 마이그레이
션합니다.
B. 웹 계층을 퍼블릭 서브넷의 Amazon EC2 인스턴스로 마이그레이션합니다. 애플리케이션 계층을 프라이빗 서브넷의 EC2 인스턴스로 마이그레이션합니다. 데이터베이스 계층을 프라이
빗 서브넷의 Amazon Aurora MySQL로 마이그레이션합니다.
C. 웹 계층을 퍼블릭 서브넷의 Amazon EC2 인스턴스로 마이그레이션합니다. 애플리케이션 계층을 프라이빗 서브넷의 EC2 인스턴스로 마이그레이션합니다. 데이터베이스 계층을 프라이
빗 서브넷의 MySQL용 Amazon RDS로 마이그레이션합니다.
D. 웹 계층과 애플리케이션 계층을 퍼블릭 서브넷의 Amazon EC2 인스턴스로 마이그레이션합니다. 데이터베이스 계층을 퍼블릭 서브넷의 Amazon Aurora MySQL로 마이그레이션합
니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q160
회사에서 AWS Key Management Service(AWS KMS) 키를 사용하여 AWS Lambda 환경 변수를 암호화하고 있습니다. 솔루션 설계자는 환경 변수를 해독하고 사용하는 데 필요한 권한이 있는지 확인해야 합니다. 올바른 권한을 구현하기 위해 솔루션 설계자가 수행해야 하는 단계는 무엇입니까? (두 가지를 선택하세요.)
A. Lambda 리소스 정책에 AWS KMS 권한을 추가합니다. 
B. Lambda 실행 역할에 AWS KMS 권한을 추가합니다. 
C. Lambda 함수 정책에 AWS KMS 권한을 추가합니다. 
D. AWS KMS 키 정책에서 Lambda 실행 역할을 허용합니다. 
E. AWS KMS 키 정책에서 Lambda 리소스 정책을 허용합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q161
회사는 AWS 클라우드에서 웹 애플리케이션을 호스팅합니다. 회사는 AWS Certificate Manager(ACM)로 가져온 인증서를 사용하도록 Elastic Load Balancer를 구성합니다. 각 인증 서가 만료되기 30일 전에 회사의 보안 팀에 알려야 합니다. 이 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. 인증서가 만료되기 30일 전부터 매일 Amazon Simple Notification Service(Amazon SNS) 주제에 사용자 지정 메시지를 게시하는 규칙을 ACM에 추가합니다. 
B. 30일 이내에 만료되는 인증서를 확인하는 AWS Config 규칙을 생성합니다. AWS Config가 비준수 리소스를 보고할 때 Amazon Simple Notification Service(Amazon SNS)
를 통해 사용자 지정 알림을 호출하도록 Amazon EventBridge(Amazon CloudWatch Events)를 구성합니다.
C. AWS Trusted Advisor를 사용하여 30일 이내에 만료되는 인증서를 확인합니다. 확인 상태 변경에 대한 Trusted Advisor 지표를 기반으로 하는 Amazon CloudWatch 경보를 생
성합니다. Amazon Simple Notification Service(Amazon SNS)를 통해 사용자 지정 알림을 보내도록 경보를 구성합니다.
D. 30일 이내에 만료되는 모든 인증서를 감지하는 Amazon EventBridge(Amazon CloudWatch Events) 규칙을 생성합니다. AWS Lambda 함수를 호출하도록 규칙을 구성합니다
. Amazon Simple Notification Service(Amazon SNS)를 통해 사용자 지정 알림을 보내도록 Lambda 함수를 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q162
한 회사에서 REST API로 검색할 주문 배송 통계를 제공하는 애플리케이션을 개발하고 있습니다. 회사는 배송 통계를 추출하고 데이터를 읽기 쉬운 HTML 형식으로 구성하고 매일 아침 동 시에 여러 이메일 주소로 보고서를 보내려고 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. 데이터를 Amazon Kinesis Data Firehose로 보내도록 애플리케이션을 구성합니다.
B. Amazon Simple Email Service(Amazon SES)를 사용하여 데이터 형식을 지정하고 이메일로 보고서를 보냅니다.
C. 데이터에 대한 애플리케이션의 API를 쿼리하기 위해 AWS Glue 작업을 호출하는 Amazon EventBridge(Amazon CloudWatch Events) 예약 이벤트를 생성합니다.
D. 데이터에 대한 애플리케이션의 API를 쿼리하기 위해 AWS Lambda 함수를 호출하는 Amazon EventBridge(Amazon CloudWatch Events) 예약 이벤트를 생성합니다.
E. 애플리케이션 데이터를 Amazon S3에 저장합니다. 보고서를 이메일로 보낼 S3 이벤트 대상으로 Amazon Simple Notification Service(Amazon SNS) 주제를 생성합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q163
한 도시에서는 ALB(Application Load Balancer) 뒤에 Amazon EC2 인스턴스에서 실행되는 웹 애플리케이션을 배포했습니다. 애플리케이션 사용자는 산발적인 성능을 보고했는데, 이 는 무작위 IP 주소에서 발생하는 DDoS 공격과 관련된 것으로 보입니다. 도시에는 구성 변경을 최소화하고 DDoS 소스에 대한 감사 추적을 제공하는 솔루션이 필요합니다. 이러한 요구 사항 을 충족하는 솔루션은 무엇입니까?
A. ALB에서 AWS WAF 웹 ACL을 활성화하고 알 수 없는 소스의 트래픽을 차단하는 규칙을 구성합니다. 
B. Amazon Inspector를 구독하세요. AWS DDoS 대응 팀(DRT)을 참여시켜 완화 제어 기능을 서비스에 통합하십시오. 
C. AWS Shield Advanced를 구독하세요. AWS DDoS 대응 팀(DRT)을 참여시켜 완화 제어 기능을 서비스에 통합하십시오. 
D. 애플리케이션에 대한 Amazon CloudFront 배포를 생성하고 ALB를 오리진으로 설정합니다. 배포에서 AWS WAF 웹 ACL을 활성화하고 알 수 없는 소스의 트래픽을 차단하는 규칙
을 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q164
회사는 AWS에 사용자 디바이스에서 센서 데이터를 수집하는 3계층 애플리케이션을 보유하고 있습니다. 트래픽은 NLB(Network Load Balancer)를 거쳐 웹 계층용 Amazon EC2 인스 턴스로 이동한 다음 마지막으로 애플리케이션 계층용 EC2 인스턴스로 이동합니다. 애플리케이션 계층은 데이터베이스를 호출합니다. 솔루션 설계자는 전송 중인 데이터의 보안을 개선하기 위해 무엇을 해야 합니까?
A. TLS 수신기를 구성합니다. NLB에 서버 인증서를 배포합니다. 
B. AWS Shield Advanced를 구성합니다. NLB에서 AWS WAF를 활성화합니다. 
C. 로드 밸런서를 Application Load Balancer(ALB)로 변경합니다. ALB에서 AWS WAF를 활성화합니다. 
D. AWS Key Management Service(AWS KMS)를 사용하여 EC2 인스턴스에서 Amazon Elastic Block Store(Amazon EBS) 볼륨을 암호화합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q165
회사는 애플리케이션에 대한 실시간 데이터 수집 아키텍처를 구성해야 합니다. 회사는 API, 데이터가 스트리(cid:1535)될 때 데이터를 변환하는 프로세스, 데이터를 위한 스토리지 솔루션이 필요합니 다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Kinesis 데이터 스트림으로 데이터를 전송하는 API를 호스팅하기 위해 Amazon EC2 인스턴스를 배포합니다. Kinesis 데이터 스트림을 데이터 소스로 사용하는 Amazon
Kinesis Data Firehose 전송 스트림을 생성합니다. AWS Lambda 함수를 사용하여 데이터를 변환합니다. Kinesis Data Firehose 전송 스트림을 사용하여 데이터를 Amazon S3로 보냅니다.
B. AWS Glue로 데이터를 전송하는 API를 호스팅하기 위해 Amazon EC2 인스턴스를 배포합니다. EC2 인스턴스에서 소스/대상 확인을 중지합니다. AWS Glue를 사용하여 데이터를
변환하고 데이터를 Amazon S3로 보냅니다.
C. Amazon Kinesis 데이터 스트림으로 데이터를 전송하도록 Amazon API Gateway API를 구성합니다. Kinesis 데이터 스트림을 데이터 소스로 사용하는 Amazon Kinesis Data
Firehose 전송 스트림을 생성합니다. AWS Lambda 함수를 사용하여 데이터를 변환합니다. Kinesis Data Firehose 전송 스트림을 사용하여 데이터를 Amazon S3로 보냅니다.
D. AWS Glue로 데이터를 전송하도록 Amazon API Gateway API를 구성합니다. AWS Lambda 함수를 사용하여 데이터를 변환합니다. AWS Glue를 사용하여 데이터를 Amazon
S3로 보냅니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q166
회사에서 계층적 구조 관계로 직원 데이터를 저장하는 애플리케이션을 만들고자 합니다. 회사는 직원 데이터에 대한 트래픽이 많은 쿼리에 대한 최소 대기 시간 응답이 필요하며 민감한 데이터 를 보호해야 합니다. 회사는 또한 직원 데이터에 재무 정보가 있는 경우 월별 이메일 메시지를 받아야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. Amazon Redshift를 사용하여 직원 데이터를 계층에 저장하십시오. 매월 Amazon S3에 데이터를 언로드합니다. 
B. Amazon DynamoDB를 사용하여 직원 데이터를 계층에 저장합니다. 매월 데이터를 Amazon S3로 내보냅니다. 
C. AWS 계정에 대해 Amazon Macie를 구성합니다. Macie를 Amazon EventBridge와 통합하여 월별 이벤트를 AWS Lambda로 전송합니다. 
D. Amazon Athena를 사용하여 Amazon S3에서 직원 데이터를 분석합니다. Athena를 Amazon QuickSight와 통합하여 분석 대시보드를 게시하고 사용자와 대시보드를 공유합니다
.
E. AWS 계정에 대해 Amazon Macie를 구성합니다. Macie를 Amazon EventBridge와 통합하여 Amazon Simple Notification Service(Amazon SNS) 구독을 통해 월별 알
림을 보냅니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q167
한 회사에서 Amazon EC2 인스턴스에서 실행할 새 웹 애플리케이션을 설계하고 있습니다. 애플리케이션은 백엔드 데이터 스토리지에 Amazon DynamoDB를 사용합니다. 애플리케이션 트래픽은 예측할 수 없습니다. 회사는 데이터베이스에 대한 응용 프로그램 읽기 및 쓰기 처리량이 보통에서 높을 것으로 예상합니다. 회사는 애플리케이션 트래픽에 대응하여 확장해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 DynamoDB 테이블 구성은 무엇입니까?
A. DynamoDB 표준 테이블 클래스를 사용하여 프로비저닝된 읽기 및 쓰기로 DynamoDB를 구성합니다. DynamoDB Auto Scaling을 정의된 최대 용량으로 설정합니다. 
B. DynamoDB Standard 테이블 클래스를 사용하여 온디맨드 모드에서 DynamoDB를 구성합니다. 
C. DynamoDB Standard Infrequent Access(DynamoDB Standard-IA) 테이블 클래스를 사용하여 프로비저닝된 읽기 및 쓰기로 DynamoDB를 구성합니다. DynamoDB
Auto Scaling을 정의된 최대 용량으로 설정합니다.
D. DynamoDB Standard Infrequent Access(DynamoDB Standard-IA) 테이블 클래스를 사용하여 온디맨드 모드에서 DynamoDB를 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q168
회사는 AWS 클라우드에서 호스팅되는 미디어 애플리케이션을 위한 공유 스토리지 솔루션을 구현하고 있습니다. 회사는 SMB 클라이언트를 사용하여 데이터에 액세스할 수 있는 기능이 필요 합니다. 솔루션은 완전히 관리되어야 합니다. 어떤 AWS 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS Storage Gateway 볼륨 게이트웨이를 생성합니다. 필요한 클라이언트 프로토콜을 사용하는 파일 공유를 만듭니다. 응용 프로그램 서버를 파일 공유에 연결합니다. 
B. AWS Storage Gateway 테이프 게이트웨이를 생성합니다. Amazon S3를 사용하도록 테이프를 구성합니다. 애플리케이션 서버를 테이프 게이트웨이에 연결합니다. 
C. Amazon EC2 Windows 인스턴스를 생성합니다. 인스턴스에 Windows 파일 공유 역할을 설치하고 구성합니다. 응용 프로그램 서버를 파일 공유에 연결합니다. 
D. Windows 파일 서버 파일 시스템용 Amazon FSx를 생성합니다. 원본 서버에 파일 시스템을 연결합니다. 애플리케이션 서버를 파일 시스템에 연결하십시오.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q169
회사에는 동일한 AWS 리전의 Amazon S3 버킷에서 대량의 데이터를 읽고 쓰는 서비스가 있습니다. 이 서비스는 VPC의 프라이빗 서브넷 내 Amazon EC2 인스턴스에 배포됩니다. 이 서비스는 퍼블릭 서브넷의 NAT 게이트웨이를 통해 Amazon S3와 통신합니다. 그러나 회사는 데이터 출력 비용을 줄일 수 있는 솔루션을 원합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 퍼블릭 서브넷에서 전용 EC2 NAT 인스턴스를 프로비저닝합니다. 이 인스턴스의 탄력적 네트워크 인터페이스를 모든 S3 트래픽의 대상으로 사용하도록 프라이빗 서브넷에 대한 라우팅
테이블을 구성합니다.
B. 프라이빗 서브넷에서 전용 EC2 NAT 인스턴스를 프로비저닝합니다. 이 인스턴스의 탄력적 네트워크 인터페이스를 모든 S3 트래픽의 대상으로 사용하도록 퍼블릭 서브넷에 대한 라우팅
테이블을 구성합니다.
C. VPC 게이트웨이 엔드포인트를 프로비저닝합니다. 게이트웨이 엔드포인트를 모든 S3 트래픽의 경로로 사용하도록 프라이빗 서브넷에 대한 경로 테이블을 구성합니다. 
D. 두 번째 NAT 게이트웨이를 프로비저닝합니다. 이 NAT 게이트웨이를 모든 S3 트래픽의 대상으로 사용하도록 프라이빗 서브넷에 대한 라우팅 테이블을 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q170
한 회사는 애플리케이션 메시징을 정확히 한 번만 전달하면서 인프라 관리를 최소화하는 솔루션을 채택하는 것을 목표로 합니다. 이러한 요구 사항을 충족하는 작업 조합은 무엇입니까? (2개를 선택하세요.)
A. 아키텍처의 컴퓨팅 계층에 AWS Lambda를 활용합니다. 
B. 아키텍처의 컴퓨팅 계층에 Amazon EC2 인스턴스를 사용합니다. 
C. 컴퓨팅 계층 간의 메시징 구성 요소로 Amazon Simple 알림 서비스(Amazon SNS)를 구현합니다. 
D. Amazon Simple Queue Service(Amazon SQS) FIFO 대기열을 컴퓨팅 계층 간의 메시징 구성 요소로 활용합니다. 
E. 아키텍처의 컴퓨팅 계층을 위해 Amazon Elastic Kubernetes Service(Amazon EKS)를 기반으로 컨테이너를 배포합니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q171
회사에 매장에 마케팅 서비스를 제공하는 애플리케이션이 있습니다. 서비스는 매장 고객의 이전 구매를 기반으로 합니다. 상점은 SFTP를 통해 거래 데이터를 회사에 업로드하고 데이터를 처 리 및 분석하여 새로운 마케팅 제안을 생성합니다. 일부 파일은 크기가 200GB를 초과할 수 있습니다. 최근 회사는 일부 매장에서 포함되어서는 안 되는 개인 식별 정보(PII)가 포함된 파일을 업로드한 것을 발견했습니다. 회사는 PII가 다시 공유될 경우 관리자에게 알림을 받기를 원합니다. 회사 는 또한 문제 해결을 자동화하기를 원합니다. 최소한의 개발 노력으로 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. Amazon S3 버킷을 안전한 전송 지점으로 사용하십시오. Amazon Inspector를 사용하여 버킷의 객체를 스캔합니다. 개체에 PII가 포함된 경우 S3 수명 주기 정책을 트리거하여 PII
가 포함된 개체를 제거합니다.
B. Amazon S3 버킷을 안전한 전송 지점으로 사용하십시오. Amazon Macie를 사용하여 버킷의 객체를 스캔합니다. 객체에 PII가 포함된 경우 Amazon Simple Notification
Service(Amazon SNS)를 사용하여 관리자에게 PII가 포함된 객체를 제거하라는 알림을 트리거합니다.
C. AWS Lambda 함수에서 사용자 지정 검색 알고리즘을 구현합니다. 객체가 버킷에 로드될 때 함수를 트리거합니다. 객체에 PII가 포함된 경우 Amazon Simple Notification
Service(Amazon SNS)를 사용하여 관리자에게 PII가 포함된 객체를 제거하라는 알림을 트리거합니다.
D. AWS Lambda 함수에서 사용자 지정 검색 알고리즘을 구현합니다. 객체가 버킷에 로드될 때 함수를 트리거합니다. 객체에 PII가 포함된 경우 Amazon Simple Email Service
(Amazon SES)를 사용하여 관리자에게 알림을 트리거하고 S3 수명 주기 정책을 트리거하여 PII가 포함된 미트를 제거합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q172
AWS에서 쇼핑 애플리케이션을 구축하는 회사에는 짧은 지연 시간, 트래픽 볼륨에 따른 확장성을 제공하고 사용자 연결이 끊어졌다가 다시 연결되는 경우에도 장바구니 데이터의 높은 가용성 을 보장하는 솔루션이 필요합니다. 장바구니 데이터의 일관적인 보존을 보장하기 위해 솔루션 설계자는 어떤 솔루션을 구현해야 합니까?
A. Amazon Aurora의 카탈로그에 액세스하려면 고정 세션 기능(세션 선호도)을 사용하여 Application Load Balancer를 구성하십시오. 
B. Amazon DynamoDB의 카탈로그 데이터와 사용자 세션의 장바구니 데이터를 캐시하도록 Redis용 Amazon ElastiCache를 구성합니다. 
C. Amazon DynamoDB의 카탈로그 데이터와 사용자 세션의 장바구니 데이터를 캐시하도록 Amazon OpenSearch Service를 구성합니다. 
D. 카탈로그 및 장바구니를 위한 Amazon Elastic Block Store(Amazon EBS) 스토리지로 Amazon EC2 인스턴스를 구성합니다. 자동 스냅샷을 설정하세요.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q173
회사는 Amazon Elastic Kubernetes Service(Amazon EKS)를 사용하여 컨테이너 애플리케이션을 실행합니다. 애플리케이션에는 고객을 관리하고 주문하는 마이크로서비스가 포함되 어 있습니다. 회사는 들어오는 요청을 적절한 마이크로서비스로 라우팅해야 합니다. 이 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. AWS 로드 밸런서 컨트롤러를 사용하여 Network Load Balancer를 프로비저닝하십시오. 
B. AWS Load Balancer Controller를 사용하여 Application Load Balancer를 프로비저닝합니다. 
C. AWS Lambda 함수를 사용하여 요청을 Amazon EKS에 연결합니다. 
D. Amazon API Gateway를 사용하여 요청을 Amazon EKS에 연결합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q174
회사는 Amazon EC2 인스턴스에서 마이크로서비스 애플리케이션을 실행하고 있습니다. 이 회사는 확장성을 위해 애플리케이션을 Amazon Elastic Kubernetes Service(Amazon EKS) 클러스터로 마이그레이션하려고 합니다. 회사는 보안 규정 준수를 유지하기 위해 엔드포인트 프라이빗 액세스를 true로 설정하고 엔드포인트 퍼블릭 액세스를 false로 설정하여 Amazon EKS 제어 플레인을 구성해야 합니다. 회사는 또한 사설 서브넷에 데이터 플레인을 배치해야 합니다. 그러나 회사는 노드가 클러스터에 가입할 수 없기 때문에 오류 알림을 받았습니 다. 노드가 클러스터에 가입하도록 허용하는 솔루션은 무엇입니까?
A. AWS Identity and Access Management(IAM)에서 필요한 권한을 AmazonEKSNodeRole IAM 역할에 부여합니다. 
B. 노드가 컨트롤 플레인에 액세스할 수 있도록 인터페이스 VPC 엔드포인트를 생성합니다. 
C. 퍼블릭 서브넷에서 노드를 재생성합니다. EC2 노드에 대한 보안 그룹을 제한합니다. 
D. 노드의 보안 그룹에서 아웃바운드 트래픽을 허용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q175
솔루션 설계자는 회사의 온프레미스 인프라를 AWS로 확장하기 위해 새로운 하이브리드 아키텍처를 설계하고 있습니다. 이 회사는 AWS 리전에 대해 지속적으로 짧은 지연 시간을 갖는 고가 용성 연결이 필요합니다. 회사는 비용을 최소화해야 하며 기본 연결이 실패할 경우 더 느린 트래픽을 수용할 의향이 있습니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 리전에 대한 AWS Direct Connect 연결을 프로비저닝합니다. 기본 Direct Connect 연결이 실패할 경우 VPN 연결을 백업으로 프로비저닝합니다. 
B. 사설 연결을 위해 지역에 대한 VPN 터널 연결을 프로비저닝합니다. 기본 VPN 연결이 실패할 경우 비공개 연결 및 백업을 위한 두 번째 VPN 터널을 프로비저닝합니다. 
C. 리전에 대한 AWS Direct Connect 연결을 프로비저닝합니다. 기본 Direct Connect 연결이 실패할 경우 백업과 동일한 리전에 대한 두 번째 Direct Connect 연결을 프로비저닝합
니다.
D. 리전에 대한 AWS Direct Connect 연결을 프로비저닝합니다. AWS CLI에서 Direct Connect 장애 조치 속성을 사용하여 기본 Direct Connect 연결이 실패할 경우 백업 연결을
자동으로 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q176
회사는 계약 문서를 보관해야 합니다. 계약은 5년 동안 지속됩니다. 회사는 5년 동안 문서를 덮어쓰거나 삭제할 수 없도록 해야 합니다. 회사는 미사용 문서를 암호화하고 매년 암호화 키를 자 동으로 교체해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하기 위해 솔루션 설계자가 수행해야 하는 단계 조합은 무엇입니까? (두 가지를 선택하세요.)
A. Amazon S3에 문서를 저장합니다. 거버넌스 모드에서 S3 객체 잠금을 사용합니다. 
B. Amazon S3에 문서를 저장합니다. 규정 준수 모드에서 S3 객체 잠금을 사용합니다. 
C. Amazon S3 관리형 암호화 키(SSE-S3)로 서버 측 암호화를 사용합니다. 키 순환을 구성합니다. 
D. AWS Key Management Service(AWS KMS) 고객 관리형 키로 서버 측 암호화를 사용합니다. 키 순환을 구성합니다. 
E. AWS Key Management Service(AWS KMS) 고객 제공(가져온) 키로 서버 측 암호화를 사용합니다. 키 순환을 구성합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q177
회사에서 기존 3계층 웹 아키텍처의 비용을 줄이고자 합니다. 웹, 애플리케이션 및 데이터베이스 서버는 개발, 테스트 및 프로덕션 환경을 위해 Amazon EC2 인스턴스에서 실행됩니다. EC2 인스턴스는 사용량이 많은 시간에 평균 30%의 CPU 사용률을 보이고 사용량이 적은 시간에는 10%의 CPU 사용률을 보입니다. 프로덕션 EC2 인스턴스는 하루 24시간 실행됩니다. 개발 및 테스트 EC2 인스턴스는 매일 최소 8시간 동안 실행됩니다. 이 회사는 개발을 중지하고 사용하지 않는 EC2 인스턴스를 테스트 하기 위해 자동화를 구현할 계획입니다. 어떤 EC2 인스턴스 구매 솔루션이 회사의 요구 사항을 가장 비용 효율적으로 충족합니까?
A. 프로덕션 EC2 인스턴스에는 스팟 인스턴스를 사용하십시오. 개발 및 테스트 EC2 인스턴스에 예약 인스턴스를 사용합니다. 
B. 프로덕션 EC2 인스턴스에 예약 인스턴스를 사용합니다. 개발 및 테스트 EC2 인스턴스에 온디맨드 인스턴스를 사용합니다. 
C. 프로덕션 EC2 인스턴스에 스팟 블록을 사용합니다. 개발 및 테스트 EC2 인스턴스에 예약 인스턴스를 사용합니다. 
D. 프로덕션 EC2 인스턴스에 온디맨드 인스턴스를 사용합니다. 개발 및 테스트 EC2 인스턴스에 스팟 블록을 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q178
솔루션 아키텍트는 두 개의 퍼블릭 서브넷과 두 개의 프라이빗 서브넷이 포함된 VPC를 설정합니다. 기업 보안 규정에 따라 모든 Amazon EC2 인스턴스는 프라이빗 서브넷 내에서 시작되어 야 합니다. 그러나 솔루션 아키텍트가 프라이빗 서브넷 내의 포트 80 및 443에서 웹 서버를 호스팅하는 EC2 인스턴스를 시작하면 외부 인터넷 트래픽이 서버에 연결할 수 없습니다. 이 문제를 해결하기 위해 솔루션 설계자는 어떤 조치를 취해야 합니까?
A. EC2 인스턴스를 프라이빗 서브넷 내의 Auto Scaling 그룹에 연결합니다. 웹사이트의 DNS 레코드가 Auto Scaling 그룹 식별자로 확인되는지 확인하세요. 
B. 퍼블릭 서브넷 내에 인터넷 연결 Application Load Balancer(ALB)를 배포합니다. ALB와 연결된 대상 그룹에 EC2 인스턴스를 추가합니다. 웹 사이트의 DNS 레코드가 ALB로 확
인되는지 확인하세요.
C. 프라이빗 서브넷 내에 NAT 게이트웨이를 설정합니다. 프라이빗 서브넷의 라우팅 테이블을 업데이트하여 NAT 게이트웨이에 기본 경로를 추가합니다. NAT 게이트웨이에 공용 탄력적 IP
주소를 연결합니다.
D. EC2 인스턴스에 연결된 보안 그룹이 포트 80의 HTTP 트래픽과 포트 443의 HTTPS 트래픽을 허용하는지 확인합니다. 웹 사이트의 DNS 레코드가 EC2 인스턴스의 퍼블릭 IP 주소
로 확인되는지 확인합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q179
회사의 IT 비용에 대한 최근 분석에서는 백업 비용을 줄여야 할 필요성이 강조되었습니다. 회사의 최고 정보 책임자는 온프레미스 백업 인프라를 단순화하고 물리적 백업 테이프 사용을 제거하 여 비용을 절감하고자 합니다. 회사는 온프레미스 백업 애플리케이션 및 워크플로우에 대한 기존 투자를 보존해야 합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. NFS 인터페이스를 사용하여 백업 애플리케이션과 연결하도록 AWS Storage Gateway를 설정합니다. 
B. NFS 인터페이스를 사용하여 백업 애플리케이션과 연결하는 Amazon EFS 파일 시스템을 설정합니다. 
C. iSCSI 인터페이스를 사용하여 백업 애플리케이션과 연결하는 Amazon EFS 파일 시스템을 설정합니다. 
D. iSCSI-가상 테이프 라이브러리(VTL) 인터페이스를 사용하여 백업 애플리케이션과 연결하도록 AWS Storage Gateway를 설정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q180
한 회사가 Application Load Balancer를 사용하여 세 개의 AWS 지역에 애플리케이션을 배포하고 있습니다. Amazon Route 53은 이들 지역 간에 트래픽을 분산하는 데 사용됩니다 . 솔루션 아키텍트는 MOST 고성능 경험을 제공하기 위해 어떤 Route 53 구성을 사용해야 합니까?
A. 대기 시간 정책이 포함된 A 레코드를 생성합니다. 
B. 지리적 위치 정책을 사용하여 A 레코드를 만듭니다. 
C. 장애 조치 정책을 사용하여 CNAME 레코드를 생성합니다. 
D. 지리 근접 정책을 사용하여 CNAME 레코드를 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q181
회사의 애플리케이션은 여러 가용 영역에 있는 Amazon EC2 인스턴스에서 실행됩니다. 애플리케이션은 타사 애플리케이션에서 실시간 데이터를 수집해야 합니다. 회사에는 수집된 원시 데 이터를 Amazon S3 버킷에 배치하는 데이터 수집 솔루션이 필요합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 데이터 수집을 위해 Amazon Kinesis 데이터 스트림을 생성합니다. Kinesis 데이터 스트림을 사용하기 위해 Amazon Kinesis Data Firehose 전송 스트림을 생성합니다. S3 버킷
을 전송 스트림의 대상으로 지정합니다.
B. AWS Database Migration Service(AWS DMS)에서 데이터베이스 마이그레이션 작업을 생성합니다. EC2 인스턴스의 복제 인스턴스를 소스 엔드포인트로 지정합니다. S3 버킷
을 대상 엔드포인트로 지정합니다. 기존 데이터를 마이그레이션하고 지속적인 변경 사항을 복제하도록 마이그레이션 유형을 설정합니다.
C. EC2 인스턴스에서 AWS DataSync 에이전트를 생성하고 구성합니다. EC2 인스턴스에서 S3 버킷으로 데이터를 전송하도록 DataSync 작업을 구성합니다. 
D. 데이터 수집을 위해 애플리케이션에 대한 AWS Direct Connect 연결을 생성합니다. Amazon Kinesis Data Firehose 전송 스트림을 생성하여 애플리케이션에서 직접 PUT 작업
을 사용합니다. S3 버킷을 전송 스트림의 대상으로 지정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q182
회사에서 데이터 저장을 위해 Amazon DynamoDB 테이블을 사용할 계획입니다. 회사는 비용 최적화에 관심이 있습니다. 테이블은 대부분의 아침에 사용되지 않습니다. 저녁에는 읽기 및 쓰기 트래픽을 예측할 수 없는 경우가 많습니다. 트래픽 급증이 발생하면 매우 빠르게 발생합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. 온디맨드 용량 모드에서 DynamoDB 테이블을 생성합니다. 
B. 글로벌 보조 인덱스가 있는 DynamoDB 테이블을 생성합니다. 
C. 프로비저닝된 용량과 Auto Scaling으로 DynamoDB 테이블을 생성합니다. 
D. 프로비저닝된 용량 모드에서 DynamoDB 테이블을 생성하고 글로벌 테이블로 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q183
회사는 Amazon EC2 인스턴스에서 Java 기반 작업을 실행합니다. 작업은 매시간 실행되며 실행하는 데 10초가 걸립니다. 작업은 예약된 간격으로 실행되며 1GB의 메모리를 사용합니다. 작업이 사용 가능한 최대 CPU를 사용하는 짧은 순간을 제외하고 인스턴스의 CPU 사용률은 낮습니다. 회사는 작업 실행 비용을 최적화하려고 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS App2Container(A2C)를 사용하여 작업을 컨테이너화합니다. 0.5 vCPU(가상 CPU) 및 1GB 메모리를 사용하여 AWS Fargate에서 Amazon Elastic Container
Service(Amazon ECS) 작업으로 작업을 실행합니다.
B. 메모리가 1GB인 AWS Lambda 함수에 코드를 복사합니다. Amazon EventBridge 예약 규칙을 생성하여 매시간 코드를 실행합니다. 
C. AWS App2Container(A2C)를 사용하여 작업을 컨테이너화합니다. 기존 Amazon Machine Image(AMI)에 컨테이너를 설치합니다. 태스크가 완료되면 스케줄이 컨테이너를 중지
하는지 확인하십시오.
D. 작업 완료 시 EC2 인스턴스를 중지하고 다음 작업이 시작될 때 EC2 인스턴스를 다시 시작하도록 기존 일정을 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q184
응용 프로그램을 사용하면 회사 본사의 사용자가 제품 데이터에 액세스할 수 있습니다. 제품 데이터는 Amazon RDS MySQL DB 인스턴스에 저장됩니다. 운영 팀은 애플리케이션 성능 저 하를 격리했으며 쓰기 트래픽에서 읽기 트래픽을 분리하려고 합니다. 솔루션 설계자는 애플리케이션의 성능을 신속하게 최적화해야 합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. 기존 데이터베이스를 다중 AZ 배포로 변경합니다. 기본 가용 영역에서 읽기 요청을 처리합니다. 
B. 기존 데이터베이스를 다중 AZ 배포로 변경합니다. 보조 가용 영역에서 읽기 요청을 처리합니다. 
C. 데이터베이스에 대한 읽기 전용 복제본을 생성합니다. 컴퓨팅 및 스토리지 리소스의 절반을 원본 데이터베이스로 사용하여 읽기 전용 복제본을 구성합니다. 
D. 데이터베이스에 대한 읽기 전용 복제본을 생성합니다. 소스 데이터베이스와 동일한 컴퓨팅 및 스토리지 리소스로 읽기 전용 복제본을 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q185
회사에 여행 발권을 위한 웹 애플리케이션이 있습니다. 이 애플리케이션은 북미 지역의 단일 데이터 센터에서 실행되는 데이터베이스를 기반으로 합니다. 회사는 글로벌 사용자 기반에 서비스 를 제공하기 위해 응용 프로그램을 확장하려고 합니다. 회사는 애플리케이션을 여러 AWS 리전에 배포해야 합니다. 예약 데이터베이스 업데이트 시 평균 대기 시간은 1초 미만이어야 합니다. 이 회사는 여러 지역에 걸쳐 웹 플랫폼을 별도로 배포하려고 합니다. 그러나 회사는 전 세계적으로 일관된 단일 기본 예약 데이터베이스를 유지해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 어떤 솔루션을 권장해야 합니까?
A. 데이터베이스를 Amazon Aurora MySQL 데이터베이스로 마이그레이션합니다. 각 지역에 Aurora 읽기 전용 복제본을 배포합니다. 데이터베이스에 액세스하려면 각 지역 배포에서 올
바른 지역 엔드포인트를 사용하세요.
B. 데이터베이스를 Amazon RDS for MySQL 데이터베이스로 마이그레이션합니다. 각 리전에 MySQL 읽기 전용 복제본을 배포합니다. 데이터베이스에 액세스하려면 각 지역 배포에서
올바른 지역 엔드포인트를 사용하세요.
C. Amazon DynamoDB를 사용하도록 애플리케이션을 변환합니다. 중앙 예약 테이블에 전역 테이블을 사용합니다. 각 지역 배포에서 올바른 지역 엔드포인트를 사용합니다.
D. 애플리케이션을 Amazon Aurora Serverless 데이터베이스로 마이그레이션합니다. 각 지역에 데이터베이스 인스턴스를 배포합니다. 각 지역 배포에서 올바른 지역 엔드포인트를 사용
하여 데이터베이스에 액세스합니다. AWS Lambda 함수를 사용하여 각 리전에서 이벤트 스트림을 처리하여 데이터베이스를 동기화합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q186
한 회사에서 모바일 장치용 멀티플레이어 게임을 배포했습니다. 이 게임에는 위도와 경도를 기반으로 플레이어의 실시간 위치 추적이 필요합니다. 게임의 데이터 저장소는 신속한 업데이트와 위치 검색을 지원해야 합니다. 이 게임은 읽기 전용 복제본이 있는 PostgreSQL DB 인스턴스용 Amazon RDS를 사용하여 위치 데이터를 저장합니다. 사용량이 가장 많은 기간에는 데이터베이스가 업데이트를 읽고 쓰 는 데 필요한 성능을 유지할 수 없습니다. 게임의 사용자 기반이 빠르게 증가하고 있습니다. 데이터 계층의 성능을 향상하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 기존 DB 인스턴스의 스냅샷을 찍습니다. 다중 AZ가 활성화된 스냅샷을 복원합니다. 
B. Kibana를 사용하여 Amazon RDS에서 Amazon Elasticsearch Service(Amazon ES)로 마이그레이션합니다. 
C. 기존 DB 인스턴스 앞에 Amazon DynamoDB Accelerator(DAX)를 배포합니다. DAX를 사용하도록 게임을 수정합니다. 
D. 기존 DB 인스턴스 앞에 Redis용 Amazon ElastiCache 클러스터를 배포합니다. Redis를 사용하도록 게임을 수정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q187
한 금융 서비스 회사는 두 개의 데이터 센터를 폐쇄하고 100TB가 넘는 데이터를 AWS로 마이그레이션하려고 합니다. 데이터는 하위 폴더의 깊은 계층 구조로 구성된 수백만 개의 작은 파일 을 포함하는 복잡한 디렉터리 구조를 가지고 있습니다. 대부분의 데이터는 구조화되지 않았으며 회사의 파일 스토리지에는 다양한 공급업체의 SMB 기반 스토리지 유형이 포함되어 있습니다. 회사는 마이그레이션 후 데이터에 액세스하기 위해 애플리케이션을 변경하지 않기를 원합니다. 솔루션 설계자는 운영 오버헤드를 최소화하면서 이러한 요구 사항을 충족하기 위해 어떤 접근 방식을 취해야 합니까?
A. AWS Direct Connect를 활용하여 데이터를 Amazon S3로 마이그레이션합니다.
B. AWS DataSync를 사용하여 데이터를 Amazon FSx for Lustre로 마이그레이션합니다.
C. AWS DataSync를 사용하여 Windows 파일 서버용 Amazon FSx로 데이터를 전송합니다.
D. AWS Direct Connect를 사용하여 온프레미스 파일 스토리지를 AWS Storage Gateway 볼륨 게이트웨이로 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q188
한 회사가 다년간의 마이그레이션 프로젝트 중에 데이터와 애플리케이션을 AWS로 이전하고 있습니다. 회사는 회사의 AWS 리전과 회사의 온프레미스 위치에서 Amazon S3의 데이터에 안전하게 액세스하려고 합니다. 데이터가 인터넷을 통과해서는 안 됩니다. 회사는 해당 지역과 온프레미스 위치 간에 AWS Direct Connect 연결을 설정했습니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon S3용 게이트웨이 엔드포인트를 생성합니다. 게이트웨이 엔드포인트를 사용하여 지역 및 온프레미스 위치의 데이터에 안전하게 액세스하세요.
B. AWS Transit Gateway에 게이트웨이를 생성하여 리전 및 온프레미스 위치에서 Amazon S3에 안전하게 액세스합니다.
C. Amazon S3용 인터페이스 엔드포인트를 생성합니다. 인터페이스 엔드포인트를 사용하여 지역 및 온프레미스 위치의 데이터에 안전하게 액세스하세요.
D. AWS Key Management Service(AWS KMS) 키를 사용하여 지역 및 온프레미스 위치에서 데이터에 안전하게 액세스합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q189
회사는 Amazon DynamoDB를 사용하여 고객 정보를 저장하는 쇼핑 애플리케이션을 실행합니다. 데이터 손상의 경우 솔루션 설계자는 15분의 RPO(복구 지점 목표)와 1시간의 RTO(복 구 시간 목표)를 충족하는 솔루션을 설계해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. DynamoDB 전역 테이블을 구성합니다. RPO 복구의 경우 애플리케이션이 다른 AWS 리전을 가리키도록 합니다. 
B. DynamoDB 특정 시점으로 복구를 구성합니다. RPO 복구를 위해 원하는 시점으로 복원합니다. 
C. 매일 DynamoDB 데이터를 Amazon S3 Glacier로 내보냅니다. RPO 복구를 위해 S3 Glacier에서 DynamoDB로 데이터를 가져옵니다. 
D. 15분마다 DynamoDB 테이블에 대한 Amazon Elastic Block Store(Amazon EBS) 스냅샷을 예약합니다. RPO 복구의 경우 EBS 스냅샷을 사용하여 DynamoDB 테이블을 복
원합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q190
한 회사가 Amazon RDS 데이터베이스를 사용하여 Amazon EC2 인스턴스에 애플리케이션을 배포했습니다. 회사는 최소 권한 원칙을 사용하여 데이터베이스 액세스 자격 증명을 구성했 습니다. 회사의 보안 팀은 SQL 주입 및 기타 웹 기반 공격으로부터 애플리케이션과 데이터베이스를 보호하려고 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇 입니까?
A. 보안 그룹과 네트워크 ACL을 사용하여 데이터베이스와 애플리케이션 서버를 보호하십시오. 
B. AWS WAF를 사용하여 애플리케이션을 보호하십시오. RDS 매개변수 그룹을 사용하여 보안 설정을 구성합니다. 
C. AWS 네트워크 방화벽을 사용하여 애플리케이션과 데이터베이스를 보호하십시오. 
D. 다양한 기능을 위해 애플리케이션 코드에서 다양한 데이터베이스 계정을 사용합니다. 데이터베이스 사용자에게 과도한 권한을 부여하지 마십시오.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q191
회사는 AWS 클라우드에서 3계층 웹 애플리케이션을 호스팅합니다. MySQL용 다중 AZAmazon RDS 서버는 데이터베이스 계층을 형성합니다. Amazon ElastiCache는 캐시 계층을 형성합니다. 회사는 고객이 데이터베이스에 항목을 추가할 때 캐시의 데이터를 추가하거나 업데이트하는 캐싱 전략을 원합니다. 캐시의 데이터는 항상 데이터베이스의 데이터와 일치해야 합니 다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 지연 로딩 캐싱 전략 구현
B. write-through 캐싱 전략 구현
C. 추가 TTL 캐싱 전략 구현
D. AWS AppConfig 캐싱 전략 구현

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q192
한 회사가 테스트 환경에서 자사 애플리케이션을 위한 AWS CloudFormation 스택을 사용하려고 합니다. 이 회사는 공개 액세스를 차단하는 Amazon S3 버킷에 CloudFormation 템플 릿을 저장하고 있습니다. 회사는 CloudFormation에게 특정 사용자 요청을 기반으로 S3 버킷의 템플릿에 액세스 권한을 부여하려고 합니다. 이 솔루션은 보안 최상의 실천 방법을 준수해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon S3에 대한 게이트웨이 VPC 엔드포인트를 생성합니다. CloudFormation 스택을 S3 오브젝트 URL을 사용하도록 구성합니다. 
B. Amazon API Gateway REST API를 생성하고 해당 API를 S3 버킷을 대상으로 설정합니다. CloudFormation 스택을 API Gateway URL을 사용하도록 구성합니다. 
C. 템플릿 오브젝트에 대한 사전 서명된 URL을 생성합니다. CloudFormation 스택을 사전 서명된 URL을 사용하도록 구성합니다. 
D. S3 버킷에서 템플릿 오브젝트에 대한 공개 액세스를 허용합니다. 테스트 환경이 생성된 후에는 공개 액세스를 차단합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q193
한 회사가 AWS에 최신 제품을 배포했습니다. 제품은 Network Load Balancer 뒤의 Auto Scaling 그룹에서 실행됩니다. 회사는 제품의 객체를 Amazon S3 버킷에 저장합니다. 이 회사는 최근 자사 시스템에 대한 악의적인 공격을 경험했습니다. 회사에는 AWS 계정의 악의적인 활동, 워크로드 및 S3 버킷에 대한 액세스 패턴을 지속적으로 모니터링하는 솔루션이 필 요합니다. 또한 솔루션은 의심스러운 활동을 보고하고 대시보드에 정보를 표시해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 결과를 모니터링하고 AWS Config에 보고하도록 Amazon Macie를 구성합니다. 
B. 결과를 모니터링하고 AWS CloudTrail에 보고하도록 Amazon Inspector를 구성합니다. 
C. 결과를 모니터링하고 AWS Security Hub에 보고하도록 Amazon GuardDuty를 구성합니다. 
D. 결과를 모니터링하고 Amazon EventBridge에 보고하도록 AWS Config를 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q194
회사는 Application Load Balancer 뒤의 Amazon EC2 인스턴스에서 비즈니스 크리티컬 웹 애플리케이션을 실행하고 있습니다. EC2 인스턴스는 Auto Scaling 그룹에 있습니다. 애 플리케이션은 단일 가용 영역에 배포된 Amazon Aurora PostgreSQL 데이터베이스를 사용합니다. 회사는 가동 중지 시간을 최소화하고 데이터 손실을 최소화하면서 애플리케이션의 가용 성을 높이길 원합니다. 최소한의 운영 노력으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 다른 AWS 지역에 EC2 인스턴스를 배치하십시오. Amazon Route 53 상태 확인을 사용하여 트래픽을 리디렉션합니다. Aurora PostgreSQL 교차 리전 복제를 사용합니다. 
B. 여러 가용 영역을 사용하도록 Auto Scaling 그룹을 구성합니다. 데이터베이스를 다중 AZ로 구성합니다. 데이터베이스에 대한 Amazon RDS Proxy 인스턴스를 구성합니다. 
C. 하나의 가용 영역을 사용하도록 Auto Scaling 그룹을 구성합니다. 데이터베이스의 시간별 스냅샷을 생성합니다. 장애 발생 시 스냅샷에서 데이터베이스를 복구합니다. 
D. 여러 AWS 리전을 사용하도록 Auto Scaling 그룹을 구성합니다. 애플리케이션의 데이터를 Amazon S3에 씁니다. S3 이벤트 알림을 사용하여 데이터베이스에 데이터를 쓰는 AWS
Lambda 함수를 시작합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q195
한 회사는 최근 해양 조사에서 얻은 200TB의 데이터를 AWS Snowball Edge Storage Optimized 디바이스에 복사합니다. 이 회사는 석유 및 가스 매장지를 찾기 위해 AWS에 호스팅 되는 고성능 컴퓨팅(HPC) 클러스터를 보유하고 있습니다. 솔루션 아키텍트는 Snowball Edge Storage Optimized 디바이스의 데이터에 대한 일관된 밀리초 미만의 지연 시간과 높은 처 리량 액세스를 클러스터에 제공해야 합니다. 회사는 디바이스를 AWS로 다시 보내고 있습니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon S3 버킷을 생성합니다. 데이터를 S3 버킷으로 가져옵니다. S3 버킷을 사용하도록 AWS Storage Gateway 파일 게이트웨이를 구성합니다. HPC 클러스터 인스턴스에서
파일 게이트웨이에 액세스합니다.
B. Amazon S3 버킷을 생성합니다. 데이터를 S3 버킷으로 가져옵니다. Lustre 파일 시스템용 Amazon FSx를 구성하고 이를 S3 버킷과 통합합니다. HPC 클러스터 인스턴스에서
FSx for Lustre 파일 시스템에 액세스합니다.
C. Amazon S3 버킷과 Amazon Elastic File System(Amazon EFS) 파일 시스템을 생성합니다. 데이터를 S3 버킷으로 가져옵니다. S3 버킷의 데이터를 EFS 파일 시스템에 복사
합니다. HPC 클러스터 인스턴스에서 EFS 파일 시스템에 액세스합니다.
D. Lustre 파일 시스템용 Amazon FSx를 생성합니다. 데이터를 FSx for Lustre 파일 시스템으로 직접 가져옵니다. HPC 클러스터 인스턴스에서 FSx for Lustre 파일 시스템에 액세
스합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q196
회사에서 이미지 처리를 위한 2계층 애플리케이션을 운영하고 있습니다. 애플리케이션은 각각 1개의 퍼블릭 서브넷과 1개의 프라이빗 서브넷이 있는 2개의 가용 영역을 사용합니다. 웹 계층용 ALB(Application Load Balancer)는 퍼블릭 서브넷을 사용합니다. 애플리케이션 계층의 Amazon EC2 인스턴스는 프라이빗 서브넷을 사용합니다. 사용자는 응용 프로그램이 예상보다 느리게 실행되고 있다고 보고합니다. 웹 서버 로그 파일의 보안 감사는 애플리케이션이 소수의 IP 주소로부터 수백만 건의 불법 요청을 수신하고 있음을 보 여줍니다. 솔루션 설계자는 회사가 보다 영구적인 솔루션을 조사하는 동안 즉각적인 성능 문제를 해결해야 합니다. 이 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. 웹 계층에 대한 인바운드 보안 그룹을 수정합니다. 리소스를 소비하는 IP 주소에 대한 거부 규칙을 추가합니다. 
B. 웹 계층 서브넷에 대한 네트워크 ACL을 수정합니다. 리소스를 소비하는 IP 주소에 대한 인바운드 거부 규칙을 추가합니다. 
C. 애플리케이션 계층에 대한 인바운드 보안 그룹을 수정합니다. 리소스를 소비하는 IP 주소에 대한 거부 규칙을 추가합니다. 
D. 애플리케이션 계층 서브넷에 대한 네트워크 ACL을 수정합니다. 리소스를 소비하는 IP 주소에 대한 인바운드 거부 규칙을 추가합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q197
개발팀이 다른 회사와 협력하여 통합 제품을 만들고 있습니다. 다른 회사는 개발 팀의 계정에 포함된 Amazon Simple Queue Service(Amazon SQS) 대기열에 액세스해야 합니다. 다른 회사는 자신의 계정 권한을 포기하지 않고 대기열을 폴링하려고 합니다. 솔루션 설계자는 SQS 대기열에 대한 액세스를 어떻게 제공해야 합니까?
A. 다른 회사에 SQS 대기열에 대한 액세스를 제공하는 인스턴스 프로필을 생성합니다. 
B. SQS 대기열에 대한 다른 회사 액세스를 제공하는 IAM 정책을 생성합니다. 
C. SQS 대기열에 대한 다른 회사 액세스를 제공하는 SQS 액세스 정책을 만듭니다. 
D. 다른 회사에 SQS 대기열에 대한 액세스를 제공하는 Amazon Simple 알림 서비스(Amazon SNS) 액세스 정책을 생성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q198
회사는 확장성 및 가용성에 대한 요구 사항을 충족하기 위해 컨테이너에서 중요한 애플리케이션을 실행하려고 합니다. 회사는 중요한 응용 프로그램의 유지 관리에 집중하는 것을 선호합니다. 회사는 컨테이너화된 워크로드를 실행하는 기본 인프라를 프로비저닝하고 관리하는 책임을 원하지 않습니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Amazon EC2 인스턴스를 사용하고 인스턴스에 Docker를 설치하십시오. 
B. Amazon EC2 작업자 노드에서 Amazon Elastic Container Service(Amazon ECS)를 사용합니다. 
C. AWS Fargate에서 Amazon Elastic Container Service(Amazon ECS)를 사용합니다. 
D. Amazon Elastic Container Service(Amazon ECS)에 최적화된 Amazon Machine Image(AMI)에서 Amazon EC2 인스턴스를 사용합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q199
한 게임 회사가 여러 AWS 리전에서 새로운 인터넷 연결 애플리케이션을 출시하려고 합니다. 애플리케이션은 통신을 위해 TCP 및 UDP 프로토콜을 사용합니다. 회사는 글로벌 사용자에게 고가용성과 최소 대기 시간을 제공해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 조치 조합을 취해야 합니까? (2개를 선택하세요.)
A. 각 리전의 애플리케이션 앞에 내부 Network Load Balancer를 생성합니다. 
B. 각 지역의 애플리케이션 앞에 외부 Application Load Balancer를 생성합니다. 
C. AWS Global Accelerator 액셀러레이터를 생성하여 각 리전의 로드 밸런서로 트래픽을 라우팅합니다. 
D. 지리적 위치 라우팅 정책을 사용하여 트래픽을 분산하도록 Amazon Route 53을 구성합니다. 
E. 트래픽을 처리하고 각 지역의 애플리케이션에 대한 요청을 라우팅하도록 Amazon CloudFront를 구성합니다.

<details>
<summary>정답 보기</summary>

**BC**
</details>

---

### Q200
소매 회사에는 여러 비즈니스가 있습니다. 각 비즈니스의 IT 팀은 자체 AWS 계정을 관리합니다. 각 팀 계정은 AWS Organizations에서 조직의 일부입니다. 각 팀은 팀 자체 AWS 계정의 Amazon DynamoDB 테이블에서 제품 재고 수준을 모니터링합니다. 회사는 공유 AWS 계정에 중앙 재고 보고 애플리케이션을 배포하고 있습니다. 애플리케이션은 모든 팀의 DynamoDB 테이블에서 항목을 읽을 수 있어야 합니다. 이러한 요구 사항을 가장 안전하게 충족하는 인증 옵션은 무엇입니까?
A. 인벤토리 애플리케이션 계정에서 DynamoDB를 AWS Secrets Manager와 통합합니다. Secrets Manager의 올바른 암호를 사용하여 DynamoDB 테이블을 인증하고 읽도록 애
플리케이션을 구성합니다. 30일마다 비밀 순환을 예약합니다.
B. 모든 비즈니스 계정에서 프로그래(cid:1535) 방식 액세스 권한이 있는 IAM 사용자를 생성합니다. 올바른 IAM 사용자 액세스 키 ID와 보안 액세스 키를 사용하여 DynamoDB 테이블을 인증하
고 읽도록 애플리케이션을 구성합니다. 30일마다 IAM 액세스 키를 수동으로 교체합니다.
C. 모든 비즈니스 계정에서 DynamoDB 테이블에 대한 역할 액세스 권한을 부여하는 정책과 인벤토리 애플리케이션 계정의 특정 역할을 신뢰하는 신뢰 정책을 사용하여 BU_ROLE이라는
IAM 역할을 생성합니다. 인벤토리 계정에서 STS AssumeRole API 작업에 대한 액세스를 허용하는 APP_ROLE이라는 역할을 생성합니다. APP_ROLE을 사용하도록 애플리케이 션을 구성하고 DynamoDB 테이블을 읽기 위해 교차 계정 역할 BU_ROLE을 수임합니다.
D. DynamoDB를 AWS Certificate Manager(ACM)와 통합합니다. DynamoDB를 인증하기 위해 ID 인증서를 생성합니다. 올바른 인증서를 사용하여 DynamoDB 테이블을 인증
하고 읽도록 애플리케이션을 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q201
회사에는 공통 Amazon RDS MySQL 다중 AZ DB 인스턴스에 자주 액세스해야 하는 여러 웹 서버가 있습니다. 회사는 사용자 자격 증명을 자주 교체해야 하는 보안 요구 사항을 충족하면 서 웹 서버가 데이터베이스에 연결할 수 있는 안전한 방법을 원합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS Secrets Manager에 데이터베이스 사용자 자격 증명을 저장합니다. 웹 서버가 AWS Secrets Manager에 액세스할 수 있도록 필요한 IAM 권한을 부여합니다. 
B. AWS Systems Manager OpsCenter에 데이터베이스 사용자 자격 증명을 저장합니다. 웹 서버가 OpsCenter에 액세스할 수 있도록 필요한 IAM 권한을 부여합니다. 
C. 안전한 Amazon S3 버킷에 데이터베이스 사용자 자격 증명을 저장합니다. 웹 서버가 자격 증명을 검색하고 데이터베이스에 액세스할 수 있도록 필요한 IAM 권한을 부여합니다. 
D. 웹 서버 파일 시스템에서 AWS KMS(AWS Key Management Service)로 암호화된 파일에 데이터베이스 사용자 자격 증명을 저장합니다. 웹 서버는 파일을 해독하고 데이터베이스
에 액세스할 수 있어야 합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q202
한 회사에는 다음 달 내에 AWS 클라우드로 이동해야 하는 150TB의 보관된 이미지 데이터가 온프레미스에 저장되어 있습니다. 회사의 현재 네트워크 연결은 야간에만 이 목적으로 최대 100Mbps의 업로드를 허용합니다. 이 데이터를 이동하고 마이그레이션 기한을 맞추는 가장 비용 효율적인 메커니즘은 무엇입니까?
A. AWS Snowmobile을 사용하여 AWS로 데이터를 전송합니다. 
B. 여러 AWS Snowball 장치를 주문하여 AWS로 데이터를 전송합니다. 
C. Amazon S3 Transfer Acceleration을 활성화하고 데이터를 안전하게 업로드합니다. 
D. Amazon S3 VPC 엔드포인트를 생성하고 VPN을 설정하여 데이터를 업로드합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q203
솔루션 설계자는 건물 내 비즈니스 테넌트의 시간당 에너지 소비량을 저장할 워크로드를 설계하고 있습니다. 센서는 각 테넌트의 사용량을 합산하는 HTTP 요청을 통해 데이터베이스에 공급 합니다. 솔루션 설계자는 가능한 경우 관리 서비스를 사용해야 합니다. 워크로드는 솔루션 설계자가 독립적인 구성 요소를 추가함에 따라 향후 더 많은 기능을 받게 됩니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Lambda 함수와 함께 Amazon API Gateway를 사용하여 센서에서 데이터를 수신하고, 데이터를 처리하고, Amazon DynamoDB 테이블에 데이터를 저장합니다. 
B. Amazon EC2 인스턴스의 Auto Scaling 그룹에서 지원하는 Elastic Load Balancer를 사용하여 센서에서 데이터를 수신하고 처리합니다. Amazon S3 버킷을 사용하여 처리된 데
이터를 저장합니다.
C. AWS Lambda 함수와 함께 Amazon API Gateway를 사용하여 센서에서 데이터를 수신하고, 데이터를 처리하고, Amazon EC2 인스턴스의 Microsoft SQL Server Express
데이터베이스에 데이터를 저장합니다.
D. Amazon EC2 인스턴스의 Auto Scaling 그룹에서 지원하는 Elastic Load Balancer를 사용하여 센서에서 데이터를 수신하고 처리합니다. Amazon Elastic File System
(Amazon EFS) 공유 파일 시스템을 사용하여 처리된 데이터를 저장합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q204
회사는 여러 가용 영역에 걸쳐 VPC에서 3계층 웹 애플리케이션을 실행합니다. Amazon EC2 인스턴스는 애플리케이션 계층에 대한 Auto Scaling 그룹에서 실행됩니다. 회사는 각 리소스의 일일 및 주간 기록 워크로드 추세를 분석하는 자동화된 확장 계획을 수립해야 합니다. 구성은 활용도의 예측 및 실시간 변화에 따라 리소스를 적절하게 확장해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 확장 전략을 권장해야 합니까?
A. EC2 인스턴스의 평균 CPU 사용률을 기준으로 단계 조정을 통해 동적 조정을 구현합니다. 
B. 예측 및 확장을 위해 예측 확장을 활성화합니다. 대상 추적을 사용하여 동적 조정을 구성합니다. 
C. 웹 애플리케이션의 트래픽 패턴을 기반으로 자동화된 예약 조정 작업을 생성합니다. 
D. 간단한 확장 정책을 설정합니다. EC2 인스턴스 시작 시간을 기준으로 휴지 기간을 늘립니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q205
회사는 Amazon Elastic Kubernetes Service(Amazon EKS) 및 Kubernetes Horizontal Pod Autoscaler를 사용하여 컨테이너 애플리케이션을 실행합니다. 작업량은 하루 종일 일정하지 않습니다. 솔루션 설계자는 기존 노드가 클러스터의 최대 용량에 도달했을 때 노드 수가 자동으로 확장되지 않아 성능 문제가 발생한다는 사실을 알게 됩니다. 최소한의 관리 오버헤드 로 이 문제를 해결하는 솔루션은 무엇입니까?
A. 메모리 사용량을 추적하여 노드를 확장합니다.
B. Kubernetes Cluster Autoscaler를 사용하여 클러스터의 노드 수를 관리합니다.
C. AWS Lambda 함수를 사용하여 EKS 클러스터의 크기를 자동으로 조정합니다.
D. Amazon EC2 Auto Scaling 그룹을 사용하여 워크로드를 분산합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q206
한 회사에는 여러 AWS 지역의 Amazon EC2 인스턴스에 배포된 HTTP 기반 애플리케이션에 액세스하는 전 세계 사용자가 있습니다. 회사는 애플리케이션의 가용성과 성능을 개선하려고 합니다. 또한 회사는 가용성에 영향을 미치거나, 보안을 손상시키거나, 과도한 리소스를 소비할 수 있는 일반적인 웹 공격으로부터 애플리케이션을 보호하려고 합니다. 고정 IP 주소가 필요합니 다. 이를 달성하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. 각 지역의 NLB(Network Load Balancer) 뒤에 EC2 인스턴스를 배치합니다. NLB에 AWS WAF를 배포합니다. AWS Global Accelerator를 사용하여 액셀러레이터를 생성하
고 NLB를 엔드포인트로 등록합니다.
B. 각 지역의 ALB(Application Load Balancer) 뒤에 EC2 인스턴스를 배치합니다. ALB에 AWS WAF를 배포합니다. AWS Global Accelerator를 사용하여 액셀러레이터를 생성
하고 ALB를 엔드포인트로 등록합니다.
C. 각 지역의 NLB(Network Load Balancer) 뒤에 EC2 인스턴스를 배치합니다. NLB에 AWS WAF를 배포합니다. Amazon Route 53 지연 시간 기반 라우팅을 사용하여 요청을
NLB로 라우팅하는 오리진으로 Amazon CloudFront 배포를 생성합니다.
D. 각 지역의 ALB(Application Load Balancer) 뒤에 EC2 인스턴스를 배치합니다. Amazon Route 53 지연 시간 기반 라우팅을 사용하여 요청을 ALB로 라우팅하는 오리진으로
Amazon CloudFront 배포를 생성합니다. CloudFront 배포에 AWS WAF를 배포합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q207
회사는 사용자가 업로드한 문서를 Amazon EBS 볼륨에 저장하는 단일 Amazon EC2 인스턴스를 사용하여 AWS에서 웹 애플리케이션을 호스팅하고 있습니다. 더 나은 확장성과 가용성 을 위해 회사는 아키텍처를 복제하고 다른 가용 영역에 두 번째 EC2 인스턴스와 EBS 볼륨을 생성하여 둘 다 Application Load Balancer 뒤에 배치했습니다. 이 변경을 완료한 후 사용자 는 웹 사이트를 새로 고칠 때마다 문서의 한 하위 집합 또는 다른 하위 집합을 볼 수 있지만 동시에 모든 문서를 볼 수는 없다고 보고했습니다. 사용자가 모든 문서를 한 번에 볼 수 있도록 하기 위해 솔루션 설계자는 무엇을 제안해야 합니까?
A. 두 EBS 볼륨에 모든 문서가 포함되도록 데이터를 복사합니다. 
B. 문서가 있는 서버로 사용자를 안내하도록 Application Load Balancer 구성 
C. 두 EBS 볼륨의 데이터를 Amazon EFS로 복사합니다. 새 문서를 Amazon EFS에 저장하도록 애플리케이션 수정 
D. 두 서버 모두에 요청을 보내도록 Application Load Balancer를 구성합니다. 올바른 서버에서 각 문서 반환

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q208
회사는 Amazon EC2에서 콘텐츠 관리 시스템(CMS)을 사용하는 웹 사이트를 운영합니다. CMS는 단일 EC2 인스턴스에서 실행되며 데이터 계층에 Amazon Aurora MySQL 다중 AZ DB 인스턴스를 사용합니다. 웹 사이트 이미지는 EC2 인스턴스 내부에 탑재된 Amazon Elastic Block Store(Amazon EBS) 볼륨에 저장됩니다. 웹 사이트의 성능과 복원력을 개선하기 위해 솔루션 설계자가 취해야 하는 작업 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 웹사이트 이미지를 모든 EC2 인스턴스에 탑재된 Amazon S3 버킷으로 이동합니다. 
B. 기본 EC2 인스턴스의 NFS 공유를 사용하여 웹사이트 이미지를 공유합니다. 이 공유를 다른 EC2 인스턴스에 마운트합니다. 
C. 모든 EC2 인스턴스에 탑재된 Amazon Elastic File System(Amazon EFS) 파일 시스템으로 웹 사이트 이미지를 이동합니다. 
D. 기존 EC2 인스턴스에서 Amazon 머신 이미지(AMI)를 생성합니다. AMI를 사용하여 Auto Scaling 그룹의 일부로 Application Load Balancer 뒤에 새 인스턴스를 프로비저닝합
니다. 최소 2개의 인스턴스를 유지하도록 Auto Scaling 그룹을 구성합니다. 웹사이트용 AWS Global Accelerator에서 액셀러레이터 구성
E. 기존 EC2 인스턴스에서 Amazon 머신 이미지(AMI)를 생성합니다. AMI를 사용하여 Auto Scaling 그룹의 일부로 Application Load Balancer 뒤에 새 인스턴스를 프로비저닝합
니다. 최소 2개의 인스턴스를 유지하도록 Auto Scaling 그룹을 구성합니다. 웹 사이트에 대한 Amazon CloudFront 배포를 구성합니다.

<details>
<summary>정답 보기</summary>

**CE**
</details>

---

### Q209
회사는 온프레미스 LDAP 디렉터리 서비스를 사용하여 AWS Management Console에 사용자를 인증해야 합니다. 디렉터리 서비스는 SAML(Security Assertion Markup Language)과 호환되지 않습니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS와 온프레미스 LDAP 간에 AWS IAM Identity Center(AWS Single Sign-On)를 활성화합니다. 
B. AWS 자격 증명을 사용하는 IAM 정책을 생성하고 정책을 LDAP에 통합합니다. 
C. LDAP 자격 증명이 업데이트될 때마다 IAM 자격 증명을 교체하는 프로세스를 설정합니다. 
D. AWS Security Token Service(AWS STS)를 사용하여 단기 자격 증명을 얻는 온프레미스 사용자 지정 자격 증명 브로커 애플리케이션 또는 프로세스를 개발합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q210
회사에서 전자상거래 웹 사이트를 위한 다중 계층 애플리케이션을 만들었습니다. 웹사이트는 퍼블릭 서브넷에 상주하는 Application Load Balancer, 퍼블릭 서브넷의 웹 계층, 프라이빗 서 브넷의 Amazon EC2 인스턴스에서 호스팅되는 MySQL 클러스터를 사용합니다. MySQL 데이터베이스는 타사 공급자가 인터넷에서 호스팅하는 제품 카탈로그 및 가격 정보를 검색해야 합니다. 솔루션 설계자는 운영 오버헤드를 늘리지 않고 보안을 극대화하는 전략을 고안해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. VPC에 NAT 인스턴스를 배포합니다. NAT 인스턴스를 통해 모든 인터넷 기반 트래픽을 라우팅합니다. 
B. 퍼블릭 서브넷에 NAT 게이트웨이를 배포합니다. 인터넷 바인딩된 모든 트래픽을 NAT 게이트웨이로 보내도록 프라이빗 서브넷 라우팅 테이블을 수정합니다. 
C. 인터넷 게이트웨이를 구성하고 VPModify 프라이빗 서브넷 라우팅 테이블에 연결하여 인터넷 바인딩 트래픽을 인터넷 게이트웨이로 보냅니다. 
D. 가상 프라이빗 게이트웨이를 구성하고 VPC에 연결합니다. 인터넷 바인딩 트래픽을 가상 프라이빗 게이트웨이로 보내도록 프라이빗 서브넷 라우팅 테이블을 수정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q211
회사에서 온프레미스 PostgreSQL 데이터베이스를 Amazon RDS for PostgreSQL DB 인스턴스로 옮겼습니다. 회사는 신제품을 성공적으로 출시했습니다. 데이터베이스의 워크로드가 증가했습니다. 회사는 인프라를 추가하지 않고 더 큰 워크로드를 수용하려고 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 전체 워크로드에 대해 예약된 DB 인스턴스를 구매합니다. PostgreSQL DB 인스턴스용 Amazon RDS를 더 크게 만듭니다. 
B. Amazon RDS for PostgreSQL DB 인스턴스를 다중 AZ DB 인스턴스로 만듭니다. 
C. 총 워크로드에 대해 예약된 DB 인스턴스를 구매합니다. PostgreSQL DB 인스턴스용 다른 Amazon RDS를 추가합니다. 
D. Amazon RDS for PostgreSQL DB 인스턴스를 온디맨드 DB 인스턴스로 만듭니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q212
솔루션 아키텍트는 가용성이 뛰어난 Redis용 Amazon ElastiCache 기반 솔루션을 설계하고 있습니다. 솔루션 아키텍트는 장애로 인해 로컬 및 AWS 리전 내에서 성능 저하 또는 데이터 손실이 발생하지 않도록 해야 합니다. 솔루션은 노드 수준과 지역 수준에서 고가용성을 제공해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 여러 노드가 포함된 샤드가 있는 다중 AZ Redis 복제 그룹을 사용하십시오. 
B. Redis AOF(Append Only Files)가 활성화된 여러 노드가 포함된 Redis 샤드를 사용합니다. 
C. 복제 그룹에 두 개 이상의 읽기 전용 복제본이 있는 다중 AZ Redis 클러스터를 사용합니다. 
D. Auto Scaling이 활성화된 여러 노드가 포함된 Redis 샤드를 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q213
회사는 계정 관리를 위해 AWS Single Sign-On(AWS SSO) 및 AWS Control Tower를 활용하여 AWS Organizations에서 AWS 계정을 관리합니다. 회사는 모든 계정에 걸쳐 권 한 관리를 간소화하는 것을 목표로 합니다. 이러한 권한은 각각 고유한 권한이 필요한 개발자 및 관리자 팀에 할당되어야 합니다. 또한 회사는 어느 그룹에든 합류하는 새로운 팀원을 쉽게 수용 할 수 있는 솔루션을 원합니다. 이러한 요구 사항을 충족하면서 운영 오버헤드를 최소화하는 솔루션은 무엇입니까?
A. 각 계정에 대해 AWS Single Sign-On(AWS SSO) 내에서 개별 사용자를 생성합니다. AWS SSO에서 별도의 개발자 및 관리자 그룹을 설정하고 사용자를 해당 그룹에 할당합니다.
각 그룹에 대한 사용자 지정 IAM 정책을 만들어 세분화된 권한을 정의합니다.
B. 각 계정에 대해 AWS Single Sign-On(AWS SSO) 내에서 개별 사용자를 생성합니다. AWS SSO 내에 별도의 개발자 및 관리자 그룹을 설정하고 이에 따라 사용자를 할당합니다.
각 사용자에게 관련 AWS 관리형 IAM 정책을 연결하여 세분화된 권한을 부여합니다.
C. AWS Single Sign-On(AWS SSO) 내에서 개별 사용자를 생성합니다. AWS SSO 내에 새로운 개발자 및 관리자 그룹을 설정합니다. 각 그룹에 필요한 IAM 정책이 포함된 새 권한
세트를 생성합니다. 이러한 새 그룹을 해당 계정에 할당하고 권한 집합을 그룹에 할당합니다. 채용 시 적절한 그룹에 새로운 사용자를 추가합니다.
D. AWS Single Sign-On(AWS SSO) 내에서 개별 사용자를 생성합니다. 각 사용자에게 필요한 IAM 정책을 포함하는 특정 권한 세트를 생성합니다. 사용자를 해당 계정에 할당하고 특
정 계정 내에서 직접 추가 IAM 권한을 부여합니다. 신규 사용자를 고용하면 AWS SSO에 추가하고 관련 계정에 할당합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q214
한 회사에서 Amazon Elastic Kubernetes Service(Amazon EKS)에 배포할 마이크로서비스 기반 애플리케이션을 개발하고 있습니다. 이 애플리케이션 내의 마이크로서비스는 서로 원 활하게 상호 작용해야 합니다. 회사는 애플리케이션을 효과적으로 관찰하여 향후 성능 문제를 식별할 수 있도록 하는 것을 목표로 합니다. 이러한 요구 사항을 가장 잘 충족하는 솔루션은 무엇입니까?
A. Amazon ElastiCache를 활용하여 마이크로서비스로 전달되는 요청 수를 최소화하도록 애플리케이션을 구성합니다. 
B. Amazon CloudWatch Container Insights를 설정하여 EKS 클러스터에서 지표를 수집하고 AWS X-Ray를 사용하여 마이크로서비스 간 요청을 추적합니다. 
C. AWS CloudTrail을 설정하여 API 호출을 모니터링하고 마이크로서비스 상호 작용을 관찰하기 위한 Amazon QuickSight 대시보드를 구성합니다. 
D. AWS Trusted Advisor를 활용하여 애플리케이션 성능을 분석합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q215
한 회사가 AWS에서 새로운 기계 학습(ML) 모델 솔루션을 개발하고 있습니다. 모델은 시작 시 Amazon S3에서 약 1GB의 모델 데이터를 가져와 메모리에 로드하는 독립적인 마이크로서 비스로 개발됩니다. 사용자는 비동기 API를 통해 모델에 액세스합니다. 사용자는 요청 또는 요청 배치를 보내고 결과를 보낼 위치를 지정할 수 있습니다. 회사는 수백 명의 사용자에게 모델을 제공합니다. 모델의 사용 패턴이 불규칙합니다. 일부 모델은 며칠 또는 몇 주 동안 사용하지 않을 수 있습니다. 다른 모델은 한 번에 수천 개의 요청 배치를 수신할 수 있습니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 디자인을 권장해야 합니까?
A. API의 요청을 Network Load Balancer(NLB)로 보냅니다. NLB에서 호출하는 AWS Lambda 함수로 모델을 배포합니다. 
B. API의 요청을 Application Load Balancer(ALB)로 보냅니다. Amazon Simple Queue Service(Amazon SQS) 대기열에서 읽는 Amazon Elastic Container Service
(Amazon ECS) 서비스로 모델을 배포합니다. AWS App Mesh를 사용하여 SQS 대기열 크기에 따라 ECS 클러스터의 인스턴스를 확장합니다.
C. API의 요청을 Amazon Simple Queue Service(Amazon SQS) 대기열로 보냅니다. SQS 이벤트에 의해 호출되는 AWS Lambda 함수로 모델을 배포합니다. AWS Auto
Scaling을 사용하여 SQS 대기열 크기에 따라 Lambda 함수의 vCPU 수를 늘립니다.
D. API의 요청을 Amazon Simple Queue Service(Amazon SQS) 대기열로 보냅니다. 대기열에서 읽는 Amazon Elastic Container Service(Amazon ECS) 서비스로 모델을
배포합니다. 대기열 크기에 따라 서비스의 클러스터와 복사본 모두에 대해 Amazon ECS에서 AWS Auto Scaling을 활성화합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q216
소셜 미디어 회사는 사용자가 AWS 클라우드에서 호스팅되는 애플리케이션에 이미지를 업로드할 수 있도록 허용하려고 합니다. 회사는 이미지가 여러 장치 유형에 표시될 수 있도록 이미지 크 기를 자동으로 조정하는 솔루션이 필요합니다. 애플리케이션은 하루 종일 예측할 수 없는 트래픽 패턴을 경험합니다. 회사는 확장성을 극대화하는 고가용성 솔루션을 찾고 있습니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 이미지 크기를 조정하고 이미지를 Amazon S3 버킷에 저장하기 위해 AWS Lambda 함수를 호출하는 Amazon S3에서 호스팅되는 정적 웹 사이트를 생성합니다. 
B. AWS Step Functions를 호출하여 이미지 크기를 조정하고 Amazon RDS 데이터베이스에 이미지를 저장하는 Amazon CloudFront에서 호스팅되는 정적 웹 사이트를 생성합니다
.
C. Amazon EC2 인스턴스에서 실행되는 웹 서버에서 호스팅되는 동적 웹 사이트를 만듭니다. EC2 인스턴스에서 실행되는 프로세스를 구성하여 이미지 크기를 조정하고 Amazon S3 버
킷에 이미지를 저장합니다.
D. Amazon Simple Queue Service(Amazon SQS)에서 크기 조정 작업을 생성하는 자동 확장 Amazon Elastic Container Service(Amazon ECS) 클러스터에서 호스팅되는
동적 웹 사이트를 생성합니다. 크기 조정 작업을 처리하기 위해 Amazon EC2 인스턴스에서 실행되는 이미지 크기 조정 프로그램을 설정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q217
제조 회사에는 Amazon S3 버킷에 .csv 파일을 업로드하는 기계 센서가 있습니다. 이러한 .csv 파일은 이미지로 변환되어야 하며 그래픽 보고서의 자동 생성을 위해 가능한 한 빨리 사용할 수 있어야 합니다. 이미지는 1개월이 지나면 관련이 없게 되지만 1년에 두 번 기계 학습(ML) 모델을 훈련시키기 위해 .csv 파일을 보관해야 합니다. ML 교육 및 감사는 몇 주 전에 미리 계획됩니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 단계 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 매시간 .csv 파일을 다운로드하고 이미지 파일을 생성하며 이미지를 S3 버킷에 업로드하는 Amazon EC2 스팟 인스턴스를 시작합니다. 
B. .csv 파일을 이미지로 변환하고 이미지를 S3 버킷에 저장하는 AWS Lambda 함수를 설계합니다. .csv 파일이 업로드되면 Lambda 함수를 호출합니다. 
C. S3 버킷의 .csv 파일 및 이미지 파일에 대한 S3 수명 주기 규칙을 생성합니다. .csv 파일을 업로드하고 1일 후에 S3 Standard에서 S3 Glacier로 전환합니다. 30일 후에 이미지 파일
을 만료하십시오.
D. S3 버킷의 .csv 파일 및 이미지 파일에 대한 S3 수명 주기 규칙을 생성합니다. 업로드 1일 후 .csv 파일을 S3 Standard에서 S3 One Zone-Infrequent Access(S3 One Zone-
IA)로 전환합니다. 30일 후에 이미지 파일을 만료하십시오.
E. S3 버킷의 .csv 파일 및 이미지 파일에 대한 S3 수명 주기 규칙을 생성합니다. .csv 파일을 업로드하고 1일 후에 S3 Standard에서 S3 Standard-Infrequent Access(S3
Standard-IA)로 전환합니다. RRS(Reduced Redundancy Storage)에 이미지 파일을 보관합니다.

<details>
<summary>정답 보기</summary>

**BC**
</details>

---

### Q218
한 글로벌 기업이 AWS Organizations의 여러 AWS 계정에서 애플리케이션을 실행합니다. 회사의 애플리케이션은 멀티파트 업로드를 사용하여 AWS 리전의 여러 Amazon S3 버킷에 데이터를 업로드합니다. 회사는 비용 준수 목적으로 불완전한 멀티파트 업로드에 대해 보고하려고 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 불완전한 멀티파트 업로드 객체 수를 보고하는 규칙으로 AWS Config를 구성합니다. 
B. 불완전한 멀티파트 업로드 개체 수를 보고하는 SCP(서비스 제어 정책)를 만듭니다. 
C. 불완전한 멀티파트 업로드 객체 수를 보고하도록 S3 스토리지 렌즈를 구성합니다. 
D. S3 다중 지역 액세스 포인트를 생성하여 불완전한 멀티파트 업로드 객체 수를 보고합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q219
한 회사는 AWS 클라우드에서 긴밀하게 결합된 고성능 컴퓨팅(HPC) 환경을 설계하고 있습니다. 이 회사는 네트워킹 및 스토리지를 위해 HPC 환경을 최적화하는 것을 목표로 합니다. 이러 한 요구 사항을 충족하는 솔루션 조합은 무엇입니까? (2개 선택)
A. Amazon CloudFront 배포판을 생성합니다. 뷰어 프로토콜 정책을 HTTP 및 HTTPS로 구성합니다.
B. 환경을 관리하기 위해 AWS Elastic Beanstalk 배포를 생성합니다.
C. AWS Global Accelerator에서 액셀러레이터를 생성합니다. 가속기에 대한 사용자 지정 라우팅을 구성합니다. 
D. Lustre 파일 시스템용 Amazon FSx를 생성합니다. 스크래치 스토리지로 파일 시스템을 구성합니다.
E. Amazon EC2 인스턴스를 시작합니다. EFA(Elastic Fabric Adapter)를 인스턴스에 연결합니다.

<details>
<summary>정답 보기</summary>

**DE**
</details>

---

### Q220
솔루션 설계자는 회사의 Amazon S3 버킷을 검토하여 개인 식별 정보(PII)를 검색해야 합니다. 회사는 us-east-1 지역 및 us-west-2 지역에 PII 데이터를 저장합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 각 리전에서 Amazon Macie를 구성합니다. Amazon S3에 있는 데이터를 분석하는 작업을 생성합니다. 
B. 모든 지역에 대해 AWS Security Hub를 구성합니다. Amazon S3에 있는 데이터를 분석하는 AWS Config 규칙을 생성합니다. 
C. Amazon S3에 있는 데이터를 분석하도록 Amazon Inspector를 구성합니다. 
D. Amazon S3에 있는 데이터를 분석하도록 Amazon GuardDuty를 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q221
다음 IAM 정책은 IAM 그룹에 연결됩니다. 이것은 그룹에 적용되는 유일한 정책입니다. 그룹 구성원에 대한 이 정책의 유효 IAM 권한은 무엇입니까?
A. 그룹 구성원은 us-east-1 지역 내 모든 Amazon EC2 작업이 허용됩니다. 허용 권한 이후의 문은 적용되지 않습니다. 
B. 그룹 구성원은 멀티 팩터 인증(MFA)으로 로그인하지 않는 한 us-east-1 리전에서 모든 Amazon EC2 권한이 거부됩니다. 
C. 그룹 구성원은 멀티 팩터 인증(MFA)으로 로그인할 때 모든 리전에 대한 ec2:StopInstances 및 ec2:TerminateInstances 권한이 허용됩니다. 그룹 구성원은 다른 모든 Amazon
EC2 작업이 허용됩니다.
D. 그룹 구성원은 멀티 팩터 인증(MFA)으로 로그인한 경우에만 us-east-1 리전에 대한 ec2:StopInstances 및 ec2:TerminateInstances 권한이 허용됩니다. 그룹 구성원은 us-
east-1 리전 내에서 다른 모든 Amazon EC2 작업이 허용됩니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q222
한 회사가 Elastic Load Balancer 뒤의 Amazon EC2 인스턴스에서 실행될 새로운 웹 서비스를 설계하고 있습니다. 그러나 많은 웹 서비스 클라이언트는 방화벽에 허용된 IP 주소에만 접 근할 수 있습니다. 솔루션 아키텍트는 고객의 요구 사항을 충족하기 위해 무엇을 권장해야 합니까?
A. 탄력적 IP 주소가 연결된 Network Load Balancer. 
B. 탄력적 IP 주소가 연결된 Application Load Balancer 
C. 탄력적 IP 주소를 가리키는 Amazon Route 53 호스팅 영역의 A 레코드 
D. 로드 밸런서 앞에서 프록시로 실행되는 퍼블릭 IP 주소가 있는 EC2 인스턴스

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q223
회사에는 로컬 데이터 센터 내에 Docker 컨테이너를 활용하는 애플리케이션이 있습니다. 애플리케이션은 컨테이너 인스턴스가 활용하는 해당 호스트의 볼륨에 영구 데이터를 저장하는 컨테 이너 호스트에서 작동합니다. 회사는 서버나 스토리지 인프라 관리를 피하기 위해 이 애플리케이션을 완전 관리형 서비스로 마이그레이션하는 것을 목표로 하고 있습니다. 이러한 요구 사항에 맞는 솔루션은 무엇입니까?
A. 자체 관리형 노드를 사용하는 Amazon Elastic Kubernetes Service(Amazon EKS)를 활용합니다. Amazon EC2 인스턴스에 연결된 Amazon Elastic Block Store
(Amazon EBS) 볼륨을 설정합니다. EBS 볼륨을 컨테이너 내에 탑재된 영구 볼륨으로 활용합니다.
B. AWS Fargate 시작 유형을 사용하여 Amazon Elastic Container Service(Amazon ECS)를 사용합니다. Amazon Elastic File System(Amazon EFS) 볼륨을 설정합니다
. EFS 볼륨을 컨테이너 내에 탑재된 영구 스토리지 볼륨으로 포함합니다.
C. AWS Fargate 시작 유형과 함께 Amazon Elastic Container Service(Amazon ECS)를 활용합니다. Amazon S3 버킷을 생성하고 S3 버킷을 컨테이너 내에 탑재된 영구 스토
리지 볼륨으로 매핑합니다.
D. Amazon EC2 시작 유형과 함께 Amazon Elastic Container Service(Amazon ECS)를 사용하십시오. Amazon Elastic File System(Amazon EFS) 볼륨을 설정합니다.
EFS 볼륨을 컨테이너 내에 탑재된 영구 스토리지 볼륨으로 추가합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q224
솔루션 설계자는 AWS CloudFormation 템플릿을 사용하여 3계층 웹 애플리케이션을 배포합니다. 웹 애플리케이션은 웹 계층과 Amazon DynamoDB 테이블에서 사용자 데이터를 저장 하고 검색하는 애플리케이션 계층으로 구성됩니다. 웹 및 애플리케이션 계층은 Amazon EC2 인스턴스에서 호스팅되며 데이터베이스 계층은 공개적으로 액세스할 수 없습니다. 애플리케이 션 EC2 인스턴스는 템플릿에서 API 자격 증명을 노출하지 않고 DynamoDB 테이블에 액세스해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. DynamoDB 테이블을 읽을 IAM 역할을 생성합니다. 인스턴스 프로필을 참조하여 역할을 애플리케이션 인스턴스와 연결합니다.
B. DynamoDB 테이블에서 읽고 쓰는 데 필요한 권한이 있는 IAM 역할을 생성합니다. EC2 인스턴스 프로필에 역할을 추가하고 인스턴스 프로필을 애플리케이션 인스턴스와 연결합니다.
C. AWS CloudFormation 템플릿의 파라미터 섹션을 사용하여 사용자가 DynamoDB 테이블에서 읽고 쓰는 데 필요한 권한이 있는 이미 생성된 IAM 사용자의 액세스 및 비밀 키를 입력
하도록 합니다.
D. DynamoDB 테이블에서 읽고 쓰는 데 필요한 권한이 있는 AWS CloudFormation 템플릿에서 IAM 사용자를 생성합니다. GetAtt 기능을 사용하여 액세스 및 비밀 키를 검색하고 사
용자 데이터를 통해 애플리케이션 인스턴스에 전달합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q225
소셜 미디어 회사는 웹사이트용 기능을 구축하고 있습니다. 이 기능을 통해 사용자는 사진을 업로드할 수 있습니다. 회사는 대규모 이벤트 기간 동안 수요가 크게 증가할 것으로 예상하고 웹사 이트가 사용자의 업로드 트래픽을 처리할 수 있는지 확인해야 합니다. MOST 확장성으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 사용자의 브라우저에서 응용 프로그램 서버로 파일을 업로드합니다. 파일을 Amazon S3 버킷으로 전송합니다. 
B. AWS Storage Gateway 파일 게이트웨이를 프로비저닝합니다. 사용자의 브라우저에서 파일 게이트웨이로 직접 파일을 업로드합니다. 
C. 애플리케이션에서 Amazon S3 미리 서명된 URL을 생성합니다. 사용자 브라우저에서 S3 버킷으로 직접 파일을 업로드합니다. 
D. Amazon Elastic File System(Amazon EFS) 파일 시스템을 프로비저닝합니다. 사용자의 브라우저에서 파일 시스템으로 직접 파일을 업로드합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q226
회사의 웹 사이트는 매일 수백만 건의 요청을 처리하며 요청 수는 계속 증가하고 있습니다. 솔루션 설계자는 웹 애플리케이션의 응답 시간을 개선해야 합니다. 솔루션 설계자는 애플리케이션이 Amazon DynamoDB 테이블에서 제품 세부 정보를 검색할 때 지연 시간을 줄여야 한다고 결정합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. DynamoDB Accelerator(DAX) 클러스터를 설정합니다. DAX를 통해 모든 읽기 요청을 라우팅합니다.
B. DynamoDB 테이블과 웹 애플리케이션 사이에 Redis용 Amazon ElastiCache를 설정합니다. Redis를 통해 모든 읽기 요청을 라우팅합니다.
C. DynamoDB 테이블과 웹 애플리케이션 사이에 Amazon ElastiCache for Memcached를 설정합니다. Memcached를 통해 모든 읽기 요청을 라우팅합니다.
D. 테이블에 Amazon DynamoDB 스트림을 설정하고 AWS Lambda가 테이블에서 읽고 Amazon ElastiCache를 채우도록 합니다. ElastiCache를 통해 모든 읽기 요청을 라우팅
합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q227
솔루션 아키텍트는 AWS에 배포되는 새로운 애플리케이션을 위한 클라우드 아키텍처를 설계하고 있습니다. 프로세스는 처리할 작업 수에 따라 필요에 따라 애플리케이션 노드를 추가 및 제거 하는 동안 병렬로 실행되어야 합니다. 프로세서 애플리케이션은 상태 비저장입니다. 솔루션 설계자는 애플리케이션이 느슨하게 결합되고 작업 항목이 지속적으로 저장되는지 확인해야 합니다. 솔루션 설계자는 어떤 디자인을 사용해야 합니까?
A. 처리해야 할 작업을 보낼 Amazon SNS 주제를 생성합니다. 프로세서 애플리케이션으로 구성된 Amazon 머신 이미지(AMI)를 생성합니다. AMI를 사용하는 시작 구성을 생성합니다.
시작 구성을 사용하여 Auto Scaling 그룹을 생성합니다. CPU 사용량에 따라 노드를 추가 및 제거하도록 Auto Scaling 그룹에 대한 조정 정책을 설정합니다.
B. 처리해야 하는 작업을 보관할 Amazon SQS 대기열을 생성합니다. 프로세서 애플리케이션으로 구성된 Amazon 머신 이미지(AMI)를 생성합니다. AMI를 사용하는 시작 구성을 생성합
니다. 시작 구성을 사용하여 Auto Scaling 그룹을 생성합니다. 네트워크 사용량에 따라 노드를 추가 및 제거하도록 Auto Scaling 그룹에 대한 조정 정책을 설정합니다.
C. 처리해야 할 작업을 보관할 Amazon SQS 대기열을 생성합니다. 프로세서 애플리케이션으로 구성된 Amazon 머신 이미지(AMI)를 생성합니다. AMI를 사용하는 시작 템플릿을 생성합
니다. 시작 템플릿을 사용하여 Auto Scaling 그룹을 생성합니다. SQS 대기열의 항목 수에 따라 노드를 추가 및 제거하도록 Auto Scaling 그룹에 대한 조정 정책을 설정합니다.
D. 처리해야 할 작업을 보낼 Amazon SNS 주제를 생성합니다. 프로세서 애플리케이션으로 구성된 Amazon 머신 이미지(AMI)를 생성합니다. AMI를 사용하는 시작 템플릿을 생성합니다
. 시작 템플릿을 사용하여 Auto Scaling 그룹을 생성합니다. SNS 주제에 게시된 메시지 수에 따라 노드를 추가 및 제거하도록 Auto Scaling 그룹에 대한 조정 정책을 설정합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q228
회사에서 PostgreSQL용 Amazon RDS를 사용하는 애플리케이션을 실행합니다. 애플리케이션은 평일 업무 시간에만 트래픽을 수신합니다. 회사는 이 사용량을 기반으로 비용을 최적화하 고 운영 오버헤드를 줄이려고 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS의 인스턴스 스케줄러를 사용하여 시작 및 중지 일정을 구성하십시오. 
B. 자동 백업을 끕니다. 데이터베이스의 매주 수동 스냅샷을 생성합니다. 
C. 최소 CPU 사용률을 기준으로 데이터베이스를 시작하고 중지하는 사용자 지정 AWS Lambda 함수를 생성합니다. 
D. 모든 Upfront 예약 DB 인스턴스를 구매합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q229
회사는 Amazon EC2 인스턴스에서 애플리케이션을 실행합니다. 회사는 애플리케이션에 재해 복구(DR) 솔루션을 구현해야 합니다. DR 솔루션은 RTO(복구 시간 목표)가 4시간 미만이어 야 합니다. 또한 DR 솔루션은 정상 작동 중에 가능한 한 적은 AWS 리소스를 사용해야 합니다. 운영상 가장 효율적인 방식으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon 머신 이미지(AMI)를 생성하여 EC2 인스턴스를 백업합니다. AMI를 보조 AWS 리전에 복사합니다. AWS Lambda 및 사용자 지정 스크립트를 사용하여 보조 리전에서 인프
라 배포를 자동화합니다.
B. Amazon 머신 이미지(AMI)를 생성하여 EC2 인스턴스를 백업합니다. AMI를 보조 AWS 리전에 복사합니다. AWS CloudFormation을 사용하여 보조 리전에서 인프라 배포를 자동
화합니다.
C. 보조 AWS 리전에서 EC2 인스턴스를 시작합니다. 보조 리전의 EC2 인스턴스를 항상 활성 상태로 유지하십시오. 
D. 보조 가용 영역에서 EC2 인스턴스를 시작합니다. 보조 가용 영역의 EC2 인스턴스를 항상 활성 상태로 유지합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q230
회사는 2개의 가용 영역에 걸쳐 VPC에서 여러 Amazon EC2 Linux 인스턴스를 실행합니다. 인스턴스는 계층적 디렉터리 구조를 사용하는 애플리케이션을 호스팅합니다. 애플리케이션은 공유 스토리지에서 동시에 빠르게 읽고 쓸 수 있어야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Amazon S3 버킷을 생성합니다. VPC의 모든 EC2 인스턴스에서 액세스를 허용합니다. 
B. Amazon Elastic File System(Amazon EFS) 파일 시스템을 생성합니다. 각 EC2 인스턴스에서 EFS 파일 시스템을 탑재합니다. 
C. 프로비저닝된 IOPS SSD(io2) Amazon Elastic Block Store(Amazon EBS) 볼륨에 파일 시스템을 생성합니다. EBS 볼륨을 모든 EC2 인스턴스에 연결합니다. 
D. 각 EC2 인스턴스에 연결된 Amazon Elastic Block Store(Amazon EBS) 볼륨에 파일 시스템을 만듭니다. 여러 EC2 인스턴스 간에 EBS 볼륨을 동기화합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q231
회사에서 고성능 컴퓨팅 및 인공 지능을 사용하여 사기 방지 및 감지 기술을 개선하려고 합니다. 회사는 가능한 한 빨리 단일 워크로드를 완료하기 위해 분산 처리가 필요합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Elastic Kubernetes Service(Amazon EKS) 및 여러 컨테이너를 사용합니다.
B. AWS ParallelCluster 및 MPI(Message Passing Interface) 라이브러리를 사용합니다.
C. Application Load Balancer 및 Amazon EC2 인스턴스를 사용합니다.
D. AWS Lambda 함수를 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q232
한 회사는 최근 프라이빗 서브넷의 Amazon EC2에서 Linux 기반 애플리케이션 인스턴스를 시작했고 VPC의 퍼블릭 서브넷의 Amazon EC2 인스턴스에서 Linux 기반 배스천 호스트를 시작했습니다. 솔루션 설계자는 회사의 인터넷 연결을 통해 온프레미스 네트워크에서 배스천 호스트 및 애플리케이션 서버에 연결해야 합니다. 솔루션 설계자는 모든 EC2 인스턴스의 보안 그 룹이 해당 액세스를 허용하는지 확인해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. 배스천 호스트의 현재 보안 그룹을 애플리케이션 인스턴스로부터의 인바운드 액세스만 허용하는 보안 그룹으로 교체하십시오. 
B. 배스천 호스트의 현재 보안 그룹을 회사 내부 IP 범위의 인바운드 액세스만 허용하는 보안 그룹으로 교체합니다. 
C. 배스천 호스트의 현재 보안 그룹을 회사의 외부 IP 범위로부터의 인바운드 액세스만 허용하는 보안 그룹으로 교체합니다. 
D. 애플리케이션 인스턴스의 현재 보안 그룹을 배스천 호스트의 사설 IP 주소에서만 인바운드 SSH 액세스를 허용하는 보안 그룹으로 바꿉니다. 
E. 애플리케이션 인스턴스의 현재 보안 그룹을 배스천 호스트의 퍼블릭 IP 주소에서만 인바운드 SSH 액세스를 허용하는 보안 그룹으로 바꿉니다.

<details>
<summary>정답 보기</summary>

**CD**
</details>

---

### Q233
회사는 여러 Amazon EC2 인스턴스에서 애플리케이션을 호스팅합니다. 애플리케이션은 Amazon SQS 대기열의 메시지를 처리하고 Amazon RDS 테이블에 쓰고 대기열에서 메시지를 삭제합니다. 때때로 중복 레코드가 RDS 테이블에서 발견됩니다. SQS 대기열에는 중복 메시지가 없습니다. 솔루션 설계자는 메시지가 한 번만 처리되도록 하려면 어떻게 해야 합니까?
A. CreateQueue API 호출을 사용하여 새 대기열을 만듭니다. 
B. AddPermission API 호출을 사용하여 적절한 권한을 추가합니다. 
C. ReceiveMessage API 호출을 사용하여 적절한 대기 시간을 설정합니다. 
D. ChangeMessageVisibility API 호출을 사용하여 가시성 제한 시간을 늘립니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q234
회사는 온프레미스 데이터 센터에서 여러 워크로드를 실행합니다. 회사의 데이터 센터는 회사의 확장되는 비즈니스 요구 사항을 충족할 만큼 빠르게 확장할 수 없습니다. 회사는 AWS로의 마 이그레이션을 계획하기 위해 온프레미스 서버 및 워크로드에 대한 사용량 및 구성 데이터를 수집하려고 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS Migration Hub에서 홈 AWS 리전을 설정합니다. AWS Systems Manager를 사용하여 온프레미스 서버에 대한 데이터를 수집합니다. 
B. AWS Migration Hub에서 홈 AWS 지역을 설정합니다. AWS Application Discovery Service를 사용하여 온프레미스 서버에 대한 데이터를 수집합니다. 
C. AWS Schema Conversion Tool(AWS SCT)을 사용하여 관련 템플릿을 생성합니다. AWS Trusted Advisor를 사용하여 온프레미스 서버에 대한 데이터를 수집합니다. 
D. AWS SCT(AWS Schema Conversion Tool)를 사용하여 관련 템플릿을 생성합니다. AWS Database Migration Service(AWS DMS)를 사용하여 온프레미스 서버에 대한
데이터를 수집합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q235
회사는 데이터를 온프레미스에 저장합니다. 데이터의 양은 회사가 사용할 수 있는 용량을 초과하여 증가하고 있습니다. 회사는 온프레미스 위치에서 Amazon S3 버킷으로 데이터를 마이그레이션하려고 합니다. 회사에는 전송 후 데이터의 무결성을 자동으로 검증하는 솔루션이 필요합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS Snowball Edge 디바이스를 주문하십시오. S3 버킷으로 온라인 데이터 전송을 수행하도록 Snowball Edge 디바이스를 구성합니다.
B. AWS DataSync 에이전트를 온프레미스에 배포합니다. S3 버킷으로의 온라인 데이터 전송을 수행하도록 DataSync 에이전트를 구성합니다.
C. 온프레미스에서 Amazon S3 파일 게이트웨이를 생성합니다. S3 파일 게이트웨이를 구성하여 S3 버킷으로 온라인 데이터 전송을 수행합니다. 
D. 온프레미스에서 Amazon S3 Transfer Acceleration에 액셀러레이터를 구성합니다. S3 버킷으로의 온라인 데이터 전송을 수행하도록 액셀러레이터를 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q236
한 회사에서 애플리케이션 테스트 중에 Amazon RDS for MySQL DB 인스턴스를 사용했습니다. 테스트 주기가 끝날 때 DB 인스턴스를 종료하기 전에 솔루션 설계자는 두 개의 백업을 생 성했습니다. 솔루션 설계자는 데이터베이스 덤프를 생성하기 위해 mysqldump 유틸리티를 사용하여 첫 번째 백업을 생성했습니다. 솔루션 설계자는 RDS 종료 시 최종 DB 스냅샷 옵션을 활성화하여 두 번째 백업을 생성했습니다. 회사는 이제 새로운 테스트 주기를 계획하고 있으며 가장 최근 백업에서 새 DB 인스턴스를 생성하려고 합니다. 이 회사는 DB 인스턴스를 호스팅하기 위해 Amazon Aurora의 MySQL 호 환 에디션을 선택했습니다. 어떤 솔루션이 새 DB 인스턴스를 생성합니까? (두 가지를 선택하세요.)
A. RDS 스냅샷을 Aurora로 직접 가져옵니다.
B. RDS 스냅샷을 Amazon S3에 업로드합니다. 그런 다음 RDS 스냅샷을 Aurora로 가져옵니다.
C. 데이터베이스 덤프를 Amazon S3에 업로드합니다. 그런 다음 데이터베이스 덤프를 Aurora로 가져옵니다.
D. AWS Database Migration Service(AWS DMS)를 사용하여 RDS 스냅샷을 Aurora로 가져옵니다.
E. 데이터베이스 덤프를 Amazon S3에 업로드합니다. 그런 다음 AWS Database Migration Service(AWS DMS)를 사용하여 데이터베이스 덤프를 Aurora로 가져옵니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q237
분석 회사는 Amazon VPC를 활용하여 다중 계층 서비스를 운영합니다. 회사는 RESTful API를 통해 수백만 명의 사용자에게 웹 분석 서비스를 제공할 계획입니다. API에 액세스하려면 인 증 서비스를 통한 사용자 확인이 필요합니다. 이러한 요구 사항에 대해 최고의 운영 효율성을 보장하는 솔루션은 무엇입니까?
A. 사용자 인증을 위해 Amazon Cognito 사용자 풀을 구성합니다. Cognito 권한 부여자를 사용하여 Amazon API Gateway REST API를 구현합니다. 
B. 사용자 인증을 위해 Amazon Cognito 자격 증명 풀을 구성합니다. Cognito 권한 부여자를 사용하여 Amazon API Gateway HTTP API를 구현합니다. 
C. 사용자 인증을 위해 AWS Lambda 함수를 구성합니다. Lambda 권한 부여자를 사용하여 Amazon API Gateway REST API를 구현합니다. 
D. 사용자 인증을 위해 IAM 사용자를 구성합니다. IAM 권한 부여자를 사용하여 Amazon API Gateway HTTP API를 구현합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q238
회사는 Amazon EC2 인스턴스를 사용하여 내부 시스템을 호스팅합니다. 배포 작업의 일부로 관리자는 AWS CLI를 사용하여 EC2 인스턴스를 종료하려고 합니다. 그러나 관리자는 403 (액세스 거부) 오류 메시지를 받습니다. 관리자는 다음 IAM 정책이 연결된 IAM 역할을 사용하고 있습니다. 실패한 요청의 원인은 무엇입니까?
A. EC2 인스턴스에는 Deny 문이 포함된 리소스 기반 정책이 있습니다. 
B. 정책 설명에 주체가 지정되지 않았습니다. 
C. "Action" 필드는 EC2 인스턴스를 종료하는 데 필요한 조치를 부여하지 않습니다. 
D. EC2 인스턴스 종료 요청은 CIDR 블록 192.0.2.0/24 또는 203.0.113.0/24에서 시작되지 않습니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q239
회사에 이미지 공유를 위한 3계층 애플리케이션이 있습니다. 이 애플리케이션은 프런트 엔드 계층에 Amazon EC2 인스턴스를 사용하고, 애플리케이션 계층에 또 다른 EC2 인스턴스를 사 용하고, MySQL 데이터베이스에 세 번째 EC2 인스턴스를 사용합니다. 솔루션 설계자는 응용 프로그램에 최소한의 변경만 필요한 확장 가능하고 가용성이 높은 솔루션을 설계해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon S3를 사용하여 프런트 엔드 계층을 호스팅하십시오. 애플리케이션 계층에 AWS Lambda 함수를 사용합니다. 데이터베이스를 Amazon DynamoDB 테이블로 이동합니다.
Amazon S3를 사용하여 사용자 이미지를 저장하고 제공합니다.
B. 프런트엔드 계층과 애플리케이션 계층에 로드 밸런싱된 다중 AZ AWS Elastic Beanstalk 환경을 사용합니다. 데이터베이스를 여러 읽기 전용 복제본이 있는 Amazon RDS DB 인
스턴스로 이동하여 사용자 이미지를 제공합니다.
C. Amazon S3를 사용하여 프런트 엔드 계층을 호스팅합니다. 애플리케이션 계층에 대한 Auto Scaling 그룹의 EC2 인스턴스 플릿을 사용합니다. 데이터베이스를 메모리 최적화 인스턴
스 유형으로 이동하여 사용자 이미지를 저장하고 제공합니다.
D. 프런트엔드 계층과 애플리케이션 계층에 로드 밸런싱된 다중 AZ AWS Elastic Beanstalk 환경을 사용합니다. 데이터베이스를 Amazon RDS 다중 AZ DB 인스턴스로 이동합니다.
Amazon S3를 사용하여 사용자 이미지를 저장하고 제공합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q240
회사에서 온프레미스 워크로드를 AWS 클라우드로 마이그레이션하고 있습니다. 이 회사는 이미 여러 Amazon EC2 인스턴스와 Amazon RDS DB 인스턴스를 사용하고 있습니다. 회사 는 업무 시간 외에 EC2 인스턴스와 DB 인스턴스를 자동으로 시작하고 중지하는 솔루션을 원합니다. 솔루션은 비용 및 인프라 유지 관리를 최소화해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 탄력적 크기 조정을 사용하여 EC2 인스턴스를 확장합니다. 업무 시간 외에는 DB 인스턴스를 0으로 조정합니다. 
B. 일정에 따라 EC2 인스턴스와 DB 인스턴스를 자동으로 시작 및 중지하는 파트너 솔루션에 대한 AWS Marketplace를 살펴보십시오. 
C. 다른 EC2 인스턴스를 시작합니다. 일정에 따라 기존 EC2 인스턴스와 DB 인스턴스를 시작 및 중지하는 셸 스크립트를 실행하도록 crontab 일정을 구성합니다. 
D. EC2 인스턴스와 DB 인스턴스를 시작하고 중지할 AWS Lambda 함수를 생성합니다. 일정에 따라 Lambda 함수를 호출하도록 Amazon EventBridge를 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q241
보안 팀은 팀의 모든 AWS 계정에서 특정 서비스 또는 작업에 대한 액세스를 제한하려고 합니다. 모든 계정은 AWS Organizations의 대규모 조직에 속합니다. 솔루션은 확장 가능해야 하 며 권한을 유지할 수 있는 단일 지점이 있어야 합니다. 이를 달성하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. ACL을 생성하여 서비스 또는 작업에 대한 액세스를 제공합니다. 
B. 계정을 허용할 보안 그룹을 생성하고 사용자 그룹에 연결합니다. 
C. 각 계정에서 교차 계정 역할을 생성하여 서비스 또는 작업에 대한 액세스를 거부합니다. 
D. 루트 조직 단위에 서비스 제어 정책을 만들어 서비스 또는 작업에 대한 액세스를 거부합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q242
회사에는 Amazon S3 버킷에 수백만 개의 객체가 있는 서버리스 웹 사이트가 있습니다. 회사는 S3 버킷을 Amazon CloudFront 배포의 오리진으로 사용합니다. 회사는 개체가 로드되기 전에 S3 버킷에 암호화를 설정하지 않았습니다. 솔루션 설계자는 모든 기존 객체와 향후 S3 버킷에 추가되는 모든 객체에 대해 암호화를 활성화해야 합니다. 최소한의 노력으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 새 S3 버킷을 생성합니다. 새 S3 버킷에 대한 기본 암호화 설정을 켭니다. 모든 기존 개체를 임시 로컬 저장소에 다운로드합니다. 새 S3 버킷에 객체를 업로드합니다. 
B. S3 버킷의 기본 암호화 설정을 켭니다. S3 Inventory 기능을 사용하여 암호화되지 않은 객체를 나열하는 .csv 파일을 생성합니다. 복사 명령을 사용하여 해당 객체를 암호화하는 S3 배
치 작업 작업을 실행합니다.
C. AWS Key Management Service(AWS KMS)를 사용하여 새 암호화 키를 생성합니다. AWS KMS 관리형 암호화 키(SSE-KMS)로 서버 측 암호화를 사용하도록 S3 버킷의 설
정을 변경합니다. S3 버킷에 대한 버전 관리를 켭니다.
D. AWS Management Console에서 Amazon S3로 이동합니다. S3 버킷의 객체를 찾습니다. 암호화 필드를 기준으로 정렬합니다. 암호화되지 않은 각 개체를 선택합니다. 수정 버튼
을 사용하여 S3 버킷의 모든 암호화되지 않은 객체에 기본 암호화 설정을 적용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q243
개발 팀은 다른 팀에서 액세스할 웹 사이트를 호스팅해야 합니다. 웹 사이트 콘텐츠는 HTML, CSS, 클라이언트 측 JavaScript 및 이미지로 구성됩니다. 웹 사이트 호스팅에 가장 비용 효율적인 방법은 무엇입니까?
A. 웹 사이트를 컨테이너화하고 AWS Fargate에서 호스팅합니다. 
B. Amazon S3 버킷을 생성하고 그곳에서 웹사이트를 호스팅합니다. 
C. Amazon EC2 인스턴스에 웹 서버를 배포하여 웹사이트를 호스팅합니다. 
D. Express.js 프레임워크를 사용하는 AWS Lambda 대상으로 Application Load Balancer를 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q244
회사에서 Amazon Elastic Container Service(Amazon ECS) 클러스터에 배포된 새 애플리케이션을 시작하고 ECS 작업에 Fargate 시작 유형을 사용하고 있습니다. 회사는 실행 시 애플리케이션에 대한 높은 트래픽이 예상되기 때문에 CPU 및 메모리 사용량을 모니터링하고 있습니다. 그러나 회사는 활용도가 감소할 때 비용을 절감하기를 원합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. Amazon EC2 Auto Scaling을 사용하여 이전 트래픽 패턴을 기반으로 특정 기간에 조정합니다. 
B. AWS Lambda 함수를 사용하여 Amazon CloudWatch 경보를 트리거하는 메트릭 위반을 기반으로 Amazon ECS를 확장합니다. 
C. 간단한 조정 정책과 함께 Amazon EC2 Auto Scaling을 사용하여 ECS 메트릭 위반이 Amazon CloudWatch 경보를 트리거할 때 조정합니다. 
D. 대상 추적 정책과 함께 AWS Application Auto Scaling을 사용하여 ECS 메트릭 위반이 Amazon CloudWatch 경보를 트리거할 때 조정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q245
솔루션 설계자는 회사의 재해 복구(DR) 아키텍처를 설계하고 있습니다. 이 회사에는 예약된 백업이 있는 프라이빗 서브넷의 Amazon EC2 인스턴스에서 실행되는 MySQL 데이터베이스가 있습니다. DR 설계에는 여러 AWS 리전이 포함되어야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. MySQL 데이터베이스를 여러 EC2 인스턴스로 마이그레이션합니다. DR 지역에서 대기 EC2 인스턴스를 구성합니다. 복제를 켭니다. 
B. MySQL 데이터베이스를 Amazon RDS로 마이그레이션합니다. 다중 AZ 배포를 사용합니다. 다른 가용 영역에서 기본 DB 인스턴스에 대한 읽기 복제를 켭니다. 
C. MySQL 데이터베이스를 Amazon Aurora 글로벌 데이터베이스로 마이그레이션합니다. 기본 리전에서 기본 DB 클러스터를 호스팅합니다. DR 리전에서 보조 DB 클러스터를 호스팅
합니다.
D. S3 CRR(Cross-Region Replication)용으로 구성된 Amazon S3 버킷에 MySQL 데이터베이스의 예약된 백업을 저장합니다. 데이터 백업을 사용하여 DR 지역에서 데이터베이스
를 복원하십시오.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q246
회사는 Amazon S3를 사용하여 정적 웹 사이트를 호스팅합니다. 회사는 웹 페이지에 연락처 양식을 추가하려고 합니다. 연락처 양식에는 사용자가 이름, 이메일 주소, 전화번호 및 사용자 메 시지를 입력할 수 있는 동적 서버 측 구성 요소가 있습니다. 회사는 매월 100회 미만의 사이트 방문이 있을 것으로 예상합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. Amazon Elastic Container Service(Amazon ECS)에서 동적 문의 양식 페이지를 호스팅합니다. 타사 이메일 공급자에 연결하도록 Amazon Simple Email Service
(Amazon SES)를 설정합니다.
B. Amazon Simple Email Service(Amazon SES)를 호출하는 AWS Lambda 백엔드로 Amazon API Gateway 엔드포인트를 생성합니다. 
C. Amazon Lightsail을 배포하여 정적 웹 페이지를 동적으로 변환합니다. 클라이언트 측 스크립팅을 사용하여 연락처 양식을 작성하십시오. 양식을 Amazon WorkMail과 통합합니다. 
D. t2.micro Amazon EC2 인스턴스를 생성합니다. LAMP(Linux, Apache, MySQL, PHP/Perl/Python) 스택을 배포하여 웹 페이지를 호스팅합니다. 클라이언트 측 스크립팅을 사
용하여 연락처 양식을 작성하십시오. 양식을 Amazon WorkMail과 통합합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q247
회사는 AWS 클라우드를 사용하여 기존 애플리케이션의 가용성과 탄력성을 높이려고 합니다. 애플리케이션의 현재 버전은 회사의 데이터 센터에 상주합니다. 예기치 않은 정전으로 인해 데이 터베이스 서버가 충돌한 후 애플리케이션에서 최근 데이터 손실이 발생했습니다. 회사는 단일 실패 지점을 방지하는 솔루션이 필요합니다. 솔루션은 애플리케이션에 사용자 요구에 맞게 확장할 수 있는 기능을 제공해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 여러 가용 영역의 Auto Scaling 그룹에서 Amazon EC2 인스턴스를 사용하여 애플리케이션 서버를 배포합니다. 다중 AZ 구성에서 Amazon RDS DB 인스턴스를 사용합니다. 
B. 단일 가용 영역의 Auto Scaling 그룹에서 Amazon EC2 인스턴스를 사용하여 애플리케이션 서버를 배포합니다. EC2 인스턴스에 데이터베이스를 배포합니다. EC2 자동 복구를 활성
화합니다.
C. 여러 가용 영역의 Auto Scaling 그룹에서 Amazon EC2 인스턴스를 사용하여 애플리케이션 서버를 배포합니다. 단일 가용 영역에서 읽기 전용 복제본이 있는 Amazon RDS DB 인
스턴스를 사용합니다. 기본 DB 인스턴스가 실패할 경우 읽기 전용 복제본을 승격하여 기본 DB 인스턴스를 교체하십시오.
D. 여러 가용 영역의 Auto Scaling 그룹에서 Amazon EC2 인스턴스를 사용하여 애플리케이션 서버를 배포합니다. 여러 가용 영역에 걸쳐 EC2 인스턴스에 기본 및 보조 데이터베이스
서버를 배포합니다. Amazon Elastic Block Store(Amazon EBS) 다중 연결을 사용하여 인스턴스 간에 공유 스토리지를 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q248
한 회사에서 AWS를 사용하여 보험 견적을 처리할 웹 애플리케이션을 설계하고 있습니다. 사용자는 애플리케이션에서 견적을 요청합니다. 견적은 견적 유형별로 구분되어야 하며, 24시간 이 내에 응답해야 하며 분실해서는 안 됩니다. 솔루션은 운영 효율성을 극대화하고 유지 보수를 최소화해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 견적 유형에 따라 여러 Amazon Kinesis 데이터 스트림을 생성합니다. 적절한 데이터 스트림으로 메시지를 보내도록 웹 애플리케이션을 구성합니다. Kinesis Client Library(KCL)를
사용하여 자체 데이터 스트림에서 메시지를 풀링하도록 애플리케이션 서버의 각 백엔드 그룹을 구성합니다.
B. 각 견적 유형에 대해 AWS Lambda 함수 및 Amazon Simple Notification Service(Amazon SNS) 주제를 생성합니다. 연결된 SNS 주제에 Lambda 함수를 구독합니다. 견적
요청을 적절한 SNS 주제에 게시하도록 애플리케이션을 구성합니다.
C. 단일 Amazon Simple Notification Service(Amazon SNS) 주제를 생성합니다. SNS 주제에 대한 Amazon Simple Queue Service(Amazon SQS) 대기열을 구독합니다.
견적 유형에 따라 적절한 SQS 대기열에 메시지를 게시하도록 SNS 메시지 필터링을 구성합니다. 자체 SQS 대기열을 사용하도록 각 백엔드 애플리케이션 서버를 구성합니다.
D. 데이터 스트림을 Amazon OpenSearch Service 클러스터로 전달하기 위해 견적 유형을 기반으로 여러 Amazon Kinesis Data Firehose 전달 스트림을 생성합니다. 적절한 전송
스트림으로 메시지를 보내도록 애플리케이션을 구성합니다. OpenSearch Service에서 메시지를 검색하고 그에 따라 처리하도록 애플리케이션 서버의 각 백엔드 그룹을 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q249
회사에서 AWS에 새로운 퍼블릭 웹 애플리케이션을 배포하려고 합니다. 애플리케이션에는 Amazon EC2 인스턴스를 사용하는 웹 서버 계층이 포함되어 있습니다. 이 애플리케이션에는 Amazon RDS for MySQL DB 인스턴스를 사용하는 데이터베이스 계층도 포함되어 있습니다. 응용 프로그램은 동적 IP 주소가 있는 글로벌 고객이 안전하고 액세스할 수 있어야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 보안 그룹을 어떻게 구성해야 합니까?
A. 0.0.0.0/0에서 포트 443의 인바운드 트래픽을 허용하도록 웹 서버에 대한 보안 그룹을 구성합니다. 웹 서버의 보안 그룹에서 포트 3306의 인바운드 트래픽을 허용하도록 DB 인스턴스
에 대한 보안 그룹을 구성합니다.
B. 고객의 IP 주소에서 포트 443의 인바운드 트래픽을 허용하도록 웹 서버에 대한 보안 그룹을 구성합니다. 웹 서버의 보안 그룹에서 포트 3306의 인바운드 트래픽을 허용하도록 DB 인스
턴스에 대한 보안 그룹을 구성합니다.
C. 고객의 IP 주소에서 포트 443의 인바운드 트래픽을 허용하도록 웹 서버에 대한 보안 그룹을 구성합니다. 고객의 IP 주소에서 포트 3306의 인바운드 트래픽을 허용하도록 DB 인스턴스에
대한 보안 그룹을 구성합니다.
D. 0.0.0.0/0에서 포트 443의 인바운드 트래픽을 허용하도록 웹 서버에 대한 보안 그룹을 구성합니다. 0.0.0.0/0에서 포트 3306의 인바운드 트래픽을 허용하도록 DB 인스턴스에 대한 보
안 그룹을 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q250
회사에서 필요한 인프라를 수동으로 프로비저닝하여 새 웹 사이트의 인프라 프로토타입을 만들고 있습니다. 이 인프라에는 Auto Scaling 그룹, Application Load Balancer 및 Amazon RDS 데이터베이스가 포함됩니다. 구성이 철저히 검증된 후 회사는 자동화된 방식으로 두 가용 영역에서 개발 및 프로덕션 사용을 위한 인프라를 즉시 배포할 수 있는 기능을 원합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. AWS Systems Manager를 사용하여 두 가용 영역에서 프로토타입 인프라를 복제하고 프로비저닝합니다. 
B. 프로토타입 인프라를 가이드로 사용하여 인프라를 템플릿으로 정의합니다. AWS CloudFormation으로 인프라를 배포하십시오. 
C. AWS Config를 사용하여 프로토타입 인프라에서 사용되는 리소스 인벤토리를 기록합니다. AWS Config를 사용하여 프로토타입 인프라를 두 개의 가용 영역에 배포합니다. 
D. AWS Elastic Beanstalk를 사용하고 프로토타입 인프라에 대한 자동 참조를 사용하도록 구성하여 2개의 가용 영역에 새 환경을 자동으로 배포합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q251
회사에서 1PB 온프레미스 이미지 리포지토리를 AWS로 마이그레이션하려고 합니다. 이미지는 서버리스 웹 애플리케이션에서 사용됩니다. 리포지토리에 저장된 이미지는 거의 액세스되지 않 지만 즉시 사용할 수 있어야 합니다. 또한 미사용 이미지를 암호화하고 우발적인 삭제로부터 보호해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 클라이언트 측 암호화를 구현하고 이미지를 Amazon S3 Glacier 볼트에 저장합니다. 우발적인 삭제를 방지하기 위해 볼트 잠금을 설정합니다. 
B. S3 Standard-Infrequent Access(S3 Standard-IA) 스토리지 클래스의 Amazon S3 버킷에 이미지를 저장합니다. S3 버킷에서 버전 관리, 기본 암호화 및 MFA 삭제를 활성화합
니다.
C. Amazon FSx for Windows File Server 파일 공유에 이미지를 저장합니다. AWS Key Management Service(AWS KMS) 고객 마스터 키(CMK)를 사용하여 파일 공유의 이
미지를 암호화하도록 Amazon FSx 파일 공유를 구성합니다. 우발적인 삭제를 방지하려면 이미지에 NTFS 권한 집합을 사용하십시오.
D. Infrequent Access 스토리지 클래스의 Amazon Elastic File System(Amazon EFS) 파일 공유에 이미지를 저장합니다. AWS Key Management Service(AWS KMS) 고
객 마스터 키(CMK)를 사용하여 파일 공유의 이미지를 암호화하도록 EFS 파일 공유를 구성합니다. 우발적인 삭제를 방지하려면 이미지에 NFS 권한 집합을 사용하십시오.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q252
회사는 Amazon Linux EC2 인스턴스 그룹에서 애플리케이션을 실행합니다. 규정 준수를 위해 회사는 모든 애플리케이션 로그 파일을 7년 동안 보관해야 합니다. 로그 파일은 모든 파일에 동시에 액세스할 수 있어야 하는 보고 도구로 분석됩니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 스토리지 솔루션은 무엇입니까?
A. Amazon Elastic Block Store(Amazon EBS) 
B. Amazon Elastic File System(Amazon EFS) 
C. Amazon EC2 인스턴스 스토어 
D. 아마존 S3

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q253
회사의 애플리케이션은 ALB(Application Load Balancer) 뒤의 Amazon EC2 인스턴스에서 실행됩니다. 인스턴스는 여러 가용 영역에 걸쳐 Amazon EC2 Auto Scaling 그룹에서 실행됩니다. 매월 1일 자정에 월말 재무 계산 일괄 처리가 실행되면 응용 프로그램이 훨씬 느려집니다. 이로 인해 EC2 인스턴스의 CPU 사용률이 즉시 100%에 도달하여 애플리케이션이 중 단됩니다. 애플리케이션이 워크로드를 처리하고 다운타임을 방지할 수 있도록 하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. ALB 앞에 Amazon CloudFront 배포를 구성합니다. 
B. CPU 사용률을 기반으로 EC2 Auto Scaling 단순 조정 정책을 구성합니다. 
C. 월별 일정을 기반으로 EC2 Auto Scaling 예약 조정 정책을 구성합니다. 
D. EC2 인스턴스에서 일부 워크로드를 제거하도록 Amazon ElastiCache를 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q254
회사에서 다중 계층 웹 애플리케이션에 Amazon ElastiCache를 사용할 계획입니다. 솔루션 설계자는 ElastiCache 클러스터용 캐시 VPC와 애플리케이션의 Amazon EC2 인스턴스용 앱 VPC를 생성합니다. 두 VPC 모두 us-east-1 리전에 있습니다. 솔루션 설계자는 애플리케이션의 EC2 인스턴스에 ElastiCache 클러스터에 대한 액세스 권한을 제공하는 솔루션을 구현해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. VPC 간에 피어링 연결을 생성합니다. 두 VPC 모두에서 피어링 연결을 위한 라우팅 테이블 항목을 추가합니다. 애플리케이션의 보안 그룹에서 인바운드 연결을 허용하도록
ElastiCache 클러스터의 보안 그룹에 대한 인바운드 규칙을 구성합니다.
B. 전송 VPC를 생성합니다. 전송 VPC를 통해 트래픽을 라우팅하도록 캐시 VPC 및 앱 VPC의 VPC 라우팅 테이블을 업데이트합니다. 애플리케이션의 보안 그룹에서 인바운드 연결을 허
용하도록 ElastiCache 클러스터의 보안 그룹에 대한 인바운드 규칙을 구성합니다.
C. VPC 간에 피어링 연결을 생성합니다. 두 VPC 모두에서 피어링 연결을 위한 라우팅 테이블 항목을 추가합니다. 애플리케이션의 보안 그룹에서 인바운드 연결을 허용하도록 피어링 연결
의 보안 그룹에 대한 인바운드 규칙을 구성합니다.
D. 전송 VPC를 생성합니다. 전송 VPC를 통해 트래픽을 라우팅하도록 캐시 VPC 및 앱 VPC의 VPC 라우팅 테이블을 업데이트합니다. 애플리케이션의 보안 그룹에서 인바운드 연결을 허
용하도록 Transit VPC의 보안 그룹에 대한 인바운드 규칙을 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q255
회사는 AWS에서 데이터 레이크를 호스팅합니다. 데이터 레이크는 PostgreSQL용 Amazon S3 및 Amazon RDS의 데이터로 구성됩니다. 회사는 데이터 시각화를 제공하고 데이터 레 이크 내의 모든 데이터 소스를 포함하는 보고 솔루션이 필요합니다. 회사의 관리 팀만 모든 시각화에 대한 전체 액세스 권한을 가져야 합니다. 나머지 회사는 제한된 액세스만 허용해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon QuickSight에서 분석을 생성합니다. 모든 데이터 소스를 연결하고 새 데이터 세트를 만듭니다. 대시보드를 게시하여 데이터를 시각화합니다. 적절한 IAM 역할과 대시보드를
공유합니다.
B. Amazon QuickSight에서 분석을 생성합니다. 모든 데이터 소스를 연결하고 새 데이터 세트를 만듭니다. 대시보드를 게시하여 데이터를 시각화합니다. 적절한 사용자 및 그룹과 대시보
드를 공유합니다.
C. Amazon S3의 데이터에 대한 AWS Glue 테이블 및 크롤러를 생성합니다. AWS Glue 추출, 변환 및 로드(ETL) 작업을 생성하여 보고서를 생성합니다. 보고서를 Amazon S3에 게
시합니다. S3 버킷 정책을 사용하여 보고서에 대한 액세스를 제한합니다.
D. Amazon S3의 데이터에 대한 AWS Glue 테이블 및 크롤러를 생성합니다. Amazon Athena Federated Query를 사용하여 PostgreSQL용 Amazon RDS 내의 데이터에 액세
스합니다. Amazon Athena를 사용하여 보고서를 생성합니다. 보고서를 Amazon S3에 게시합니다. S3 버킷 정책을 사용하여 보고서에 대한 액세스를 제한합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q256
회사는 서로 다른 데이터베이스에서 오는 배치 데이터를 생성합니다. 이 회사는 또한 네트워크 센서 및 애플리케이션 API에서 라이브 스트림 데이터를 생성합니다. 회사는 비즈니스 분석을 위 해 모든 데이터를 한 곳으로 통합해야 합니다. 회사는 수신 데이터를 처리한 다음 다른 Amazon S3 버킷에 데이터를 준비해야 합니다. 팀은 나중에 일회성 쿼리를 실행하고 데이터를 비즈니 스 인텔리전스 도구로 가져와 핵심 성과 지표(KPI)를 표시합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 일회성 쿼리에는 Amazon Athena를 사용하십시오. Amazon QuickSight를 사용하여 KPI용 대시보드를 생성합니다. 
B. 일회성 쿼리에 Amazon Kinesis Data Analytics를 사용합니다. Amazon QuickSight를 사용하여 KPI용 대시보드를 생성합니다. 
C. 데이터베이스에서 Amazon Redshift 클러스터로 개별 레코드를 이동하는 사용자 지정 AWS Lambda 함수를 생성합니다. 
D. AWS Glue 추출, 변환 및 로드(ETL) 작업을 사용하여 데이터를 JSON 형식으로 변환합니다. 여러 Amazon OpenSearch Service(Amazon Elasticsearch Service) 클러스
터에 데이터를 로드합니다.
E. AWS Lake Formation의 청사진을 사용하여 데이터 레이크로 수집할 수 있는 데이터를 식별합니다. AWS Glue를 사용하여 소스를 크롤링하고, 데이터를 추출하고, 데이터를
Apache Parquet 형식으로 Amazon S3에 로드합니다.

<details>
<summary>정답 보기</summary>

**AE**
</details>

---

### Q257
회사에서 온프레미스 PostgreSQL 데이터베이스를 Amazon Aurora PostgreSQL로 마이그레이션하고 있습니다. 온프레미스 데이터베이스는 마이그레이션 중에 온라인 상태를 유지하 고 액세스할 수 있어야 합니다. Aurora 데이터베이스는 온프레미스 데이터베이스와 동기화된 상태를 유지해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자가 수행해야 하는 작업 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 지속적인 복제 작업을 만듭니다. 
B. 온프레미스 데이터베이스의 데이터베이스 백업을 생성합니다. 
C. AWS Database Migration Service(AWS DMS) 복제 서버를 생성합니다. 
D. AWS Schema Conversion Tool(AWS SCT)을 사용하여 데이터베이스 스키마를 변환합니다. 
E. Amazon EventBridge(Amazon CloudWatch Events) 규칙을 생성하여 데이터베이스 동기화를 모니터링합니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q258
회사에서 MySQL 데이터베이스를 온프레미스에서 AWS로 마이그레이션하려고 합니다. 이 회사는 최근 비즈니스에 상당한 영향을 미치는 데이터베이스 중단을 경험했습니다. 이러한 일이 다 시 발생하지 않도록 회사는 데이터 손실을 최소화하고 모든 트랜잭션을 최소 두 개의 노드에 저장하는 안정적인 AWS 데이터베이스 솔루션을 원합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 3개의 가용 영역에 있는 3개의 노드에 대한 동기식 복제로 Amazon RDS DB 인스턴스를 생성합니다. 
B. 다중 AZ 기능이 활성화된 Amazon RDS MySQL DB 인스턴스를 생성하여 데이터를 동기식으로 복제합니다. 
C. Amazon RDS MySQL DB 인스턴스를 생성한 다음 데이터를 동기식으로 복제하는 별도의 AWS 리전에서 읽기 전용 복제본을 생성합니다. 
D. Amazon RDS MySQL DB 인스턴스에 데이터를 동기식으로 복제하기 위해 AWS Lambda 함수를 트리거하는 MySQL 엔진이 설치된 Amazon EC2 인스턴스를 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q259
한 회사가 AWS에서 멀티플레이어 게임 애플리케이션을 호스팅합니다. 회사는 애플리케이션이 밀리초 미만의 대기 시간으로 데이터를 읽고 기록 데이터에 대해 일회성 쿼리를 실행하기를 원 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 자주 액세스하는 데이터에는 Amazon RDS를 사용하십시오. 주기적으로 사용자 지정 스크립트를 실행하여 데이터를 Amazon S3 버킷으로 내보냅니다. 
B. 데이터를 Amazon S3 버킷에 직접 저장합니다. S3 수명 주기 정책을 구현하여 오래된 데이터를 장기 저장을 위해 S3 Glacier Deep Archive로 이동합니다. Amazon Athena를 사
용하여 Amazon S3의 데이터에 대해 일회성 쿼리를 실행합니다.
C. 자주 액세스하는 데이터의 경우 DynamoDB Accelerator(DAX)와 함께 Amazon DynamoDB를 사용합니다. DynamoDB 테이블 내보내기를 사용하여 데이터를 Amazon S3
버킷으로 내보냅니다. Amazon Athena를 사용하여 Amazon S3의 데이터에 대해 일회성 쿼리를 실행합니다.
D. 자주 액세스하는 데이터에는 Amazon DynamoDB를 사용하십시오. Amazon Kinesis Data Streams로 스트리(cid:1535)을 켭니다. Amazon Kinesis Data Firehose를 사용하여
Kinesis Data Streams에서 데이터를 읽습니다. 레코드를 Amazon S3 버킷에 저장합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q260
회사에서 PostgreSQL 데이터베이스를 포함하는 3계층 웹 애플리케이션을 호스팅합니다. 데이터베이스는 문서의 메타데이터를 저장합니다. 회사는 매달 보고서에서 회사가 검토하는 문서를 검색하기 위해 핵심 용어에 대한 메타데이터를 검색합니다. 문서는 Amazon S3에 저장됩니다. 문서는 일반적으로 한 번만 작성되지만 자주 업데이트됩니다. 보고 프로세스는 관계형 쿼리를 사용하여 몇 시간이 걸립니다. 보고 프로세스는 문서 수정 또는 새 문서 추가를 방해해서는 안 됩니다. 이러한 요구 사항을 충족하는 운영상 가장 효율적인 솔루션은 무엇입니까? (2개 선택)
A. 읽기 전용 복제본이 포함된 새로운 Amazon DocumentDB(MongoDB 호환) 클러스터를 설정합니다. 읽기 복제본을 확장하여 보고서를 생성합니다.
B. PostgreSQL 예약 인스턴스용 새 Amazon RDS 및 온디맨드 읽기 전용 복제본을 설정합니다. 읽기 전용 복제본을 확장하여 보고서를 생성합니다.
C. Aurora 복제본이 포함된 새로운 Amazon Aurora PostgreSQL DB 클러스터를 설정합니다. Aurora 복제본에 쿼리를 실행하여 보고서를 생성합니다.
D. PostgreSQL 다중 AZ DB 인스턴스용 새 Amazon RDS를 설정합니다. 보고 모듈이 기본 노드에 영향을 주지 않도록 보조 RDS 노드를 쿼리하도록 보고 모듈을 구성합니다.
E. 문서를 저장할 새 Amazon DynamoDB 테이블을 설정합니다. 새 문서 항목을 지원하려면 된 쓰기 용량을 사용하십시오. 보고서를 지원하기 위해 읽기 용량을 자동으로 확장합니다.

<details>
<summary>정답 보기</summary>

**BC**
</details>

---

### Q261
회사에는 다양한 런타임으로 분당 최대 800회 AWS Lambda 함수를 호출하는 이벤트 기반 애플리케이션이 있습니다. Lambda 함수는 Amazon Aurora MySQL DB 클러스터에 저장 된 데이터에 액세스합니다. 회사는 사용자 활동이 증가함에 따라 연결 시간 초과를 인지하고 있습니다. 데이터베이스는 과부하의 징후를 보이지 않습니다. CPU, 메모리 및 디스크 액세스 메트 릭이 모두 낮습니다. 최소한의 운영 오버헤드로 이 문제를 해결하는 솔루션은 무엇입니까?
A. 더 많은 연결을 처리하려면 Aurora MySQL 노드의 크기를 조정하십시오. 데이터베이스 연결 시도에 대한 Lambda 함수의 재시도 논리를 구성합니다. 
B. Redis용 Amazon ElastiCache를 설정하여 데이터베이스에서 일반적으로 읽은 항목을 캐시합니다. 읽기를 위해 ElastiCache에 연결하도록 Lambda 함수를 구성합니다. 
C. Aurora 복제본을 리더 노드로 추가합니다. 라이터 엔드포인트가 아닌 DB 클러스터의 리더 엔드포인트에 연결하도록 Lambda 함수를 구성합니다. 
D. Amazon RDS 프록시를 사용하여 프록시를 생성합니다. DB 클러스터를 대상 데이터베이스로 설정합니다. DB 클러스터가 아닌 프록시에 연결하도록 Lambda 함수를 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q262
회사는 7개의 Amazon EC2 인스턴스를 사용하여 AWS에서 웹 애플리케이션을 호스팅합니다. 회사는 DNS 쿼리에 대한 응답으로 모든 정상적인 EC2 인스턴스의 IP 주소가 반환되도록 요구합니다. 이 요구 사항을 충족하려면 어떤 정책을 사용해야 합니까?
A. 단순 라우팅 정책 
B. 레이턴시 라우팅 정책 
C. 다중값 라우팅 정책 
D. 지리적 위치 라우팅 정책

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q263
이미지 호스팅 회사는 객체를 Amazon S3 버킷에 저장합니다. 회사는 S3 버킷의 개체가 대중에게 우발적으로 노출되는 것을 방지하려고 합니다. 전체 AWS 계정의 모든 S3 객체는 비공개 로 유지되어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon GuardDuty를 사용하여 S3 버킷 정책을 모니터링합니다. AWS Lambda 함수를 사용하여 객체를 공개하는 변경 사항을 수정하는 자동 수정 작업 규칙을 생성합니다. 
B. AWS Trusted Advisor를 사용하여 공개적으로 액세스 가능한 S3 버킷을 찾습니다. 변경 사항이 감지되면 Trusted Advisor에서 이메일 알림을 구성합니다. 퍼블릭 액세스를 허용하
는 경우 S3 버킷 정책을 수동으로 변경합니다.
C. AWS Resource Access Manager를 사용하여 공개적으로 액세스 가능한 S3 버킷을 찾습니다. 변경이 감지되면 Amazon Simple Notification Service(Amazon SNS)를 사
용하여 AWS Lambda 함수를 호출합니다. 프로그래(cid:1535) 방식으로 변경 사항을 수정하는 Lambda 함수를 배포합니다.
D. 계정 수준에서 S3 퍼블릭 액세스 차단 기능을 사용합니다. AWS Organizations를 사용하여 IAM 사용자가 설정을 변경하지 못하도록 하는 서비스 제어 정책(SCP)을 생성합니다. 계
정에 SCP를 적용합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q264
회사에는 자동차의 IoT 센서에서 데이터를 수집하는 애플리케이션이 있습니다. 데이터는 Amazon Kinesis Data Firehose를 통해 Amazon S3에 스트리(cid:1535) 및 저장됩니다. 데이터는 매 년 수조 개의 S3 객체를 생성합니다. 매일 아침 회사는 지난 30일 동안의 데이터를 사용하여 일련의 기계 학습(ML) 모델을 재교육합니다. 매년 4회 회사는 이전 12개월의 데이터를 사용하여 분석을 수행하고 다른 ML 모델을 교육합니다. 데이터는 최대 1년 동안 최소한의 지연으로 사용할 수 있어야 합니다. 1년 후에는 데이터를 보관 목적으로 보관해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 스토리지 솔루션은 무엇입니까?
A. S3 Intelligent-Tiering 스토리지 클래스를 사용합니다. 1년 후 객체를 S3 Glacier Deep Archive로 전환하는 S3 수명 주기 정책을 생성합니다. 
B. S3 Intelligent-Tiering 스토리지 클래스를 사용합니다. 1년 후 자동으로 객체를 S3 Glacier Deep Archive로 이동하도록 S3 Intelligent-Tiering을 구성합니다. 
C. S3 Standard-Infrequent Access(S3 Standard-IA) 스토리지 클래스를 사용합니다. 1년 후 객체를 S3 Glacier Deep Archive로 전환하는 S3 수명 주기 정책을 생성합니다. 
D. S3 Standard 스토리지 클래스를 사용합니다. 30일 후에 객체를 S3 Standard-Infrequent Access(S3 Standard-IA)로 전환한 다음 1년 후에 S3 Glacier Deep Archive로 전
환하는 S3 수명 주기 정책을 생성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q265
솔루션 설계자는 회사의 스토리지 비용을 줄이기 위해 솔루션을 구현해야 합니다. 회사의 모든 데이터는 Amazon S3 Standard 스토리지 클래스에 있습니다. 회사는 모든 데이터를 최소 25 년 동안 보관해야 합니다. 가장 최근 2년 간의 데이터는 가용성이 높고 즉시 검색할 수 있어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. S3 수명 주기 정책을 설정하여 객체를 S3 Glacier Deep Archive로 즉시 전환하십시오. 
B. 2년 후 객체를 S3 Glacier Deep Archive로 전환하도록 S3 수명 주기 정책을 설정합니다. 
C. S3 Intelligent-Tiering을 사용합니다. 보관 옵션을 활성화하여 데이터가 S3 Glacier Deep Archive에 보관되도록 합니다. 
D. 객체를 S3 One Zone-Infrequent Access(S3 One Zone-IA)로 즉시 전환하고 2년 후에 S3 Glacier Deep Archive로 전환하도록 S3 수명 주기 정책을 설정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q266
게임 회사는 AWS에서 브라우저 기반 애플리케이션을 호스팅합니다. 애플리케이션 사용자는 Amazon S3에 저장된 많은 수의 비디오 및 이미지를 소비합니다. 이 내용은 모든 사용자에게 동일합니다. 이 응용 프로그램은 인기가 높아졌으며 전 세계적으로 수백만 명의 사용자가 이러한 미디어 파일에 액세스합니다. 회사는 원본에 대한 부하를 줄이면서 사용자에게 파일을 제공하려고 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 웹 서버 앞에 AWS Global Accelerator 액셀러레이터를 배포합니다. 
B. S3 버킷 앞에 Amazon CloudFront 웹 배포를 배포합니다. 
C. 웹 서버 앞에 Redis 인스턴스용 Amazon ElastiCache를 배포합니다. 
D. 웹 서버 앞에 Amazon ElastiCache for Memcached 인스턴스를 배포합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q267
회사에서 내부 감사를 실시하고 있습니다. 회사는 회사의 AWS Lake Formation 데이터 레이크와 연결된 Amazon S3 버킷의 데이터에 민감한 고객 또는 직원 데이터가 포함되지 않도록 하려고 합니다. 회사는 개인 식별 정보(PII) 또는 여권 번호 및 신용 카드 번호를 포함한 금융 정보를 검색하려고 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 계정에서 AWS Audit Manager를 구성합니다. 감사를 위해 PCI DSS(Payment Card Industry Data Security Standards)를 선택합니다. 
B. S3 버킷에서 Amazon S3 인벤토리 구성 인벤토리를 쿼리하도록 Amazon Athena를 구성합니다. 
C. 필요한 데이터 유형에 대해 관리형 식별자를 사용하는 데이터 검색 작업을 실행하도록 Amazon Macie를 구성합니다. 
D. Amazon S3 Select를 사용하여 S3 버킷에서 보고서를 실행합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q268
기상 스타트업 회사는 사용자에게 날씨 데이터를 온라인으로 판매하는 맞춤형 웹 애플리케이션을 보유하고 있습니다. 이 회사는 Amazon DynamoDB를 사용하여 데이터를 저장하고 새로운 날씨 이벤트가 기록될 때마다 4개의 내부 팀 관리자에게 경고를 보내는 새로운 서비스를 구축하려고 합니다. 회사는 이 새로운 서비스가 현재 애플리케이션의 성능에 영향을 미치는 것을 원하 지 않습니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하려면 솔루션 설계자가 무엇을 해야 합니까?
A. DynamoDB 트랜잭션을 사용하여 새 이벤트 데이터를 테이블에 씁니다. 내부 팀에 알리도록 트랜잭션을 구성합니다. 
B. 현재 애플리케이션이 4개의 Amazon Simple Notification Service(Amazon SNS) 주제에 메시지를 게시하도록 합니다. 각 팀이 하나의 주제를 구독하도록 합니다. 
C. 테이블에서 Amazon DynamoDB 스트림을 활성화합니다. 트리거를 사용하여 팀이 구독할 수 있는 단일 Amazon Simple Notification Service(Amazon SNS) 주제에 씁니다. 
D. 각 레코드에 사용자 정의 속성을 추가하여 새 항목에 플래그를 지정합니다. 새 항목이 있는지 매분 테이블을 스캔하고 팀이 구독할 수 있는 Amazon Simple Queue Service
(Amazon SQS) 대기열에 알리는 cron 작업을 작성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q269
회사는 Salesforce 계정과 Amazon S3 간에 데이터를 안전하게 교환하고자 합니다. 회사는 AWS Key Management Service (AWS KMS) 고객 관리 키 (CMK)를 사용하여 데이터 를 휴식 상태에서 암호화해야 합니다. 또한 데이터를 전송 중에도 암호화해야 합니다. 회사는 Salesforce 계정에 대한 API 액세스를 활성화했습니다. 가장 적은 개발 노력으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Salesforce에서 Amazon S3로 데이터를 안전하게 전송하기 위해 AWS Lambda 함수를 생성합니다. 
B. AWS Step Functions 워크플로우를 생성합니다. Salesforce에서 Amazon S3로 데이터를 안전하게 전송하는 작업을 정의합니다. 
C. Amazon AppFlow 플로우를 생성합니다. Salesforce에서 Amazon S3로 데이터를 안전하게 전송합니다. 
D. Salesforce에서 Amazon S3로 데이터를 안전하게 전송하기 위해 사용자 정의 커넥터를 생성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q270
회사에서 새로운 웹 기반 고객 관계 관리 애플리케이션을 구축하고 있습니다. 애플리케이션은 Application Load Balancer(ALB) 뒤에 있는 Amazon Elastic Block Store(Amazon EBS) 볼륨이 지원하는 여러 Amazon EC2 인스턴스를 사용합니다. 이 애플리케이션은 Amazon Aurora 데이터베이스도 사용합니다. 애플리케이션의 모든 데이터는 유휴 및 전송 중에 암 호화되어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. ALB에서 AWS Key Management Service(AWS KMS) 인증서를 사용하여 전송 중인 데이터를 암호화합니다. AWS Certificate Manager(ACM)를 사용하여 유휴 상태의
EBS 볼륨 및 Aurora 데이터베이스 스토리지를 암호화합니다.
B. AWS 루트 계정을 사용하여 AWS Management Console에 로그인합니다. 회사의 암호화 인증서를 업로드합니다. 루트 계정에 있는 동안 계정의 저장 및 전송 중인 모든 데이터에 대
해 암호화를 켜는 옵션을 선택합니다.
C. AWS Key Management Service(AWS KMS)를 사용하여 유휴 상태의 EBS 볼륨 및 Aurora 데이터베이스 스토리지를 암호화합니다. ALB에 AWS Certificate Manager
(ACM) 인증서를 연결하여 전송 중인 데이터를 암호화합니다.
D. BitLocker를 사용하여 유휴 상태의 모든 데이터를 암호화합니다. 회사의 TLS 인증서 키를 AWS Key Management Service(AWS KMS)로 가져옵니다. KMS 키를 ALB에 연결
하여 전송 중인 데이터를 암호화합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q271
회사에는 다음으로 구성된 데이터 수집 워크플로가 있습니다. * 새로운 데이터 전달에 대한 알림을 위한 Amazon Simple Notification Service(Amazon SNS) 주제 * 데이터를 처리하고 메타데이터를 기록하는 AWS Lambda 함수 수집 워크플로가 실패하는 것을 회사에서 관찰합니다. 때때로 네트워크 연결 문제로 인해. 이러한 실패가 발생하면 회사에서 수동으로 작업을 다시 실행하지 않는 한 Lambda 함수는 해당 데 이터를 수집하지 않습니다. Lambda 함수가 미래에 모든 데이터를 수집하도록 하기 위해 솔루션 설계자는 어떤 작업 조합을 취해야 합니까? (두 가지를 선택하세요.)
A. 여러 가용 영역에 Lambda 함수를 배포합니다. 
B. Amazon Simple Queue Service(Amazon SQS) 대기열을 생성하고 SNS 주제를 구독합니다. 
C. Lambda 함수에 할당된 CPU와 메모리를 늘립니다. 
D. Lambda 함수에 대해 프로비저닝된 처리량을 늘립니다. 
E. Amazon Simple Queue Service(Amazon SQS) 대기열에서 읽도록 Lambda 함수를 수정합니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q272
회사는 Amazon EC2 인스턴스와 Amazon RDS에서 2계층 애플리케이션을 호스팅합니다. 응용 프로그램의 요구 사항은 시간에 따라 다릅니다. 업무 시간 이후와 주말에는 부하가 최소화 됩니다. EC2 인스턴스는 최소 2개의 인스턴스와 최대 5개의 인스턴스로 구성된 EC2 Auto Scaling 그룹에서 실행됩니다. 응용 프로그램은 항상 사용할 수 있어야 하지만 회사는 전체 비용 에 대해 우려하고 있습니다. 비용 효율적으로 가용성 요구 사항을 가장 잘 충족하는 솔루션은 무엇입니까?
A. 모든 EC2 스팟 인스턴스를 사용하십시오. 사용하지 않을 때는 RDS 데이터베이스를 중지하십시오. 
B. 5개의 EC2 인스턴스에 적용되는 EC2 Instance Savings Plans를 구입합니다. RDS 예약 DB 인스턴스를 구매합니다. 
C. 2개의 EC2 예약 인스턴스를 구입합니다. 필요에 따라 최대 3개의 추가 EC2 스팟 인스턴스를 사용합니다. 사용하지 않을 때는 RDS 데이터베이스를 중지하십시오. 
D. 2개의 EC2 인스턴스에 적용되는 EC2 Instance Savings Plans를 구입합니다. 필요에 따라 최대 3개의 추가 EC2 온디맨드 인스턴스를 사용합니다. RDS 예약 DB 인스턴스를 구
매합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q273
보고 팀은 매일 Amazon S3 버킷에서 파일을 받습니다. 보고 팀은 Amazon QuickSight에서 사용하기 위해 매일 동시에 이 초기 S3 버킷에서 분석 S3 버킷으로 파일을 수동으로 검토하 고 복사합니다. 더 많은 팀이 더 큰 크기의 더 많은 파일을 초기 S3 버킷으로 보내기 시작했습니다. 보고 팀은 파일이 초기 S3 버킷에 들어갈 때 자동으로 파일 분석 S3 버킷을 이동하려고 합니다. 보고 팀은 또한 AWS Lambda 함수를 사용하여 복사된 데이터에서 패턴 일치 코드를 실행하 려고 합니다. 또한 보고 팀은 데이터 파일을 Amazon SageMaker Pipelines의 파이프라인으로 보내려고 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 분석 S3 버킷에 파일을 복사하는 Lambda 함수를 생성합니다. 분석 S3 버킷에 대한 S3 이벤트 알림을 생성합니다. 이벤트 알림의 대상으로 Lambda 및 SageMaker 파이프라인을
구성합니다. s3:ObjectCreated:Put을 이벤트 유형으로 구성합니다.
B. 분석 S3 버킷에 파일을 복사하는 Lambda 함수를 생성합니다. Amazon EventBridge(Amazon CloudWatch Events)에 이벤트 알림을 보내도록 분석 S3 버킷을 구성합니다.
EventBridge(CloudWatch 이벤트)에서 ObjectCreated 규칙을 구성합니다. Lambda 및 SageMaker 파이프라인을 규칙의 대상으로 구성합니다.
C. S3 버킷 간에 S3 복제를 구성합니다. 분석 S3 버킷에 대한 S3 이벤트 알림을 생성합니다. 이벤트 알림의 대상으로 Lambda 및 SageMaker 파이프라인을 구성합니다.
s3:ObjectCreated:Put을 이벤트 유형으로 구성합니다.
D. S3 버킷 간에 S3 복제를 구성합니다. Amazon EventBridge(Amazon CloudWatch Events)에 이벤트 알림을 보내도록 분석 S3 버킷을 구성합니다. EventBridge
(CloudWatch 이벤트)에서 ObjectCreated 규칙을 구성합니다. Lambda 및 SageMaker 파이프라인을 규칙의 대상으로 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q274
회사는 Amazon Aurora MySQL DB 클러스터를 스토리지로 사용하는 다중 계층 웹 애플리케이션을 호스팅합니다. 애플리케이션 계층은 Amazon EC2 인스턴스에서 호스팅됩니다. 회사 의 IT 보안 지침에 따라 데이터베이스 자격 증명을 암호화하고 14일마다 교체해야 합니다. 최소한의 운영 노력으로 이 요구 사항을 충족하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 새 AWS Key Management Service(AWS KMS) 암호화 키를 생성합니다. AWS Secrets Manager를 사용하여 적절한 자격 증명과 함께 KMS 키를 사용하는 새 암호를 생성합
니다. 암호를 Aurora DB 클러스터와 연결합니다. 14일의 사용자 지정 순환 기간을 구성합니다.
B. AWS Systems Manager Parameter Store에서 두 개의 매개변수를 생성합니다. 하나는 사용자 이름을 문자열 매개변수로 사용하고 다른 하나는 SecureString 유형을 암호로 사
용합니다. 암호 매개변수에 대해 AWS Key Management Service(AWS KMS) 암호화를 선택하고 애플리케이션 계층에서 이러한 매개변수를 로드합니다. 14일마다 암호를 교체하 는 AWS Lambda 함수를 구현합니다.
C. 자격 증명이 포함된 파일을 AWS KMS(AWS Key Management Service) 암호화 Amazon Elastic File System(Amazon EFS) 파일 시스템에 저장합니다. 애플리케이션 계
층의 모든 EC2 인스턴스에 EFS 파일 시스템을 탑재합니다. 응용 프로그램이 파일을 읽을 수 있고 슈퍼 사용자만 파일을 수정할 수 있도록 파일 시스템의 파일에 대한 액세스를 제한합니 다. 14일마다 Aurora에서 키를 교체하고 새 자격 증명을 파일에 쓰는 AWS Lambda 함수를 구현합니다.
D. 애플리케이션이 자격 증명을 로드하는 데 사용하는 AWS KMS(AWS Key Management Service) 암호화 Amazon S3 버킷에 자격 증명이 포함된 파일을 저장합니다. 올바른 자
격 증명이 사용되도록 정기적으로 파일을 응용 프로그램에 다운로드하십시오. 14일마다 Aurora 자격 증명을 교체하고 이 자격 증명을 S3 버킷의 파일에 업로드하는 AWS Lambda 함 수를 구현합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q275
회사에는 Amazon RDS MySQL DB 인스턴스에서 정보를 검색하는 자격 증명이 내장된 사용자 지정 애플리케이션이 있습니다. 경영진은 최소한의 프로그래(cid:1535) 노력으로 애플리케이션을 더 안전하게 만들어야 한다고 말합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS Key Management Service(AWS KMS)를 사용하여 키를 생성합니다. AWS KMS에서 데이터베이스 자격 증명을 로드하도록 애플리케이션을 구성합니다. 자동 키 순환을
활성화합니다.
B. 애플리케이션 사용자를 위해 RDS for MySQL 데이터베이스에서 자격 증명을 생성하고 자격 증명을 AWS Secrets Manager에 저장합니다. Secrets Manager에서 데이터베이스
자격 증명을 로드하도록 애플리케이션을 구성합니다. Secret Manager에서 자격 증명을 교체하는 AWS Lambda 함수를 생성합니다.
C. 애플리케이션 사용자를 위해 RDS for MySQL 데이터베이스에서 자격 증명을 생성하고 자격 증명을 AWS Secrets Manager에 저장합니다. Secrets Manager에서 데이터베이스
자격 증명을 로드하도록 애플리케이션을 구성합니다. Secrets Manager를 사용하여 RDS for MySQL 데이터베이스에서 애플리케이션 사용자의 자격 증명 교체 일정을 설정합니다.
D. 애플리케이션 사용자를 위해 RDS for MySQL 데이터베이스에서 자격 증명을 생성하고 자격 증명을 AWS Systems Manager Parameter Store에 저장합니다. Parameter
Store에서 데이터베이스 자격 증명을 로드하도록 애플리케이션을 구성합니다. Parameter Store를 사용하여 RDS for MySQL 데이터베이스에서 애플리케이션 사용자에 대한 자격 증명 교체 일정을 설정합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q276
회사에서 Linux 기반 웹 서버 그룹을 AWS로 마이그레이션하고 있습니다. 웹 서버는 일부 콘텐츠에 대해 공유 파일 저장소의 파일에 액세스해야 합니다. 회사는 신청서를 변경해서는 안됩니 다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 웹 서버에 대한 액세스 권한이 있는 Amazon S3 Standard 버킷을 생성합니다. 
B. Amazon S3 버킷을 원본으로 사용하여 Amazon CloudFront 배포를 구성합니다. 
C. Amazon Elastic File System(Amazon EFS) 파일 시스템을 생성합니다. 모든 웹 서버에 EFS 파일 시스템을 마운트합니다. 
D. 범용 SSD(gp3) Amazon Elastic Block Store(Amazon EBS) 볼륨을 구성합니다. 모든 웹 서버에 EBS 볼륨을 마운트합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q277
회사는 회사 웹 사이트에 널리 사용되는 콘텐츠 관리 시스템(CMS)을 사용합니다. 그러나 필요한 패칭과 유지보수가 부담스럽다. 회사는 웹사이트를 재설계하고 있으며 새로운 솔루션을 원합 니다. 웹사이트는 1년에 4번 업데이트되며 동적 콘텐츠를 사용할 필요가 없습니다. 솔루션은 높은 확장성과 향상된 보안을 제공해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 변경 조합은 무엇입니까? (두 가지를 선택하세요.)
A. HTTPS 기능을 사용하도록 웹 사이트 앞에 Amazon CloudFront를 구성합니다. 
B. 웹 사이트 앞에 AWS WAF 웹 ACL을 배포하여 HTTPS 기능을 제공합니다. 
C. 웹 사이트 콘텐츠를 관리하고 제공하기 위해 AWS Lambda 함수를 생성하고 배포합니다. 
D. 새 웹사이트와 Amazon S3 버킷을 생성합니다. 정적 웹 사이트 호스팅이 활성화된 S3 버킷에 웹 사이트를 배포합니다. 
E. 새 웹사이트를 만듭니다. Application Load Balancer 뒤에 있는 Amazon EC2 인스턴스의 Auto Scaling 그룹을 사용하여 웹 사이트를 배포합니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q278
회사는 단일 VPC의 Amazon EC2 인스턴스에서 고가용성 이미지 처리 애플리케이션을 실행합니다. EC2 인스턴스는 여러 가용 영역에 걸쳐 여러 서브넷 내에서 실행됩니다. EC2 인스턴 스는 서로 통신하지 않습니다. 그러나 EC2 인스턴스는 Amazon S3에서 이미지를 다운로드하고 단일 NAT 게이트웨이를 통해 Amazon S3에 이미지를 업로드합니다. 회사는 데이터 전송 요금에 대해 우려하고 있습니다. 회사가 지역 데이터 전송 요금을 피하는 가장 비용 효율적인 방법은 무엇입니까?
A. 각 가용 영역에서 NAT 게이트웨이를 시작합니다. 
B. NAT 게이트웨이를 NAT 인스턴스로 교체합니다. 
C. Amazon S3용 게이트웨이 VPC 엔드포인트를 배포합니다. 
D. EC2 인스턴스를 실행할 EC2 전용 호스트를 프로비저닝합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q279
회사는 디지털 미디어 스트리(cid:1535) 애플리케이션을 호스팅하기 위해 Amazon Elastic Kubernetes Service(Amazon EKS) 클러스터를 생성해야 합니다. EKS 클러스터는 저장을 위해 Amazon Elastic Block Store(Amazon EBS) 볼륨이 지원하는 관리형 노드 그룹을 사용합니다. 회사는 AWS Key Management Service(AWS KMS)에 저장된 고객 관리형 키를 사용하여 유휴 상태의 모든 데이터를 암호화해야 합니다. 최소한의 운영 오버헤드로 이 요구 사항을 충족하는 작업 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 고객 관리 키를 사용하는 Kubernetes 플러그인을 사용하여 데이터 암호화를 수행합니다. 
B. EKS 클러스터 생성 후 EBS 볼륨을 찾습니다. 고객 관리형 키를 사용하여 암호화를 활성화합니다. 
C. EKS 클러스터가 생성될 AWS 리전에서 기본적으로 EBS 암호화를 활성화합니다. 고객 관리형 키를 기본 키로 선택합니다. 
D. EKS 클러스터를 생성합니다. 고객 관리형 키에 대한 권한을 부여하는 정책이 있는 IAM 역할을 생성합니다. 역할을 EKS 클러스터와 연결합니다. 
E. 고객 관리형 키를 EKS 클러스터에 Kubernetes 비밀로 저장합니다. 고객 관리형 키를 사용하여 EBS 볼륨을 암호화합니다.

<details>
<summary>정답 보기</summary>

**CD**
</details>

---

### Q280
회사는 PostgreSQL DB 인스턴스용 Amazon RDS를 사용하여 웹 서버 플릿을 실행합니다. 일상적인 규정 준수 검사 후 회사는 모든 프로덕션 데이터베이스에 대해 1초 미만의 복구 지점 목표(RPO)를 요구하는 표준을 설정합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. DB 인스턴스에 대해 다중 AZ 배포를 활성화합니다. 
B. 하나의 가용 영역에서 DB 인스턴스에 대해 Auto Scaling을 활성화합니다. 
C. 하나의 가용 영역에서 DB 인스턴스를 구성하고 별도의 가용 영역에서 여러 읽기 전용 복제본을 생성합니다. 
D. 하나의 가용 영역에서 DB 인스턴스를 구성하고 AWS DMS(AWS Database Migration Service) 변경 데이터 캡처(CDC) 작업을 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q281
회사에는 이벤트 데이터를 생성하는 서비스가 있습니다. 회사는 AWS를 사용하여 수신된 이벤트 데이터를 처리하려고 합니다. 데이터는 처리 전반에 걸쳐 유지되어야 하는 특정 순서로 기록됩 니다. 회사는 운영 오버헤드를 최소화하는 솔루션을 구현하려고 합니다. 솔루션 설계자는 이를 어떻게 달성해야 합니까?
A. 메시지를 보관할 Amazon Simple Queue Service(Amazon SQS) FIFO 대기열을 생성합니다. 대기열의 메시지를 처리하도록 AWS Lambda 함수를 설정합니다. 
B. 처리할 페이로드가 포함된 알림을 전달할 Amazon Simple Notification Service(Amazon SNS) 주제를 생성합니다. AWS Lambda 함수를 구독자로 구성합니다. 
C. 메시지를 보관할 Amazon Simple Queue Service(Amazon SQS) 표준 대기열을 생성합니다. 대기열의 메시지를 독립적으로 처리하도록 AWS Lambda 함수를 설정합니다. 
D. 처리할 페이로드가 포함된 알림을 전달할 Amazon Simple Notification Service(Amazon SNS) 주제를 생성합니다. Amazon Simple Queue Service(Amazon SQS) 대기
열을 구독자로 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q282
한 회사가 AWS에서 3계층 애플리케이션을 구축하고 있습니다. 프레젠테이션 계층은 정적 웹 사이트를 제공합니다. 논리 계층은 컨테이너화된 애플리케이션입니다. 이 응용 프로그램은 관계 형 데이터베이스에 데이터를 저장합니다. 이 회사는 배포를 단순화하고 운영 비용을 절감하기를 원합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon S3를 사용하여 정적 콘텐츠를 호스팅합니다. 컴퓨팅 성능을 위해 AWS Fargate와 함께 Amazon Elastic Container Service(Amazon ECS)를 사용합니다. 데이터베
이스에 대해 관리형 Amazon RDS 클러스터를 사용합니다.
B. Amazon CloudFront를 사용하여 정적 콘텐츠를 호스팅합니다. 컴퓨팅 성능을 위해 Amazon EC2와 함께 Amazon Elastic Container Service(Amazon ECS)를 사용합니다.
데이터베이스에 대해 관리형 Amazon RDS 클러스터를 사용합니다.
C. Amazon S3를 사용하여 정적 콘텐츠를 호스팅합니다. 컴퓨팅 성능을 위해 AWS Fargate와 함께 Amazon Elastic Kubernetes Service(Amazon EKS)를 사용합니다. 데이터
베이스에 대해 관리형 Amazon RDS 클러스터를 사용합니다.
D. Amazon EC2 예약 인스턴스를 사용하여 정적 콘텐츠를 호스팅합니다. 컴퓨팅 성능을 위해 Amazon EC2와 함께 Amazon Elastic Kubernetes Service(Amazon EKS)를 사
용합니다. 데이터베이스에 대해 관리형 Amazon RDS 클러스터를 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q283
회사에서 VPC에 2계층 웹 애플리케이션을 배포하고 있습니다. 웹 계층은 여러 가용 영역에 걸쳐 있는 퍼블릭 서브넷이 있는 Amazon EC2 Auto Scaling 그룹을 사용하고 있습니다. 데이 터베이스 계층은 별도의 프라이빗 서브넷에 있는 MySQL DB 인스턴스용 Amazon RDS로 구성됩니다. 웹 계층은 제품 정보를 검색하기 위해 데이터베이스에 액세스해야 합니다. 웹 응용 프로그램이 의도한 대로 작동하지 않습니다. 웹 애플리케이션에서 데이터베이스에 연결할 수 없다고 보고합니다. 데이터베이스가 가동 및 실행 중인 것으로 확인되었습니다. 네트워크 ACL, 보안 그룹 및 라우팅 테이블에 대한 모든 구성은 여전히 기본 상태입니다. 애플리케이션 수정을 위해 솔루션 아키텍트는 무엇을 추천해야 합니까?
A. 프라이빗 서브넷의 네트워크 ACL에 명시적 규칙을 추가하여 웹 티어의 EC2 인스턴스에서 오는 트래픽을 허용합니다. 
B. 웹 계층의 EC2 인스턴스와 데이터베이스 계층 간의 트래픽을 허용하도록 VPC 경로 테이블에 경로를 추가합니다. 
C. 웹 계층의 EC2 인스턴스와 데이터베이스 계층의 RDS 인스턴스를 두 개의 개별 VPC에 배포하고 VPC 피어링을 구성합니다. 
D. 데이터베이스 계층 RDS 인스턴스의 보안 그룹에 인바운드 규칙을 추가하여 웹 계층 보안 그룹의 트래픽을 허용합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q284
회사가 단일 AWS 리전에서 모바일 게임 앱을 개발하고 있습니다. 앱은 Auto Scaling 그룹의 여러 Amazon EC2 인스턴스에서 실행됩니다. 회사는 앱 데이터를 Amazon DynamoDB 에 저장합니다. 앱은 사용자와 서버 간에 TCP 및 UDP 트래픽을 사용하여 통신합니다. 이 응용 프로그램은 전 세계적으로 사용되며 회사는 모든 사용자에게 가능한 가장 낮은 대기 시간을 보 장하고자 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Global Accelerator를 사용하여 가속기를 생성합니다. Global Accelerator 통합을 사용하고 TCP 및 UDP 포트에서 수신 대기하는 가속기 엔드포인트 뒤에 Application
Load Balancer(ALB)를 생성합니다. Auto Scaling 그룹을 업데이트하여 ALB에 인스턴스를 등록합니다.
B. AWS Global Accelerator를 사용하여 가속기를 생성합니다. Global Accelerator 통합을 사용하고 TCP 및 UDP 포트에서 수신 대기하는 가속기 엔드포인트 뒤에 NLB(Network
Load Balancer)를 생성합니다. Auto Scaling 그룹을 업데이트하여 NLB에 인스턴스를 등록합니다.
C. Amazon CloudFront 콘텐츠 전송 네트워크(CDN) 엔드포인트를 생성합니다. 엔드포인트 뒤에 NLB(Network Load Balancer)를 생성하고 TCP 및 UDP 포트에서 수신 대기합
니다. Auto Scaling 그룹을 업데이트하여 NLB에 인스턴스를 등록합니다. NLB를 오리진으로 사용하도록 CloudFront를 업데이트합니다.
D. Amazon CloudFront 콘텐츠 전송 네트워크(CDN) 엔드포인트를 생성합니다. 엔드포인트 뒤에 ALB(Application Load Balancer)를 생성하고 TCP 및 UDP 포트에서 수신 대기
합니다. Auto Scaling 그룹을 업데이트하여 ALB에 인스턴스를 등록합니다. ALB를 오리진으로 사용하도록 CloudFront를 업데이트합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q285
회사에 Amazon DynamoDB 테이블이 지원하는 애플리케이션이 있습니다. 회사의 규정 준수 요구 사항은 데이터베이스 백업을 매월 수행하고 6개월 동안 사용할 수 있어야 하며 7년 동안 유지해야 한다고 지정합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 매월 1일에 DynamoDB 테이블을 백업하는 AWS Backup 계획을 생성합니다. 6개월 후 백업을 콜드 스토리지로 전환하는 수명 주기 정책을 지정합니다. 각 백업의 보존 기간을 7년으
로 설정합니다.
B. 매월 1일에 DynamoDB 테이블의 DynamoDB 온디맨드 백업을 생성합니다. 6개월 후 백업을 Amazon S3 Glacier Flexible Retrieval로 전환합니다. 7년보다 오래된 백업을 삭
제하려면 S3 수명 주기 정책을 생성하십시오.
C. AWS SDK를 사용하여 DynamoDB 테이블의 온디맨드 백업을 생성하는 스크립트를 개발합니다. 매월 1일에 스크립트를 실행하는 Amazon EventBridge 규칙을 설정합니다. 6개
월 이상 된 DynamoDB 백업을 콜드 스토리지로 전환하고 7년 이상 된 백업을 삭제하기 위해 매월 2일에 실행할 두 번째 스크립트를 생성합니다.
D. AWS CLI를 사용하여 DynamoDB 테이블의 온디맨드 백업을 생성합니다. Cron 표현식을 사용하여 매월 1일에 명령을 실행하는 Amazon EventBridge 규칙을 설정합니다. 6개월
후 백업을 콜드 스토리지로 전환하고 7년 후 백업을 삭제하도록 명령에 지정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q286
결제 처리 회사는 고객과의 모든 음성 통신을 녹음하고 오디오 파일을 Amazon S3 버킷에 저장합니다. 회사는 오디오 파일에서 텍스트를 캡처해야 합니다. 회사는 텍스트에서 고객에게 속한 모든 개인 식별 정보(PII)를 제거해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Amazon Kinesis Video Streams를 사용하여 오디오 파일을 처리합니다. AWS Lambda 함수를 사용하여 알려진 PII 패턴을 스캔합니다. 
B. 오디오 파일이 S3 버킷에 업로드되면 AWS Lambda 함수를 호출하여 Amazon Textract 작업을 시작하여 통화 녹음을 분석합니다. 
C. PII 수정을 켠 상태로 Amazon Transcribe 전사 작업을 구성합니다. 오디오 파일이 S3 버킷에 업로드되면 AWS Lambda 함수를 호출하여 전사 작업을 시작합니다. 출력을 별도의
S3 버킷에 저장합니다.
D. 트랜스크립션이 켜진 오디오 파일을 수집하는 Amazon Connect 고객 응대 흐름을 생성합니다. 알려진 PII 패턴을 스캔하기 위해 AWS Lambda 함수를 포함합니다. 오디오 파일이
S3 버킷에 업로드되면 Amazon EventBridge를 사용하여 고객 응대 흐름을 시작하십시오.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q287
회사는 AWS CloudTrail 로그를 3년 동안 보관해야 합니다. 회사는 상위 계정의 AWS Organizations를 사용하여 AWS 계정 집합에 CloudTrail을 적용하고 있습니다. CloudTrail 대 상 S3 버킷은 S3 버전 관리가 활성화된 상태로 구성됩니다. 3년 후 현재 객체를 삭제하는 S3 수명 주기 정책이 있습니다. S3 버킷 사용 4년차 이후 S3 버킷 지표는 개체 수가 계속 증가했음을 보여줍니다. 그러나 S3 버킷에 전달되는 새 CloudTrail 로그의 수는 일관되게 유지되었습니다. 가장 비용 효율적인 방식으로 3년 이상 된 개체를 삭제하는 솔루션은 무엇입니까?
A. 3년 후에 개체가 만료되도록 조직의 중앙 집중식 CloudTrail 추적을 구성합니다. 
B. 현재 버전뿐만 아니라 이전 버전도 삭제하도록 S3 수명 주기 정책을 구성합니다. 
C. Amazon S3에서 3년 이상 된 객체를 열거하고 삭제하는 AWS Lambda 함수를 생성합니다. 
D. 상위 계정을 S3 버킷으로 전달되는 모든 객체의 소유자로 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q288
한 회사가 AWS에서 온라인 트랜잭션 처리(OLTP) 워크로드를 실행하고 있습니다. 이 워크로드는 다중 AZ 배포에서 암호화되지 않은 Amazon RDS DB 인스턴스를 사용합니다. 매일 데 이터베이스 스냅샷은 이 인스턴스에서 가져옵니다. 앞으로 데이터베이스와 스냅샷이 항상 암호화되도록 하기 위해 솔루션 설계자는 어떻게 해야 합니까?
A. 최신 DB 스냅샷 사본을 암호화한다. 암호화된 스냅샷을 복원하여 기존 DB 인스턴스를 교체합니다. 
B. 새로운 암호화된 Amazon Elastic Block Store(Amazon EBS) 볼륨을 생성하고 여기에 스냅샷을 복사합니다. DB 인스턴스에서 암호화를 활성화합니다. 
C. 스냅샷을 복사하고 AWS Key Management Service(AWS KMS)를 사용하여 암호화를 활성화합니다. 암호화된 스냅샷을 기존 DB 인스턴스로 복원합니다. 
D. AWS Key Management Service(AWS KMS) 관리형 키(SSE-KMS)로 서버 측 암호화를 사용하여 암호화된 Amazon S3 버킷에 스냅샷을 복사합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q289
한 전자상거래 회사가 AWS에서 하루에 하나의 거래 웹사이트를 시작하려고 합니다. 매일 24시간 동안 정확히 하나의 제품이 판매됩니다. 이 회사는 사용량이 많은 시간에 밀리초 대기 시간 으로 시간당 수백만 건의 요청을 처리할 수 있기를 원합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon S3를 사용하여 다른 S3 버킷에서 전체 웹 사이트를 호스팅합니다. Amazon CloudFront 배포를 추가합니다. S3 버킷을 배포의 원본으로 설정합니다. 주문 데이터를
Amazon S3에 저장합니다.
B. 여러 가용 영역의 Auto Scaling 그룹에서 실행되는 Amazon EC2 인스턴스에 전체 웹 사이트를 배포합니다. ALB(Application Load Balancer)를 추가하여 웹 사이트 트래픽을 분
산합니다. 백엔드 API에 대해 다른 ALB를 추가하십시오. MySQL용 Amazon RDS에 데이터를 저장합니다.
C. 전체 애플리케이션을 마이그레이션하여 컨테이너에서 실행합니다. Amazon Elastic Kubernetes Service(Amazon EKS)에서 컨테이너를 호스팅합니다. Kubernetes Cluster
Autoscaler를 사용하여 팟(Pod) 수를 늘리거나 줄여 트래픽의 버스트를 처리합니다. MySQL용 Amazon RDS에 데이터를 저장합니다.
D. Amazon S3 버킷을 사용하여 웹 사이트의 정적 콘텐츠를 호스팅합니다. Amazon CloudFront 배포를 배포합니다. S3 버킷을 오리진으로 설정합니다. 백엔드 API에 Amazon API
Gateway 및 AWS Lambda 함수를 사용합니다. Amazon DynamoDB에 데이터를 저장합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q290
빠르게 성장하는 전자상거래 회사는 단일 AWS 리전에서 워크로드를 실행하고 있습니다. 솔루션 설계자는 다른 AWS 리전을 포함하는 재해 복구(DR) 전략을 생성해야 합니다. 회사는 대기 시간을 최소화하면서 DR 지역에서 데이터베이스를 최신 상태로 유지하기를 원합니다. DR 지역의 나머지 인프라는 감소된 용량으로 실행되어야 하며 필요한 경우 확장할 수 있어야 합니다. 가장 낮은 RTO(복구 시간 목표)로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 파일럿 라이트 배포와 함께 Amazon Aurora 글로벌 데이터베이스를 사용합니다. 
B. 웜 대기 배포와 함께 Amazon Aurora 글로벌 데이터베이스를 사용합니다. 
C. 파일럿 라이트 배포와 함께 Amazon RDS 다중 AZ DB 인스턴스를 사용합니다. 
D. 웜 대기 배포와 함께 Amazon RDS 다중 AZ DB 인스턴스를 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q291
로펌은 대중과 정보를 공유해야 합니다. 이 정보에는 공개적으로 읽을 수 있어야 하는 수백 개의 파일이 포함됩니다. 지정된 미래 날짜 이전에 누구든지 파일을 수정하거나 삭제하는 것은 금지 됩니다. 가장 안전한 방식으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 정적 웹 사이트 호스팅용으로 구성된 Amazon S3 버킷에 모든 파리를 업로드합니다. 지정된 날짜까지 S3 버킷에 액세스하는 모든 AWS 보안 주체에게 읽기 전용 IAM 권한을 부여합
니다.
B. S3 버전 관리가 활성화된 새 Amazon S3 버킷을 생성합니다. 지정된 날짜에 따라 보존 기간이 있는 S3 Object Lock을 사용하십시오. 정적 웹 사이트 호스팅을 위해 S3 버킷을 구성
합니다. 객체에 대한 읽기 전용 액세스를 허용하도록 S3 버킷 정책을 설정합니다.
C. S3 버전 관리가 활성화된 새 Amazon S3 버킷을 생성합니다. 객체 수정 또는 삭제 시 AWS Lambda 함수를 실행하도록 이벤트 트리거를 구성합니다. 개체를 프라이빗 S3 버킷의 원
래 버전으로 바꾸도록 Lambda 함수를 구성합니다.
D. 정적 웹 사이트 호스팅용으로 구성된 Amazon S3 버킷에 모든 파일을 업로드합니다. 파일이 포함된 폴더를 선택합니다. 지정된 날짜에 따라 보존 기간이 있는 S3 Object Lock을 사용
하십시오. S3 버킷에 액세스하는 모든 AWS 보안 주체에게 읽기 전용 IAM 권한을 부여합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q292
한 회사에서 Amazon Route 53 지연 시간 기반 라우팅을 사용하여 전 세계 사용자를 위해 UDP 기반 애플리케이션으로 요청을 라우팅하고 있습니다. 이 애플리케이션은 미국, 아시아 및 유 럽에 있는 회사의 온프레미스 데이터 센터에 있는 중복 서버에서 호스팅됩니다. 회사의 규정 준수 요구 사항에 따르면 애플리케이션은 온프레미스에서 호스팅되어야 합니다. 회사는 애플리케이 션의 성능과 가용성을 개선하고자 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 3개의 AWS 리전에서 3개의 NLB(Network Load Balancer)를 구성하여 온프레미스 엔드포인트를 처리합니다. AWS Global Accelerator를 사용하여 가속기를 생성하고 NLB를
엔드포인트로 등록합니다. 가속기 DNS를 가리키는 CNAME을 사용하여 애플리케이션에 대한 액세스를 제공합니다.
B. 3개의 AWS 리전에서 3개의 Application Load Balancer(ALB)를 구성하여 온프레미스 엔드포인트를 처리합니다. AWS Global Accelerator를 사용하여 가속기를 생성하고 ALB
를 엔드포인트로 등록합니다. 가속기 DNS를 가리키는 CNAME을 사용하여 애플리케이션에 대한 액세스를 제공합니다.
C. 3개의 AWS 리전에서 3개의 NLB(Network Load Balancer)를 구성하여 온프레미스 엔드포인트를 처리합니다. Route 53에서 3개의 NLB를 가리키는 지연 시간 기반 레코드를 생
성하고 이를 Amazon CloudFront 배포의 오리진으로 사용합니다. CloudFront DNS를 가리키는 CNAME을 사용하여 애플리케이션에 대한 액세스를 제공합니다.
D. 온프레미스 엔드포인트를 처리하기 위해 3개의 AWS 리전에서 3개의 ALB(Application Load Balancer)를 구성합니다. Route 53에서 3개의 ALB를 가리키는 지연 시간 기반 레코
드를 생성하고 이를 Amazon CloudFront 배포의 오리진으로 사용합니다. CloudFront DNS를 가리키는 CNAME을 사용하여 애플리케이션에 대한 액세스를 제공합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q293
회사는 사용자 요청을 수집하고 요청 유형에 따라 처리를 위해 적절한 마이크로 서비스에 요청을 발송하는 데 사용되는 비동기 API를 소유하고 있습니다. 이 회사는 Amazon API Gateway 를 사용하여 API 프런트 엔드를 배포하고 Amazon DynamoDB를 호출하여 사용자 요청을 처리 마이크로서비스로 보내기 전에 저장하는 AWS Lambda 함수를 사용하고 있습니다. 회사는 예산이 허용하는 한 많은 DynamoDB 처리량을 프로비저닝했지만 회사는 여전히 가용성 문제를 겪고 있으며 사용자 요청이 손실되고 있습니다. 솔루션 설계자는 기존 사용자에게 영향을 주지 않고 이 문제를 해결하기 위해 무엇을 해야 합니까?
A. API 게이트웨이에서 서버 측 조절 제한을 사용하여 조절을 추가합니다. 
B. DynamoDB Accelerator(DAX) 및 Lambda를 사용하여 DynamoDB에 대한 쓰기를 버퍼링합니다. 
C. 사용자 요청이 있는 테이블에 대해 DynamoDB에서 보조 인덱스를 생성합니다. 
D. Amazon Simple Queue Service(Amazon SQS) 대기열과 Lambda를 사용하여 DynamoDB에 대한 쓰기를 버퍼링합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q294
애플리케이션은 VPC A에 탄력적 IP 주소가 있는 Amazon EC2 인스턴스에서 실행됩니다. 애플리케이션은 VPC B의 데이터베이스에 액세스해야 합니다. 두 VPC 모두 동일한 AWS 계 정에 있습니다. 필요한 액세스를 가장 안전하게 제공하는 솔루션은 무엇입니까?
A. VPC A에 있는 애플리케이션 서버의 퍼블릭 IP 주소에서 오는 모든 트래픽을 허용하는 DB 인스턴스 보안 그룹을 생성합니다. 
B. VPC A와 VPC B 사이에 VPC 피어링 연결을 구성합니다. 
C. DB 인스턴스를 공개적으로 액세스할 수 있도록 합니다. 퍼블릭 IP 주소를 DB 인스턴스에 할당합니다. 
D. 탄력적 IP 주소가 있는 EC2 인스턴스를 VPC B로 시작합니다. 새 EC2 인스턴스를 통해 모든 요청을 프록시합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q295
그룹에는 Amazon S3 버킷을 나열하고 해당 버킷에서 객체를 삭제할 수 있는 권한이 필요합니다. 관리자는 버킷에 대한 액세스 권한을 제공하기 위해 다음 IAM 정책을 생성하고 해당 정책 을 그룹에 적용했습니다. 그룹은 버킷의 객체를 삭제할 수 없습니다. 회사는 최소 권한 액세스 규칙을 따릅니다. 버킷 액세스를 수정하기 위해 솔루션 설계자가 정책에 추가해야 하는 설명은 무엇입니까?
A.
B.
C.
D.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q296
한 회사가 최근 글로벌 전자 상거래 애플리케이션을 위한 데이터 저장소로 Amazon Aurora를 사용하기 시작했습니다. 대규모 보고서가 실행될 때 개발자는 전자 상거래 애플리케이션이 제대 로 작동하지 않는다고 보고합니다. 솔루션 설계자는 Amazon CloudWatch에서 지표를 검토한 후 월별 보고서를 실행할 때 ReadIOPS 및 CPUUtilizalion 지표가 급증하고 있음을 발견 했습니다. 가장 비용 효율적인 솔루션은 무엇입니까?
A. 월별 보고를 Amazon Redshift로 마이그레이션합니다. 
B. 월간 보고를 Aurora 복제본으로 마이그레이션합니다. 
C. Aurora 데이터베이스를 더 큰 인스턴스 클래스로 마이그레이션합니다. 
D. Aurora 인스턴스에서 프로비저닝된 IOPS를 늘립니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q297
회사는 타사 데이터 피드와 통합해야 합니다. 데이터 피드는 웹후크를 보내 새 데이터를 사용할 준비가 되면 외부 서비스에 알립니다. 개발자는 회사에서 웹후크 콜백을 수신할 때 데이터를 검 색하는 AWS Lambda 함수를 작성했습니다. 개발자는 제3자가 호출할 수 있도록 Lambda 함수를 제공해야 합니다. 이러한 요구 사항을 가장 효율적으로 충족하는 솔루션은 무엇입니까?
A. Lambda 함수에 대한 함수 URL을 생성합니다. Webhook에 대한 Lambda 함수 URL을 타사에 제공합니다. 
B. Lambda 함수 앞에 ALB(Application Load Balancer)를 배포합니다. Webhook에 대한 ALB URL을 타사에 제공합니다. 
C. Amazon Simple Notification Service(Amazon SNS) 주제를 생성합니다. Lambda 함수에 주제를 연결합니다. Webhook에 대한 제3자에게 SNS 주제의 공개 호스트 이름을
제공합니다.
D. Amazon Simple Queue Service(Amazon SQS) 대기열을 생성합니다. 대기열을 Lambda 함수에 연결합니다. Webhook에 대해 타사에 SQS 대기열의 공개 호스트 이름을 제
공합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q298
회사에는 Management 및 Production이라는 두 개의 VPC가 있습니다. 관리 VPC는 고객 게이트웨이를 통해 VPN을 사용하여 데이터 센터의 단일 디바이스에 연결합니다. 프로덕션 VPC는 2개의 연결된 AWS Direct Connect 연결이 있는 가상 프라이빗 게이트웨이를 사용합니다. 관리 및 프로덕션 VPC는 모두 단일 VPC 피어링 연결을 사용하여 애플리케이션 간의 통신을 허용합니다. 솔루션 아키텍트는 이 아키텍처에서 단일 실패 지점을 완화하기 위해 무엇을 해야 합니까?
A. 관리 VPC와 프로덕션 VPC 사이에 VPN 세트를 추가하십시오. 
B. 두 번째 가상 프라이빗 게이트웨이를 추가하고 관리 VPC에 연결합니다. 
C. 두 번째 고객 게이트웨이 디바이스에서 관리 VPC에 두 번째 VPN 세트를 추가합니다. 
D. 관리 VPC와 프로덕션 VPC 간에 두 번째 VPC 피어링 연결을 추가합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q299
회사는 데이터 센터의 NAS(Network Attached Storage)에 700TB의 백업 데이터를 저장하고 있습니다. 이 백업 데이터는 드문 규제 요청을 위해 액세스할 수 있어야 하며 7년 동안 보관 해야 합니다. 회사는 이 백업 데이터를 데이터 센터에서 AWS로 마이그레이션하기로 결정했습니다. 마이그레이션은 1개월 이내에 완료되어야 합니다. 회사는 데이터 전송에 사용할 수 있는 공 용 인터넷 연결에 500Mbps의 전용 대역폭을 가지고 있습니다. 최저 비용으로 데이터를 마이그레이션하고 저장하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 데이터를 전송할 AWS Snowball 디바이스를 주문합니다. 수명 주기 정책을 사용하여 파일을 Amazon S3 Glacier Deep Archive로 전환합니다. 
B. 데이터 센터와 Amazon VPC 간에 VPN 연결을 배포합니다. AWS CLI를 사용하여 온프레미스에서 Amazon S3 Glacier로 데이터를 복사합니다. 
C. 500Mbps AWS Direct Connect 연결을 프로비저닝하고 데이터를 Amazon S3로 전송합니다. 수명 주기 정책을 사용하여 파일을 Amazon S3 Glacier Deep Archive로 전환합
니다.
D. AWS DataSync를 사용하여 데이터를 전송하고 온프레미스에 DataSync 에이전트를 배포합니다. DataSync 작업을 사용하여 온프레미스 NAS 스토리지에서 Amazon S3
Glacier로 파일을 복사합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q300
회사에는 다양한 AWS 리전의 여러 AWS 계정에 분산된 프로덕션 워크로드가 있습니다. 이 회사는 AWS Cost Explorer를 사용하여 비용과 사용량을 지속적으로 모니터링합니다. 회사는 워크로드의 비용 및 사용 지출이 비정상적일 때 알림을 받기를 원합니다. 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (2개 선택)
A. 프로덕션 워크로드가 실행 중인 AWS 계정에서 AWS Cost Management 콘솔의 Cost Explorer를 사용하여 연결된 계정 예산을 생성합니다. 
B. 프로덕션 워크로드가 실행 중인 AWS 계정에서 AWS Cost Management 콘솔의 AWS Cost Anomaly Detection을 사용하여 연결된 계정 모니터를 생성합니다. 
C. 프로덕션 워크로드가 실행 중인 AWS 계정에서 AWS 비용 관리 콘솔의 비용 이상 탐지를 사용하여 비용 및 사용 보고서를 생성합니다. 
D. 보고서를 작성하고 이메일 메시지를 보내 매주 회사에 알립니다.
E. 필요한 임계값으로 구독을 생성하고 주간 요약을 사용하여 회사에 알립니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q301
애플리케이션은 여러 가용 영역의 Amazon EC2 인스턴스에서 실행됩니다. 인스턴스는 Application Load Balancer 뒤의 Amazon EC2 Auto Scaling 그룹에서 실행됩니다. 애플리 케이션은 EC2 인스턴스의 CPU 사용률이 40% 또는 거의 40%일 때 최상의 성능을 발휘합니다. 솔루션 설계자는 그룹의 모든 인스턴스에서 원하는 성능을 유지하기 위해 무엇을 해야 합니까?
A. 간단한 조정 정책을 사용하여 Auto Scaling 그룹을 동적으로 조정하십시오. 
B. 대상 추적 정책을 사용하여 Auto Scaling 그룹을 동적으로 확장합니다. 
C. AWS Lambda 함수를 사용하여 원하는 Auto Scaling 그룹 용량을 업데이트합니다. 
D. 예약된 조정 작업을 사용하여 Auto Scaling 그룹을 확장 및 축소합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q302
빠르게 성장하는 글로벌 전자상거래 회사는 AWS에서 웹 애플리케이션을 호스팅하고 있습니다. 웹 애플리케이션에는 정적 콘텐츠와 동적 콘텐츠가 포함됩니다. 웹사이트는 Amazon RDS 데이터베이스에 OLTP(온라인 트랜잭션 처리) 데이터를 저장합니다. 웹사이트 사용자의 페이지 로드 속도가 느려지고 있습니다. 이 문제를 해결하기 위해 솔루션 아키텍트가 취해야 할 조치 조합은 무엇입니까? (두 가지를 선택하세요.)
A. Amazon Redshift 클러스터를 구성합니다. 
B. Amazon CloudFront 배포를 설정합니다. 
C. Amazon S3에서 동적 웹 콘텐츠를 호스팅합니다. 
D. RDS DB 인스턴스에 대한 읽기 전용 복제본을 생성합니다. 
E. RDS DB 인스턴스에 대한 다중 AZ 배포를 구성합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q303
회사에 고객 주문을 처리하는 애플리케이션이 있습니다. 회사는 주문을 Amazon Aurora 데이터베이스에 저장하는 Amazon EC2 인스턴스에서 애플리케이션을 호스팅합니다 . 때때로 트래픽이 많을 때 워크로드가 주문을 충분히 빠르게 처리하지 못합니다. 가능한 한 빨리 데이터베이스에 주문을 안정적으로 기록하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 트래픽이 많을 때 EC2 인스턴스의 인스턴스 크기를 늘립니다. Amazon Simple Notification Service(Amazon SNS)에 주문을 작성합니다. SNS 주제에 데이터베이스 엔드포인
트를 구독합니다.
B. Amazon Simple Queue Service(Amazon SQS) 대기열에 주문을 씁니다. Application Load Balancer 뒤의 Auto Scaling 그룹에서 EC2 인스턴스를 사용하여 SQS 대기
열에서 읽고 주문을 데이터베이스로 처리합니다.
C. Amazon Simple Notification Service(Amazon SNS)에 주문을 작성합니다. SNS 주제에 데이터베이스 엔드포인트를 구독합니다. Application Load Balancer 뒤의 Auto
Scaling 그룹에서 EC2 인스턴스를 사용하여 SNS 주제에서 읽습니다.
D. EC2 인스턴스가 CPU 임계값 제한에 도달하면 Amazon Simple Queue Service(Amazon SQS) 대기열에 주문을 씁니다. Application Load Balancer 뒤의 Auto Scaling
그룹에서 EC2 인스턴스의 예약된 조정을 사용하여 SQS 대기열에서 읽고 데이터베이스로 주문을 처리합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q304
한 회사가 온프레미스 데이터 센터에서 AWS로 상용 기성 애플리케이션을 마이그레이션할 계획입니다. 이 소프트웨어에는 용량 및 가동 시간 요구 사항을 예측할 수 있는 소켓과 코어를 사용 하는 소프트웨어 라이센스 모델이 있습니다. 회사는 올해 초에 구입한 기존 라이센스를 사용하려고 합니다. 가장 비용 효율적인 Amazon EC2 요금 옵션은 무엇입니까?
A. 전용 예약 호스트 
B. 전용 온디맨드 호스트 
C. 전용 예약 인스턴스 
D. 전용 온디맨드 인스턴스

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q305
회사에서 기밀 데이터를 Amazon S3에 저장할 준비를 하고 있습니다. 규정 준수를 위해 데이터는 유휴 상태에서 암호화되어야 합니다. 감사 목적으로 암호화 키 사용을 기록해야 합니다. 키 는 매년 교체해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족하고 운영상 가장 효율적입니까?
A. 고객 제공 키를 사용한 서버 측 암호화(SSE-C) 
B. Amazon S3 관리 키(SSE-S3)를 사용한 서버 측 암호화 
C. 수동 교체가 있는 AWS KMS 키(SSE-KMS)를 사용한 서버 측 암호화 
D. 자동 교체가 있는 AWS KMS 키(SSE-KMS)를 사용한 서버 측 암호화

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q306
게임 회사는 공개 점수판을 데이터 센터에서 AWS 클라우드로 옮기고 있습니다. 이 회사는 Application Load Balancer 뒤에 Amazon EC2 Windows Server 인스턴스를 사용하여 동 적 애플리케이션을 호스팅합니다. 회사는 애플리케이션을 위한 고가용성 스토리지 솔루션이 필요합니다. 애플리케이션은 정적 파일과 동적 서버 측 코드로 구성됩니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. Amazon S3에 정적 파일을 저장합니다. Amazon CloudFront를 사용하여 엣지에서 객체를 캐싱합니다. 
B. 정적 파일을 Amazon S3에 저장합니다. Amazon ElastiCache를 사용하여 엣지에서 객체를 캐싱합니다. 
C. Amazon Elastic File System(Amazon EFS)에 서버 측 코드를 저장합니다. 파일을 공유할 각 EC2 인스턴스에 EFS 볼륨을 탑재합니다. 
D. Windows File Server용 Amazon FSx에 서버 측 코드를 저장합니다. 파일을 공유할 각 EC2 인스턴스에 FSx for Windows File Server 볼륨을 탑재합니다. 
E. 범용 SSD(gp2) Amazon Elastic Block Store(Amazon EBS) 볼륨에 서버 측 코드를 저장합니다. 각 EC2 인스턴스에 EBS 볼륨을 탑재하여 파일을 공유합니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q307
회사가 AWS에서 애플리케이션을 시작하고 있습니다. 애플리케이션은 Application Load Balancer(ALB)를 사용하여 단일 대상 그룹에 있는 최소 2개의 Amazon EC2 인스턴스로 트 래픽을 보냅니다. 인스턴스는 각 환경의 Auto Scaling 그룹에 있습니다. 회사는 개발 환경과 생산 환경이 필요합니다. 프로덕션 환경에는 트래픽이 많은 기간이 있습니다. 개발 환경을 가장 비용 효율적으로 구성하는 솔루션은 무엇입니까?
A. 하나의 EC2 인스턴스만 대상으로 하도록 개발 환경에서 대상 그룹을 재구성합니다. 
B. ALB 밸런싱 알고리즘을 최소 미해결 요청으로 변경합니다. 
C. 두 환경 모두에서 EC2 인스턴스의 크기를 줄입니다. 
D. 개발 환경의 Auto Scaling 그룹에서 최대 EC2 인스턴스 수를 줄입니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q308
한 회사에서 온라인 멀티플레이어 게임용 네트워크를 설계하고 있습니다. 이 게임은 UDP 네트워킹 프로토콜을 사용하며 8개의 AWS 리전에 배포됩니다. 네트워크 아키텍처는 최종 사용자에 게 고품질 게임 경험을 제공하기 위해 대기 시간과 패킷 손실을 최소화해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 각 리전에서 전송 게이트웨이를 설정합니다. 각 전송 게이트웨이 간에 리전 간 피어링 연결을 생성합니다. 
B. 각 리전에서 UDP 리스너 및 엔드포인트 그룹으로 AWS Global Accelerator를 설정합니다. 
C. UDP를 켠 상태에서 Amazon CloudFront를 설정합니다. 각 리전에서 오리진을 구성합니다. 
D. 각 지역 간에 VPC 피어링 메시를 설정합니다. 각 VPC에 대해 UDP를 켭니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q309
엔터테인먼트 회사는 Amazon DynamoDB를 사용하여 미디어 메타데이터를 저장하고 있습니다. 애플리케이션이 읽기 집약적이며 지연이 발생합니다. 회사에는 추가 운영 오버헤드를 처리 할 직원이 없으며 애플리케이션을 재구성하지 않고 DynamoDB의 성능 효율성을 개선해야 합니다. 이 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. Redis용 Amazon ElastiCache를 사용합니다. 
B. Amazon DynamoDB Accelerator(DAX)를 사용합니다. 
C. DynamoDB 전역 테이블을 사용하여 데이터를 복제합니다. 
D. 자동 검색이 활성화된 Memcached용 Amazon ElastiCache를 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q310
회사는 대규모 Amazon EC2 인스턴스 플릿에서 애플리케이션을 실행합니다. 애플리케이션은 항목을 읽고 Amazon DynamoDB 테이블에 씁니다. DynamoDB 테이블의 크기는 지속적 으로 증가하지만 애플리케이션에는 지난 30일 동안의 데이터만 필요합니다. 회사는 비용과 개발 노력을 최소화하는 솔루션이 필요합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS CloudFormation 템플릿을 사용하여 전체 솔루션을 배포합니다. 30일마다 CloudFormation 스택을 재배포하고 원래 스택을 삭제합니다. 
B. AWS Marketplace에서 모니터링 애플리케이션을 실행하는 EC2 인스턴스를 사용합니다. Amazon DynamoDB Streams를 사용하여 테이블에 새 항목이 생성될 때 타임스탬프를
저장하도록 모니터링 애플리케이션을 구성합니다. EC2 인스턴스에서 실행되는 스크립트를 사용하여 30일보다 오래된 타임스탬프가 있는 항목을 삭제합니다.
C. 테이블에 새 항목이 생성될 때 AWS Lambda 함수를 호출하도록 Amazon DynamoDB Streams를 구성합니다. 테이블에서 30일보다 오래된 항목을 삭제하도록 Lambda 함수를
구성합니다.
D. 애플리케이션을 확장하여 현재 타임스탬프에 30일을 더한 값을 테이블에 생성된 각 새 항목에 추가하는 속성을 추가합니다. 속성을 TTL 속성으로 사용하도록 DynamoDB를 구성합니다
.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q311
회사는 Amazon EC2 인스턴스에서 실행되는 지연 시간에 민감한 애플리케이션을 위해 인 메모리 데이터베이스를 실행하려고 합니다. 애플리케이션은 분당 100,000개 이상의 트랜잭션을 처리하며 높은 네트워크 처리량이 필요합니다. 솔루션 설계자는 데이터 전송 비용을 최소화하는 비용 효율적인 네트워크 설계를 제공해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 동일한 AWS 리전 내의 동일한 가용 영역에서 모든 EC2 인스턴스를 시작합니다. EC2 인스턴스를 시작할 때 클러스터 전략으로 배치 그룹을 지정합니다. 
B. 동일한 AWS 지역 내의 다른 가용 영역에서 모든 EC2 인스턴스를 시작합니다. EC2 인스턴스를 시작할 때 파티션 전략으로 배치 그룹을 지정합니다. 
C. Auto Scaling 그룹을 배포하여 네트워크 활용 목표에 따라 다른 가용 영역에서 EC2 인스턴스를 시작합니다. 
D. 서로 다른 가용 영역에서 EC2 인스턴스를 시작하기 위해 단계 조정 정책으로 Auto Scaling 그룹을 배포합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q312
회사는 오래된 뉴스 영상에서 AWS에 비디오 아카이브를 저장할 수 있는 솔루션을 찾고 있습니다. 회사는 비용을 최소화해야 하며 이러한 파일을 복원할 필요가 거의 없습니다. 파일이 필요할 때 최대 5분 내에 사용할 수 있어야 합니다. 가장 비용 효율적인 솔루션은 무엇입니까?
A. 비디오 아카이브를 Amazon S3 Glacier에 저장하고 긴급 검색을 사용합니다. 
B. 비디오 아카이브를 Amazon S3 Glacier에 저장하고 표준 검색을 사용합니다. 
C. 비디오 아카이브를 Amazon S3 Standard-Infrequent Access(S3 Standard-IA)에 저장합니다. 
D. 비디오 아카이브를 Amazon S3 One Zone-Infrequent Access(S3 One Zone-IA)에 저장합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q313
회사에는 여러 모니터링 장치에서 실시간 데이터를 수신하는 API가 있습니다. API는 나중에 분석할 수 있도록 이 데이터를 Amazon RDS DB 인스턴스에 저장합니다. 모니터링 장치가 API로 보내는 데이터의 양은 변동합니다. 트래픽이 많은 기간 동안 API는 종종 시간 초과 오류를 반환합니다. 로그를 검사한 후 회사는 데이터베이스가 API에서 오는 쓰기 트래픽 볼륨을 처리할 수 없음을 확인합니다. 솔루션 설계자는 데이터베이스에 대한 연결 수를 최소화하고 트래픽이 많은 기간 동 안 데이터가 손실되지 않도록 해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 사용 가능한 메모리가 더 많은 인스턴스 유형으로 DB 인스턴스의 크기를 늘리십시오. 
B. DB 인스턴스를 다중 AZ DB 인스턴스로 수정합니다. 모든 활성 RDS DB 인스턴스에 쓰도록 애플리케이션을 구성합니다. 
C. 수신 데이터를 Amazon Simple Queue Service(Amazon SQS) 대기열에 쓰도록 API를 수정합니다. Amazon SQS가 호출하는 AWS Lambda 함수를 사용하여 대기열에서
데이터베이스로 데이터를 씁니다.
D. 수신 데이터를 Amazon Simple Notification Service(Amazon SNS) 주제에 쓰도록 API를 수정합니다. Amazon SNS가 호출하는 AWS Lambda 함수를 사용하여 주제에서
데이터베이스로 데이터를 씁니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q314
회사에서 온프레미스 데이터 센터를 AWS로 마이그레이션하려고 합니다. 회사의 규정 준수 요구 사항에 따라 회사는 ap-northeast-3 리전만 사용할 수 있습니다. 회사 관리자는 VPC를 인 터넷에 연결할 수 없습니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까? (두 가지를 선택하세요.)
A. AWS Control Tower를 사용하여 데이터 레지던시 가드레일을 구현하여 인터넷 액세스를 거부하고 ap-northeast-3을 제외한 모든 AWS 리전에 대한 액세스를 거부합니다. 
B. AWS WAF의 규칙을 사용하여 인터넷 액세스를 방지합니다. AWS 계정 설정에서 ap-northeast-3을 제외한 모든 AWS 지역에 대한 액세스를 거부합니다. 
C. AWS Organizations를 사용하여 VPC가 인터넷에 액세스하지 못하도록 하는 SCPS(서비스 제어 정책)를 구성합니다. ap-northeast-3을 제외한 모든 AWS 리전에 대한 액세스를
거부합니다.
D. 각 VPC의 네트워크 ACL에 대한 아웃바운드 규칙을 생성하여 0.0.0.0/0의 모든 트래픽을 거부합니다. 각 사용자에 대한 IAM 정책을 생성하여 ap-northeast-3 이외의 AWS 리전 사
용을 방지합니다.
E. AWS Config를 사용하여 관리형 규칙을 활성화하여 인터넷 게이트웨이를 감지 및 경고하고 ap-northeast-3 외부에 배포된 새 리소스를 감지 및 경고합니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q315
회사는 AWS 클라우드의 컨테이너에서 애플리케이션을 실행하려고 합니다. 이러한 애플리케이션은 상태 비저장이며 기본 인프라 내의 중단을 허용할 수 있습니다. 회사는 비용과 운영 오버헤 드를 최소화하는 솔루션이 필요합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Amazon EC2 Auto Scaling 그룹의 스팟 인스턴스를 사용하여 애플리케이션 컨테이너를 실행합니다. 
B. Amazon Elastic Kubernetes Service(Amazon EKS) 관리형 노드 그룹에서 스팟 인스턴스를 사용합니다. 
C. Amazon EC2 Auto Scaling 그룹에서 온디맨드 인스턴스를 사용하여 애플리케이션 컨테이너를 실행합니다. 
D. Amazon Elastic Kubernetes Service(Amazon EKS) 관리형 노드 그룹에서 온디맨드 인스턴스를 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q316
한 회사가 최근 메시지 처리 시스템을 AWS로 마이그레이션했습니다. 시스템은 Amazon EC2 인스턴스에서 실행되는 ActiveMQ 대기열로 메시지를 수신합니다. 메시지는 Amazon EC2에서 실행되는 소비자 애플리케이션에 의해 처리됩니다. 소비자 애플리케이션은 메시지를 처리하고 결과를 Amazon EC2에서 실행되는 MySQL 데이터베이스에 기록합니다. 회사는 이 애플리케이션이 운영 복잡성이 낮으면서 가용성이 높기를 원합니다. 가장 높은 가용성을 제공하는 아키텍처는 무엇입니까?
A. 다른 가용 영역에 두 번째 ActiveMQ 서버를 추가합니다. 다른 가용 영역에 추가 소비자 EC2 인스턴스를 추가합니다. MySQL 데이터베이스를 다른 가용 영역에 복제합니다. 
B. 두 가용 영역에 걸쳐 구성된 활성/대기 브로커와 함께 Amazon MQ를 사용합니다. 다른 가용 영역에 추가 소비자 EC2 인스턴스를 추가합니다. MySQL 데이터베이스를 다른 가용 영역
에 복제합니다.
C. 두 가용 영역에 걸쳐 구성된 활성/대기 브로커와 함께 Amazon MQ를 사용합니다. 다른 가용 영역에 추가 소비자 EC2 인스턴스를 추가합니다. 다중 AZ가 활성화된 MySQL용
Amazon RDS를 사용합니다.
D. 두 가용 영역에 걸쳐 구성된 활성/대기 브로커와 함께 Amazon MQ를 사용합니다. 두 가용 영역에서 소비자 EC2 인스턴스에 대한 Auto Scaling 그룹을 추가합니다. 다중 AZ가 활성
화된 MySQL용 Amazon RDS를 사용합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q317
회사는 AWS 계정의 모든 애플리케이션에서 Amazon EC2 Auto Scaling 이벤트를 보고하는 솔루션을 구축하고 있습니다. 회사는 Amazon S3에 EC2 Auto Scaling 상태 데이터를 저장하기 위해 서버리스 솔루션을 사용해야 합니다. 그런 다음 회사는 Amazon S3의 데이터를 사용하여 대시보드에서 거의 실시간 업데이트를 제공합니다. 솔루션은 EC2 인스턴스 시작 속 도에 영향을 미치지 않아야 합니다. 회사는 이러한 요구 사항을 충족하기 위해 어떻게 데이터를 Amazon S3로 이동해야 합니까?
A. Amazon CloudWatch 지표 스트림을 사용하여 EC2 Auto Scaling 상태 데이터를 Amazon Kinesis Data Firehose로 보냅니다. 데이터를 Amazon S3에 저장합니다. 
B. Amazon EMR 클러스터를 시작하여 EC2 Auto Scaling 상태 데이터를 수집하고 데이터를 Amazon Kinesis Data Firehose로 보냅니다. 데이터를 Amazon S3에 저장합니다. 
C. Amazon EventBridge 규칙을 생성하여 일정에 따라 AWS Lambda 함수를 호출합니다. EC2 Auto Scaling 상태 데이터를 Amazon S3로 직접 보내도록 Lambda 함수를 구성
합니다.
D. EC2 인스턴스를 시작하는 동안 부트스트랩 스크립트를 사용하여 Amazon Kinesis 에이전트를 설치합니다. EC2 Auto Scaling 상태 데이터를 수집하고 데이터를 Amazon
Kinesis Data Firehose로 보내도록 Kinesis 에이전트를 구성합니다. 데이터를 Amazon S3에 저장합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q318
한 회사가 AWS에 새로운 공개 웹 애플리케이션을 배포하고 있습니다. 애플리케이션은 ALB(Application Load Balancer) 뒤에서 실행됩니다. 애플리케이션은 외부 CA(인증 기관)에서 발급한 SSL/TLS 인증서를 사용하여 에지에서 암호화해야 합니다. 인증서는 매년 만료되기 전에 교체되어야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. ACM(AWS Certificate Manager)을 사용하여 SSL/TLS 인증서를 발급하세요. ALB에 인증서를 적용합니다. 관리형 갱신 기능을 사용하여 인증서를 자동으로 교체하세요. 
B. ACM(AWS Certificate Manager)을 사용하여 SSL/TLS 인증서를 가져옵니다. ALB에 인증서를 적용합니다. 인증서 만료가 가까워지면 Amazon EventBridge(Amazon
CloudWatch Events)를 사용하여 알림을 보냅니다. 인증서를 수동으로 순환합니다.
C. AWS Certificate Manager(ACM)을 사용하여 SSL/TLS 인증서를 발급합니다. 인증서에서 키 자료를 가져옵니다. AL에 인증서 적용 관리형 갱신 기능을 사용하여 인증서를 자동으
로 교체합니다.
D. AWS 사설 인증 기관을 사용하여 루트 CA에서 SSL/TLS 인증서를 발급합니다. ALB에 인증서를 적용합니다. 관리형 갱신 기능을 사용하여 인증서를 자동으로 교체하세요.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q319
회사는 특정 지불 ID에 대한 메시지가 전송된 순서대로 수신되어야 하는 지불 처리 시스템을 사용합니다. 그렇지 않으면 결제가 잘못 처리될 수 있습니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 어떤 조치를 취해야 합니까? (두 가지를 선택하세요.)
A. 결제 ID를 파티션 키로 사용하여 Amazon DynamoDB 테이블에 메시지를 씁니다. 
B. 결제 ID를 파티션 키로 사용하여 Amazon Kinesis 데이터 스트림에 메시지를 씁니다. 
C. 결제 ID를 키로 사용하여 Amazon ElastiCache for Memcached 클러스터에 메시지를 씁니다. 
D. Amazon Simple Queue Service(Amazon SQS) 대기열에 메시지를 씁니다. 결제 ID를 사용하도록 메시지 속성을 설정합니다. 
E. Amazon Simple Queue Service(Amazon SQS) FIFO 대기열에 메시지를 씁니다. 결제 ID를 사용할 메시지 그룹을 설정합니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q320
금융 회사는 AWS에서 웹 애플리케이션을 호스팅합니다. 이 애플리케이션은 Amazon API Gateway 지역 API 엔드포인트를 사용하여 사용자에게 현재 주가를 검색할 수 있는 기능을 제공 합니다. 회사의 보안 팀은 API 요청 수가 증가한 것을 발견했습니다. 보안 팀은 HTTP 플러드 공격이 애플리케이션을 오프라인 상태로 만들 수 있다고 우려하고 있습니다. 솔루션 설계자는 이러한 유형의 공격으로부터 애플리케이션을 보호하기 위한 솔루션을 설계해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 최대 TTL이 24시간인 API Gateway 지역 API 엔드포인트 앞에 Amazon CloudFront 배포를 생성합니다. 
B. 속도 기반 규칙을 사용하여 리전 AWS WAF 웹 ACL을 생성합니다. 웹 ACL을 API Gateway 단계와 연결합니다. 
C. Amazon CloudWatch 지표를 사용하여 개수 지표를 모니터링하고 미리 정의된 속도에 도달하면 보안 팀에 알립니다. 
D. API Gateway 지역 API 엔드포인트 앞에 Lambda@Edge를 사용하여 Amazon CloudFront 배포를 생성합니다 . 사전 정의된 속도를 초과하는 IP 주소의 요청을 차단하는 AWS
Lambda 함수를 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q321
회사에서 AWS 인프라에 대한 월별 유지 관리를 수행합니다. 이러한 유지 관리 활동 중에 회사는 여러 AWS 리전에서 Amazon RDS for MySQL 데이터베이스에 대한 자격 증명을 교체 해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 자격 증명을 AWS Secrets Manager에 비밀로 저장합니다. 필요한 리전에 대해 다중 리전 비밀 복제를 사용합니다. 일정에 따라 비밀을 교체하도록 Secrets Manager를 구성합니다
.
B. 보안 문자열 파라미터를 생성하여 AWS Systems Manager에 자격 증명을 비밀로 저장합니다. 필요한 리전에 대해 다중 리전 비밀 복제를 사용합니다. 일정에 따라 암호를 교체하도록
Systems Manager를 구성합니다.
C. 서버 측 암호화(SSE)가 활성화된 Amazon S3 버킷에 자격 증명을 저장합니다. Amazon EventBridge(Amazon CloudWatch Events)를 사용하여 AWS Lambda 함수를 호
출하여 자격 증명을 교체합니다.
D. AWS Key Management Service(AWS KMS) 다중 리전 고객 관리 키를 사용하여 자격 증명을 비밀로 암호화합니다. Amazon DynamoDB 전역 테이블에 암호를 저장합니다.
AWS Lambda 함수를 사용하여 DynamoDB에서 비밀을 검색합니다. RDS API를 사용하여 암호를 교체합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q322
회사에서 주요 웹 애플리케이션 중 하나의 콘텐츠에 대한 액세스를 제한하고 AWS에서 사용할 수 있는 권한 부여 기술을 사용하여 콘텐츠를 보호하려고 합니다. 이 회사는 서버리스 아키텍처 와 100명 미만의 사용자를 위한 인증 솔루션을 구현하려고 합니다. 솔루션은 기본 웹 애플리케이션과 통합하고 웹 콘텐츠를 전역적으로 제공해야 합니다. 솔루션은 또한 회사의 사용자 기반이 성장함에 따라 확장되어야 하며 가능한 한 가장 낮은 로그인 대기 시간을 제공해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 인증에 Amazon Cognito를 사용하십시오. 인증을 위해 Lambda@Edge를 사용합니다 . Amazon CloudFront를 사용하여 전 세계적으로 웹 애플리케이션을 제공합니다. 
B. 인증을 위해 Microsoft Active Directory용 AWS Directory Service를 사용합니다. 승인을 위해 AWS Lambda를 사용합니다. Application Load Balancer를 사용하여 웹 애
플리케이션을 전역적으로 제공합니다.
C. 인증에 Amazon Cognito를 사용합니다. 승인을 위해 AWS Lambda를 사용합니다. Amazon S3 Transfer Acceleration을 사용하여 전 세계적으로 웹 애플리케이션을 제공합니
다.
D. 인증을 위해 Microsoft Active Directory용 AWS Directory Service를 사용합니다. 인증을 위해 Lambda@Edge를 사용합니다 . AWS Elastic Beanstalk를 사용하여 전 세계
적으로 웹 애플리케이션을 제공합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q323
한 회사에서 여러 가용 영역의 Amazon EC2 인스턴스에서 실행되는 웹 기반 애플리케이션을 구축하고 있습니다. 웹 애플리케이션은 총 약 900TB 크기의 텍스트 문서 저장소에 대한 액세 스를 제공합니다. 회사는 웹 애플리케이션이 높은 수요 기간을 경험할 것으로 예상합니다. 솔루션 설계자는 텍스트 문서의 저장소 구성 요소가 항상 응용 프로그램의 요구 사항을 충족하도록 확 장할 수 있는지 확인해야 합니다. 회사는 솔루션의 전체 비용에 대해 우려하고 있습니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 스토리지 솔루션은 무엇입니까?
A. Amazon Elastic Block Store(Amazon EBS) 
B. Amazon Elastic File System(Amazon EFS) 
C. Amazon OpenSearch 서비스(Amazon Elasticsearch 서비스) 
D. 아마존 S3

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q324
회사에서 새로운 서버리스 워크로드 배포를 준비하고 있습니다. 솔루션 설계자는 최소 권한 원칙을 사용하여 AWS Lambda 함수를 실행하는 데 사용할 권한을 구성해야 합니다. Amazon EventBridge(Amazon CloudWatch Events) 규칙이 함수를 호출합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. lambda:InvokeFunction을 액션으로, *를 보안 주체로 사용하여 함수에 실행 역할을 추가합니다. 
B. Lambda:InvokeFunction을 작업으로, Service: lambda.amazonaws.com을 보안 주체로 사용하여 함수에 실행 역할을 추가합니다. 
C. Lambda:*를 작업으로, Service: events.amazonaws.com을 보안 주체로 사용하여 함수에 리소스 기반 정책을 추가합니다. 
D. Lambda:InvokeFunction을 작업으로, Service: events.amazonaws.com을 보안 주체로 사용하여 함수에 리소스 기반 정책을 추가합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q325
회사에 Java 및 PHP 기반 웹 애플리케이션이 있습니다. 회사는 애플리케이션을 온프레미스에서 AWS로 옮길 계획입니다. 회사는 새로운 사이트 기능을 자주 테스트할 수 있는 능력이 필요 합니다. 회사는 또한 최소한의 운영 오버헤드를 필요로 하는 가용성이 높고 관리되는 솔루션이 필요합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon S3 버킷을 생성합니다. S3 버킷에서 정적 웹 호스팅을 활성화합니다. 정적 콘텐츠를 S3 버킷에 업로드합니다. AWS Lambda를 사용하여 모든 동적 콘텐츠를 처리합니다. 
B. 웹 애플리케이션을 AWS Elastic Beanstalk 환경에 배포합니다. 기능 테스트를 위해 URL 스와핑을 사용하여 여러 Elastic Beanstalk 환경 간에 전환합니다. 
C. Java 및 PHP로 구성된 Amazon EC2 인스턴스에 웹 애플리케이션을 배포합니다. Auto Scaling 그룹과 Application Load Balancer를 사용하여 웹 사이트의 가용성을 관리하십
시오.
D. 웹 애플리케이션을 컨테이너화합니다. 웹 애플리케이션을 Amazon EC2 인스턴스에 배포합니다. AWS 로드 밸런서 컨트롤러를 사용하여 테스트용 새 사이트 기능이 포함된 컨테이너
간에 트래픽을 동적으로 라우팅합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q326
한 회사에서 us-west-2 리전의 NLB(Network Load Balancer) 뒤에 있는 3개의 Amazon EC2 인스턴스에 자체 관리형 DNS 솔루션을 구현했습니다. 회사 사용자의 대부분은 미국과 유럽에 있습니다. 회사는 솔루션의 성능과 가용성을 개선하고자 합니다. 회사는 eu-west-1 지역에서 3개의 EC2 인스턴스를 시작 및 구성하고 EC2 인스턴스를 새 NLB의 대상으로 추가합 니다. 회사에서 트래픽을 모든 EC2 인스턴스로 라우팅하는 데 사용할 수 있는 솔루션은 무엇입니까?
A. 두 NLB 중 하나로 요청을 라우팅하는 Amazon Route 53 지리적 위치 라우팅 정책을 생성합니다. Amazon CloudFront 배포를 생성합니다. Route 53 레코드를 배포 원본으로 사
용합니다.
B. AWS Global Accelerator에서 표준 가속기를 생성합니다. us-west-2 및 eu-west-1에서 엔드포인트 그룹을 생성합니다. 끝점 그룹의 끝점으로 두 개의 NLB를 추가합니다. 
C. 탄력적 IP 주소를 6개의 EC2 인스턴스에 연결합니다. 6개의 EC2 인스턴스 중 하나로 요청을 라우팅하는 Amazon Route 53 지리적 위치 라우팅 정책을 생성합니다. Amazon
CloudFront 배포를 생성합니다. Route 53 레코드를 배포 원본으로 사용합니다.
D. 두 개의 NLB를 두 개의 ALB(Application Load Balancer)로 교체합니다. 요청을 두 ALB 중 하나로 라우팅하는 Amazon Route 53 지연 시간 라우팅 정책을 생성합니다.
Amazon CloudFront 배포를 생성합니다. Route 53 레코드를 배포 원본으로 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q327
회사는 Amazon EC2 인스턴스에서 실행되는 RESTful 웹 서비스 애플리케이션을 사용하여 수천 개의 원격 장치에서 데이터를 수집합니다. EC2 인스턴스는 원시 데이터를 수신하고 원시 데이터를 변환하며 모든 데이터를 Amazon S3 버킷에 저장합니다. 원격 장치의 수는 곧 수백만 개로 증가할 것입니다. 이 회사는 운영 오버헤드를 최소화하는 확장성이 뛰어난 솔루션이 필요 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. AWS Glue를 사용하여 Amazon S3에서 원시 데이터를 처리합니다. 
B. Amazon Route 53을 사용하여 트래픽을 다른 EC2 인스턴스로 라우팅합니다. 
C. 들어오는 데이터의 양을 수용하기 위해 더 많은 EC2 인스턴스를 추가합니다. 
D. 원시 데이터를 Amazon Simple Queue Service(Amazon SQS)로 보냅니다. EC2 인스턴스를 사용하여 데이터를 처리합니다. 
E. Amazon API Gateway를 사용하여 원시 데이터를 Amazon Kinesis 데이터 스트림으로 보냅니다. 데이터 스트림을 소스로 사용하여 데이터를 Amazon S3에 전달하도록
Amazon Kinesis Data Firehose를 구성합니다.

<details>
<summary>정답 보기</summary>

**AE**
</details>

---

### Q328
회사에 소프트웨어 엔지니어링에 사용되는 AWS 계정이 있습니다. AWS 계정은 한 쌍의 AWS Direct Connect 연결을 통해 회사의 온프레미스 데이터 센터에 액세스할 수 있습니다. 모든 비 VPC 트래픽은 가상 프라이빗 게이트웨이로 라우팅됩니다. 개발팀은 최근 콘솔을 통해 AWS Lambda 함수를 생성했습니다. 개발 팀은 함수가 회사 데이터 센터의 프라이빗 서브넷에서 실행되는 데이터베이스에 액세스할 수 있도록 허용해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 적절한 보안 그룹을 사용하여 VPC에서 실행되도록 Lambda 함수를 구성합니다. 
B. AWS에서 데이터 센터로 VPN 연결을 설정합니다. VPN을 통해 Lambda 함수의 트래픽을 라우팅합니다. 
C. Lambda 함수가 Direct Connect를 통해 온프레미스 데이터 센터에 액세스할 수 있도록 VPC의 라우팅 테이블을 업데이트합니다. 
D. 탄력적 IP 주소를 생성합니다. 탄력적 네트워크 인터페이스 없이 탄력적 IP 주소를 통해 트래픽을 보내도록 Lambda 함수를 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q329
회사는 온프레미스 데이터 센터에서 마케팅 웹 사이트를 호스팅합니다. 웹 사이트는 정적 문서로 구성되며 단일 서버에서 실행됩니다. 관리자는 웹 사이트 콘텐츠를 자주 업데이트하지 않고 SFTP 클라이언트를 사용하여 새 문서를 업로드합니다. 회사는 AWS에서 웹 사이트를 호스팅하고 Amazon CloudFront를 사용하기로 결정했습니다. 회사의 솔루션 아키텍트가 CloudFront 배포를 생성합니다. 솔루션 설계자는 웹 사이트 호스 팅이 CloudFront 오리진 역할을 할 수 있도록 가장 비용 효율적이고 탄력적인 아키텍처를 설계해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Lightsail을 사용하여 가상 서버를 생성합니다. Lightsail 인스턴스에서 웹 서버를 구성합니다. SFTP 클라이언트를 사용하여 웹 사이트 콘텐츠를 업로드합니다. 
B. Amazon EC2 인스턴스에 대한 AWS Auto Scaling 그룹을 생성합니다. Application Load Balancer를 사용하십시오. SFTP 클라이언트를 사용하여 웹 사이트 콘텐츠를 업로드
합니다.
C. 프라이빗 Amazon S3 버킷을 생성합니다. S3 버킷 정책을 사용하여 CloudFront 원본 액세스 ID(OAI)에서 액세스를 허용합니다. AWS CLI를 사용하여 웹사이트 콘텐츠를 업로드합
니다.
D. 퍼블릭 Amazon S3 버킷을 생성합니다. SFTP용 AWS 전송을 구성합니다. 웹 사이트 호스팅을 위해 S3 버킷을 구성합니다. SFTP 클라이언트를 사용하여 웹 사이트 콘텐츠를 업로
드합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q330
회사는 사용자에게 글로벌 속보, 지역 경보 및 날씨 업데이트를 제공하는 웹 기반 포털을 운영합니다. 포털은 정적 및 동적 콘텐츠를 혼합하여 각 사용자에게 개인화된 보기를 제공합니다. 콘텐 츠는 ALB(Application Load Balancer) 뒤의 Amazon EC2 인스턴스에서 실행되는 API 서버를 통해 HTTPS를 통해 제공됩니다. 회사는 포털에서 이 콘텐츠를 전 세계 사용자에게 가 능한 한 빨리 제공하기를 원합니다. 솔루션 설계자는 모든 사용자에게 최소한의 대기 시간을 보장하기 위해 애플리케이션을 어떻게 설계해야 합니까?
A. 단일 AWS 리전에서 애플리케이션 스택을 배포합니다. Amazon CloudFront를 사용하여 ALB를 오리진으로 지정하여 모든 정적 및 동적 콘텐츠를 제공합니다. 
B. 두 AWS 리전에 애플리케이션 스택을 배포합니다. Amazon Route 53 지연 시간 라우팅 정책을 사용하여 가장 가까운 리전에서 ALB의 모든 콘텐츠를 제공합니다. 
C. 단일 AWS 리전에서 애플리케이션 스택을 배포합니다. Amazon CloudFront를 사용하여 정적 콘텐츠를 제공합니다. ALB에서 직접 동적 콘텐츠를 제공합니다. 
D. 두 AWS 리전에 애플리케이션 스택을 배포합니다. Amazon Route 53 지리적 위치 라우팅 정책을 사용하여 가장 가까운 리전에서 ALB의 모든 콘텐츠를 제공합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q331
전자상거래 회사는 분석을 위해 판매 기록을 집계하고 필터링하기 위해 예약된 일일 작업을 실행해야 합니다. 회사는 판매 기록을 Amazon S3 버킷에 저장합니다. 각 개체의 크기는 최대 10GB입니다. 판매 이벤트 수에 따라 작업을 완료하는 데 최대 1시간이 걸릴 수 있습니다. 작업의 CPU 및 메모리 사용량은 일정하며 미리 알려져 있습니다. 솔루션 설계자는 작업을 실행하는 데 필요한 운영 노력을 최소화해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon EventBridge 알림이 있는 AWS Lambda 함수를 생성합니다. EventBridge 이벤트가 하루에 한 번 실행되도록 예약합니다. 
B. AWS Lambda 함수를 생성합니다. Amazon API Gateway HTTP API를 생성하고 API를 함수와 통합합니다. API를 호출하고 함수를 호출하는 Amazon EventBridge 예약 이
벤트를 생성합니다.
C. AWS Fargate 시작 유형으로 Amazon Elastic Container Service(Amazon ECS) 클러스터를 생성합니다. 작업을 실행하기 위해 클러스터에서 ECS 작업을 시작하는
Amazon EventBridge 예약 이벤트를 생성합니다.
D. Amazon EC2 시작 유형이 있는 Amazon Elastic Container Service(Amazon ECS) 클러스터와 하나 이상의 EC2 인스턴스가 있는 Auto Scaling 그룹을 생성합니다. 작업을
실행하기 위해 클러스터에서 ECS 작업을 시작하는 Amazon EventBridge 예약 이벤트를 생성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q332
솔루션 설계자는 모든 신규 사용자가 특정 복잡성 요구 사항과 IAM 사용자 암호에 대한 필수 교체 기간을 갖기를 원합니다. 이를 달성하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. 전체 AWS 계정에 대한 전반적인 암호 정책을 설정합니다. 
B. AWS 계정의 각 IAM 사용자에 대한 암호 정책을 설정합니다. 
C. 타사 공급업체 소프트웨어를 사용하여 암호 요구 사항을 설정합니다. 
D. Amazon CloudWatch 규칙을 Create_newuser 이벤트에 연결하여 적절한 요구 사항으로 암호를 설정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q333
회사에서 온프레미스 서버에서 Amazon EC2 인스턴스로 애플리케이션을 마이그레이션하고 있습니다. 마이그레이션 설계 요구 사항의 일부로 솔루션 설계자는 인프라 지표 경보를 구현해야 합니다. 짧은 시간 동안 CPU 사용률이 50% 이상으로 증가하면 회사에서 조치를 취할 필요가 없습니다. 그러나 CPU 사용률이 50% 이상으로 증가하고 디스크의 읽기 IOPS가 동시에 높은 경우 회사는 가능한 한 빨리 조치를 취해야 합니다. 솔루션 설계자는 또한 잘못된 경보를 줄여야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 가능한 경우 Amazon CloudWatch 복합 경보를 생성합니다. 
B. 지표를 시각화하고 문제에 신속하게 대응하기 위해 Amazon CloudWatch 대시보드를 생성합니다. 
C. Amazon CloudWatch Synthetics 카나리아를 생성하여 애플리케이션을 모니터링하고 경보를 울립니다. 
D. 가능한 경우 여러 지표 임계값이 있는 단일 Amazon CloudWatch 지표 경보를 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q334
회사는 독점 응용 프로그램의 로그 파일을 분석할 수 있는 기능이 필요합니다. 로그는 Amazon S3 버킷에 JSON 형식으로 저장됩니다. 쿼리는 간단하고 주문형으로 실행됩니다. 솔루션 설 계자는 기존 아키텍처를 최소한으로 변경하여 분석을 수행해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하려면 솔루션 설계자가 무엇을 해야 합니까?
A. Amazon Redshift를 사용하여 모든 콘텐츠를 한 곳에 로드하고 필요에 따라 SQL 쿼리를 실행합니다. 
B. Amazon CloudWatch Logs를 사용하여 로그를 저장합니다. Amazon CloudWatch 콘솔에서 필요에 따라 SQL 쿼리를 실행합니다. 
C. Amazon S3와 함께 Amazon Athena를 직접 사용하여 필요에 따라 쿼리를 실행합니다. 
D. AWS Glue를 사용하여 로그를 분류합니다. 필요에 따라 Amazon EMR에서 임시 Apache Spark 클러스터를 사용하여 SQL 쿼리를 실행합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q335
솔루션 설계자는 현금 회수 서비스를 위해 Amazon API Gateway에서 REST API를 설계하고 있습니다. 응용 프로그램에는 컴퓨팅 리소스를 위해 1GB의 메모리와 2GB의 스토리지가 필요합니다. 애플리케이션은 데이터가 관계형 형식이어야 합니다. 최소한의 관리 노력으로 이러한 요구 사항을 충족하는 추가 AWS 서비스 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 아마존 EC2
B. AWS 람다
C. 아마존 RDS
D. 아마존 DynamoDB
E. Amazon Elastic Kubernetes 서비스(Amazon EKS)

<details>
<summary>정답 보기</summary>

**BC**
</details>

---

### Q336
회사에서 AWS에 웹 애플리케이션을 배포했습니다. 이 회사는 조정 요구 사항을 지원하기 위해 기본 DB 인스턴스와 5개의 읽기 전용 복제본을 사용하여 MySQL용 Amazon RDS에서 백 엔드 데이터베이스를 호스팅합니다. 읽기 전용 복제본은 기본 DB 인스턴스보다 1초 이상 뒤처져서는 안 됩니다. 데이터베이스는 정기적으로 예약된 저장 프로시저를 실행합니다. 웹 사이트의 트래픽이 증가함에 따라 복제본은 피크 로드 기간 동안 추가 지연을 경험합니다. 솔루션 설계자는 복제 지연을 최대한 줄여야 합니다. 솔루션 설계자는 애플리케이션 코드에 대한 변경을 최소화하고 지속적인 운영 오버헤드를 최소화해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 데이터베이스를 Amazon Aurora MySQL로 마이그레이션합니다. 읽기 전용 복제본을 Aurora 복제본으로 교체하고 Aurora Auto Scaling을 구성합니다. 저장 프로시저를 Aurora
MySQL 기본 함수로 바꿉니다.
B. 데이터베이스 앞에 Redis 클러스터용 Amazon ElastiCache를 배포합니다. 응용 프로그램이 데이터베이스를 쿼리하기 전에 캐시를 확인하도록 응용 프로그램을 수정하십시오. 저장
프로시저를 AWS Lambda 함수로 바꿉니다.
C. 데이터베이스를 Amazon EC2 인스턴스에서 실행되는 MySQL 데이터베이스로 마이그레이션합니다. 모든 복제본 노드에 대해 컴퓨팅에 최적화된 대규모 EC2 인스턴스를 선택합니다.
EC2 인스턴스에서 저장 프로시저를 유지합니다.
D. 데이터베이스를 Amazon DynamoDB로 마이그레이션합니다. 필요한 처리량을 지원하고 온디맨드 용량 확장을 구성하기 위해 많은 수의 RCU(읽기 용량 단위)를 프로비저닝합니다.
저장 프로시저를 DynamoDB 스트림으로 바꿉니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q337
솔루션 설계자는 Amazon API Gateway를 사용하여 사용자의 요청을 수신할 새 API를 설계하고 있습니다. 요청량은 매우 다양합니다. 단일 요청을 받지 않고 몇 시간이 지날 수 있습니다. 데이터 처리는 비동기식으로 이루어지지만 요청이 이루어진 후 몇 초 이내에 완료되어야 합니다. 최저 비용으로 요구 사항을 제공하기 위해 솔루션 설계자가 API를 호출하도록 해야 하는 컴퓨팅 서비스는 무엇입니까?
A. AWS Glue 작업 
B. AWS Lambda 함수 
C. Amazon Elastic Kubernetes Service(Amazon EKS)에서 호스팅되는 컨테이너화된 서비스 
D. Amazon EC2와 함께 Amazon ECS에서 호스팅되는 컨테이너화된 서비스

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q338
4년 차 미디어 회사는 AWS 계정을 구성하기 위해 AWS Organizations 모든 기능 기능 세트를 사용하고 있습니다. 회사의 재무 팀에 따르면 회원 계정의 청구 정보는 회원 계정의 루트 사 용자를 포함하여 누구도 액세스할 수 없어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 모든 재무 팀 사용자를 IAM 그룹에 추가합니다. Billing이라는 AWS 관리형 정책을 그룹에 연결합니다. 
B. 루트 사용자를 포함한 모든 사용자의 청구 정보에 대한 액세스를 거부하는 자격 증명 기반 정책을 첨부합니다. 
C. 청구 정보에 대한 액세스를 거부하는 서비스 제어 정책(SCP)을 만듭니다. 루트 조직 단위(OU)에 SCP를 연결합니다. 
D. 조직의 모든 기능 기능 집합에서 조직 통합 결제 기능 집합으로 변환합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q339
회사에서 마이크로서비스 기반 서버리스 웹 애플리케이션을 실행합니다. 애플리케이션은 여러 Amazon DynamoDB 테이블에서 데이터를 검색할 수 있어야 합니다. 솔루션 설계자는 애플리 케이션의 기본 성능에 영향을 주지 않고 데이터를 검색할 수 있는 기능을 애플리케이션에 제공해야 합니다. 운영상 가장 효율적인 방식으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS AppSync 파이프라인 해석기
B. Lambda@Edge 기능이 있는 Amazon CloudFront
C. AWS Lambda 함수를 사용하는 엣지 최적화 Amazon API Gateway
D. DynamoDB 커넥터를 사용한 Amazon Athena Federated Query

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q340
회사는 애플리케이션에서 생성하는 대량의 스트리(cid:1535) 데이터를 수집하고 처리해야 합니다. 이 애플리케이션은 Amazon EC2 인스턴스에서 실행되며 기본 설정으로 구성된 Amazon Kinesis Data Streams로 데이터를 전송합니다. 격일로 애플리케이션은 데이터를 소비하고 비즈니스 인텔리전스(BI) 처리를 위해 데이터를 Amazon S3 버킷에 기록합니다. 회사는 Amazon S3가 애플리케이션이 Kinesis Data Streams로 보내는 모든 데이터를 수신하지 못하는 것을 관찰합니다. 솔루션 설계자는 이 문제를 해결하기 위해 무엇을 해야 합니까?
A. 데이터 보존 기간을 수정하여 Kinesis Data Streams 기본 설정을 업데이트합니다. 
B. Kinesis Producer Library(KPL)를 사용하여 Kinesis Data Streams로 데이터를 전송하도록 애플리케이션을 업데이트합니다. 
C. Kinesis Data Streams로 전송되는 데이터의 처리량을 처리하도록 Kinesis 샤드 수를 업데이트합니다. 
D. S3 버킷 내에서 S3 버전 관리를 켜서 S3 버킷에 수집된 모든 객체의 모든 버전을 보존합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q341
텔레마케팅 회사는 AWS에서 고객 콜 센터 기능을 설계하고 있습니다. 이 회사는 여러 화자 인식을 제공하고 대본 파일을 생성하는 솔루션이 필요합니다. 회사는 비즈니스 패턴을 분석하기 위 해 트랜스크립트 파일을 쿼리하려고 합니다. 기록 파일은 감사 목적으로 7년 동안 저장되어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 여러 화자 인식을 위해 Amazon Rekognition을 사용하십시오. 성적표 파일을 Amazon S3에 저장합니다. 성적표 파일 분석을 위해 기계 학습 모델을 사용합니다. 
B. 여러 화자 인식을 위해 Amazon Transcribe를 사용합니다. 성적표 파일 분석에 Amazon Athena를 사용합니다. 
C. 여러 화자 인식을 위해 Amazon Translate를 사용합니다. Amazon Redshift에 기록 파일을 저장합니다. 성적표 파일 분석에 SQL 쿼리를 사용합니다. 
D. 여러 화자 인식을 위해 Amazon Rekognition을 사용합니다. 성적표 파일을 Amazon S3에 저장합니다. 성적표 파일 분석에 Amazon Textract를 사용하십시오.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q342
신입 사원이 배포 엔지니어로 회사에 합류했습니다. 배포 엔지니어는 AWS CloudFormation 템플릿을 사용하여 여러 AWS 리소스를 생성합니다. 솔루션 설계자는 배포 엔지니어가 최소 권한 원칙에 따라 작업 활동을 수행하기를 원합니다. 이 목표를 달성하기 위해 솔루션 설계자가 취해야 하는 작업 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 배포 엔지니어가 AWS CloudFormation 스택 작업을 수행하기 위해 AWS 계정 루트 사용자 자격 증명을 사용하도록 합니다. 
B. 배포 엔지니어를 위한 새 IAM 사용자를 생성하고 PowerUsers IAM 정책이 연결된 그룹에 IAM 사용자를 추가합니다. 
C. 배포 엔지니어를 위한 새 IAM 사용자를 생성하고 AdministratorAccess IAM 정책이 연결된 그룹에 IAM 사용자를 추가합니다. 
D. 배포 엔지니어를 위한 새 IAM 사용자를 생성하고 AWS CloudFormation 작업만 허용하는 IAM 정책이 있는 그룹에 IAM 사용자를 추가합니다. 
E. 배포 엔지니어를 위한 IAM 역할을 생성하여 해당 IAM 역할을 사용하여 AWS CloudFormation 스택 및 시작 스택에 특정한 권한을 명시적으로 정의합니다.

<details>
<summary>정답 보기</summary>

**DE**
</details>

---

### Q343
솔루션 설계자는 애플리케이션이 Amazon RDS DB 인스턴스에 액세스하는 데 사용하는 데이터베이스 사용자 이름과 암호를 안전하게 저장해야 합니다. 데이터베이스에 액세스하는 애플리 케이션은 Amazon EC2 인스턴스에서 실행됩니다. 솔루션 설계자는 AWS Systems Manager Parameter Store에서 보안 매개변수를 생성하려고 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Parameter Store 파라미터에 대한 읽기 액세스 권한이 있는 IAM 역할을 생성합니다. 파라미터를 암호화하는 데 사용되는 AWS Key Management Service(AWS KMS) 키에 대
한 Decrypt 액세스를 허용합니다. 이 IAM 역할을 EC2 인스턴스에 할당합니다.
B. Parameter Store 파라미터에 대한 읽기 액세스를 허용하는 IAM 정책을 생성합니다. 파라미터를 암호화하는 데 사용되는 AWS Key Management Service(AWS KMS) 키에 대
한 Decrypt 액세스를 허용합니다. 이 IAM 정책을 EC2 인스턴스에 할당합니다.
C. Parameter Store 파라미터와 EC2 인스턴스 간에 IAM 신뢰 관계를 생성합니다. 신뢰 정책에서 Amazon RDS를 보안 주체로 지정합니다. 
D. DB 인스턴스와 EC2 인스턴스 간에 IAM 신뢰 관계를 생성합니다. 신뢰 정책에서 Systems Manager를 보안 주체로 지정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q344
회사는 최근 청구서에서 Amazon EC2 비용이 증가했음을 확인했습니다. 청구 팀은 몇 가지 EC2 인스턴스에 대한 인스턴스 유형의 원치 않는 수직 확장을 발견했습니다. 솔루션 아키텍트는 최근 2개월간의 EC2 비용을 비교하는 그래프를 생성하고 심층 분석을 수행하여 수직 확장의 근본 원인을 식별해야 합니다. 솔루션 설계자는 최소한의 운영 오버헤드로 정보를 어떻게 생성해야 합니까?
A. AWS 예산을 사용하여 예산 보고서를 생성하고 인스턴스 유형에 따라 EC2 비용을 비교합니다. 
B. 비용 탐색기의 세분화된 필터링 기능을 사용하여 인스턴스 유형에 따라 EC2 비용을 심층 분석합니다. 
C. AWS Billing and Cost Management 대시보드의 그래프를 사용하여 지난 2개월 동안 인스턴스 유형을 기준으로 EC2 비용을 비교합니다. 
D. AWS 비용 및 사용 보고서를 사용하여 보고서를 생성하고 Amazon S3 버킷으로 보냅니다. Amazon S3와 함께 Amazon QuickSight를 소스로 사용하여 인스턴스 유형을 기반으로
대화형 그래프를 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q345
한 회사가 Application Load Balancer 뒤의 Amazon EC2 온디맨드 인스턴스 그룹에서 프로덕션 환경의 상태 비저장 웹 애플리케이션을 실행합니다. 애플리케이션은 각 영업일 8시간 동안 사용량이 많습니다. 응용 프로그램 사용량은 밤 사이 중간 정도이며 안정적입니다. 주말에는 애플리케이션 사용량이 적습니다. 회사는 애플리케이션의 가용성에 영향을 미치지 않으면서 EC2 비용을 최소화하려고 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 전체 워크로드에 스팟 인스턴스를 사용합니다. 
B. 기준 사용 수준에 대해 예약 인스턴스를 사용합니다. 애플리케이션에 필요한 추가 용량에는 스팟 인스턴스를 사용하십시오. 
C. 기본 사용 수준에 대해 온디맨드 인스턴스를 사용합니다. 애플리케이션에 필요한 추가 용량에는 스팟 인스턴스를 사용하십시오. 
D. 기본 사용 수준에 전용 인스턴스를 사용합니다. 애플리케이션에 필요한 추가 용량에 대해서는 온디맨드 인스턴스를 사용하십시오.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q346
IAM 사용자는 지난 주 프로덕션 배포 중에 회사 계정의 AWS 리소스에 대해 몇 가지 구성을 변경했습니다. 솔루션 설계자는 몇 가지 보안 그룹 규칙이 원하는 대로 구성되지 않았음을 알게 되 었습니다. 솔루션 설계자는 어떤 IAM 사용자가 변경을 담당했는지 확인하려고 합니다. 솔루션 설계자는 원하는 정보를 찾기 위해 어떤 서비스를 사용해야 합니까?
A. Amazon GuardDuty 
B. 아마존 인스펙터 
C. AWS 클라우드트레일 
D. AWS 구성

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q347
한 회사는 AWS에서 서버리스 애플리케이션을 운영하며, 이 애플리케이션은 백엔드 데이터베이스로 Amazon RDS를 사용합니다. 애플리케이션은 때때로 예측할 수 없는 급격한 트래픽 증 가를 겪습니다. 트래픽이 증가할 때마다 애플리케이션은 데이터베이스에 대해 자주 연결을 열고 닫으며, 이로 인해 데이터베이스로부터 오류를 받거나 연결이 부족해지는 문제가 발생합니다. 회사는 애플리케이션이 항상 확장 가능하고 고가용성을 유지할 수 있도록 해야 합니다. 어떤 해결책이 이러한 요구사항을 충족시키며 애플리케이션의 코드 변경 없이 가능할까요?
A. 서버리스 애플리케이션의 RDS 데이터베이스의 옵션 그룹에서 최대 연결 수를 증가시킵니다. 
B. RDS DB 인스턴스의 인스턴스 크기를 최대 부하 트래픽에 맞게 증가시킵니다. 
C. 서버리스 애플리케이션과 Amazon RDS 사이에 Amazon RDS 프록시를 배포합니다. 
D. Amazon RDS에 대한 예약 인스턴스를 구매하여 최대 부하 트래픽 시에도 데이터베이스를 고가용성으로 유지합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q348
솔루션 아키텍트가 Policy1과 Policy2라는 두 가지 IAM 정책을 만들었습니다. 두 정책 모두 IAM 그룹에 연결됩니다. 클라우드 엔지니어가 IAM 그룹에 IAM 사용자로 추가됩니다. 클라우드 엔지니어는 어떤 작업을 수행할 수 있습니까?
A. IAM 사용자 삭제 
B. 디렉토리 삭제 
C. Amazon EC2 인스턴스 삭제 
D. Amazon CloudWatch Logs에서 로그 삭제

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q349
글로벌 이벤트의 주최자는 일일 보고서를 정적 HTML 페이지로 온라인에 게시하려고 합니다. 이 페이지는 전 세계 사용자로부터 수백만 건의 조회수를 생성할 것으로 예상됩니다. 파일은 Amazon S3 버킷에 저장됩니다. 솔루션 설계자는 효율적이고 효과적인 솔루션을 설계하라는 요청을 받았습니다. 이를 달성하기 위해 솔루션 설계자는 어떤 조치를 취해야 합니까?
A. 파일에 대해 미리 서명된 URL을 생성합니다. 
B. 모든 리전에 교차 리전 복제를 사용합니다. 
C. Amazon Route 53의 지리적 근접성 기능을 사용합니다. 
D. S3 버킷과 함께 Amazon CloudFront를 원본으로 사용합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q350
한 회사에 IPv6 주소를 사용하여 Amazon EC2 인스턴스에서 호스팅되는 애플리케이션이 있습니다. 애플리케이션은 인터넷을 사용하여 다른 외부 애플리케이션과의 통신을 시작해야 합니 다. 그러나 회사의 보안 정책에 따르면 외부 서비스는 EC2 인스턴스에 대한 연결을 시작할 수 없습니다. 솔루션 설계자는 이 문제를 해결하기 위해 무엇을 권장해야 합니까?
A. NAT 게이트웨이를 생성하고 이를 서브넷 라우팅 테이블의 대상으로 만듭니다. 
B. 인터넷 게이트웨이를 만들고 이를 서브넷의 라우팅 테이블 대상으로 만듭니다. 
C. 가상 프라이빗 게이트웨이를 만들고 이를 서브넷의 라우팅 테이블 대상으로 만듭니다. 
D. 외부 전용 인터넷 게이트웨이를 만들고 이를 서브넷 라우팅 테이블의 대상으로 만듭니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q351
자전거 공유 회사는 피크 운영 시간 동안 자전거의 위치를 추적하기 위해 다계층 아키텍처를 개발하고 있습니다. 회사는 기존 분석 플랫폼에서 이러한 데이터 포인트를 사용하려고 합니다. 솔루 션 설계자는 이 아키텍처를 지원하기 위해 가장 실행 가능한 다중 계층 옵션을 결정해야 합니다. 데이터 포인트는 REST API에서 액세스할 수 있어야 합니다. 위치 데이터 저장 및 검색에 대한 이러한 요구 사항을 충족하는 작업은 무엇입니까?
A. Amazon S3와 함께 Amazon Athena를 사용합니다. 
B. AWS Lambda와 함께 Amazon API Gateway를 사용합니다. 
C. Amazon Redshift와 함께 Amazon QuickSight를 사용합니다. 
D. Amazon Kinesis Data Analytics와 함께 Amazon API Gateway를 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q352
회사의 애플리케이션은 Auto Scaling 그룹의 Amazon EC2 인스턴스에서 실행됩니다. 회사는 해당 애플리케이션이 일주일 중 임의의 요일에 갑작스러운 트래픽 증가를 경험한다는 사실을 발견했습니다. 회사는 갑작스러운 트래픽 증가 중에도 애플리케이션 성능을 유지하려고 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. Auto Scaling 그룹의 크기를 변경하려면 수동 스케일링을 사용하십시오. 
B. 예측 조정을 사용하여 Auto Scaling 그룹의 크기를 변경합니다. 
C. 동적 스케일링을 사용하여 Auto Scaling 그룹의 크기를 변경합니다. 
D. 일정 조정을 사용하여 Auto Scaling 그룹의 크기를 변경합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q353
한 회사가 많은 독립 실행형 AWS 계정에서 통합된 다중 계정 아키텍처로 이동하려고 합니다. 이 회사는 다양한 사업부에 대해 많은 새 AWS 계정을 생성할 계획입니다. 회사는 중앙 집중식 회사 디렉터리 서비스를 사용하여 이러한 AWS 계정에 대한 액세스를 인증해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자가 권장해야 하는 작업 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 모든 기능을 켠 상태에서 AWS Organizations에 새 조직을 만듭니다. 조직에서 새 AWS 계정을 생성합니다. 
B. Amazon Cognito 자격 증명 풀을 설정합니다. Amazon Cognito 인증을 수락하도록 AWS IAM Identity Center(AWS Single Sign-On)를 구성합니다. 
C. AWS 계정을 관리하기 위해 서비스 제어 정책(SCP)을 구성합니다. AWS IAM Identity Center(AWS Single Sign-On)를 AWS Directory Service에 추가합니다. 
D. AWS Organizations에서 새 조직을 생성합니다. AWS Directory Service를 직접 사용하도록 조직의 인증 메커니즘을 구성합니다. 
E. 조직에서 AWS IAM Identity Center(AWS Single Sign-On)를 설정합니다. IAM Identity Center를 구성하고 회사의 회사 디렉터리 서비스와 통합합니다.

<details>
<summary>정답 보기</summary>

**AE**
</details>

---

### Q354
회사에서 대량의 생산 데이터를 동일한 AWS 리전의 테스트 환경으로 복제하는 기능을 개선하려고 합니다. 데이터는 Amazon Elastic Block Store(Amazon EBS) 볼륨의 Amazon EC2 인스턴스에 저장됩니다. 복제된 데이터에 대한 수정은 생산 환경에 영향을 미치지 않아야 합니다. 이 데이터에 액세스하는 소프트웨어에는 지속적으로 높은 I/O 성능이 필요합니다. 솔루션 설계자는 프로덕션 데이터를 테스트 환경으로 복제하는 데 필요한 시간을 최소화해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 프로덕션 EBS 볼륨의 EBS 스냅샷을 찍습니다. 테스트 환경의 EC2 인스턴스 스토어 볼륨에 스냅샷을 복원합니다. 
B. EBS 다중 연결 기능을 사용하도록 프로덕션 EBS 볼륨을 구성합니다. 프로덕션 EBS 볼륨의 EBS 스냅샷을 생성합니다. 프로덕션 EBS 볼륨을 테스트 환경의 EC2 인스턴스에 연결합
니다.
C. 프로덕션 EBS 볼륨의 EBS 스냅샷을 찍습니다. 새 EBS 볼륨을 생성하고 초기화합니다. 프로덕션 EBS 스냅샷에서 볼륨을 복원하기 전에 새 EBS 볼륨을 테스트 환경의 EC2 인스턴
스에 연결합니다.
D. 프로덕션 EBS 볼륨의 EBS 스냅샷을 찍습니다. EBS 스냅샷에서 EBS 빠른 스냅샷 복원 기능을 켭니다. 스냅샷을 새 EBS 볼륨으로 복원합니다. 테스트 환경에서 새 EBS 볼륨을
EC2 인스턴스에 연결합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q355
회사는 회사의 AWS 계정에서 작업을 수행하기 위해 외부 공급업체를 고용했습니다. 벤더는 벤더가 소유한 AWS 계정에서 호스팅되는 자동화 도구를 사용합니다. 공급업체는 회사의 AWS 계정에 대한 IAM 액세스 권한이 없습니다. 솔루션 설계자는 공급업체에 이 액세스 권한을 어떻게 부여해야 합니까?
A. 공급업체의 IAM 역할에 대한 액세스 권한을 위임하려면 회사 계정에서 IAM 역할을 생성합니다. 벤더가 요구하는 권한에 대한 역할에 적절한 IAM 정책을 연결합니다. 
B. 암호 복잡성 요구 사항을 충족하는 암호를 사용하여 회사 계정에서 IAM 사용자를 생성합니다. 벤더가 요구하는 권한에 대해 적절한 IAM 정책을 사용자에게 연결합니다. 
C. 회사 계정에 IAM 그룹을 생성합니다. 공급업체 계정의 도구 IAM 사용자를 그룹에 추가합니다. 공급업체에 필요한 권한에 대해 적절한 IAM 정책을 그룹에 연결합니다. 
D. IAM 콘솔에서 공급자 유형으로 "AWS 계정"을 선택하여 새 자격 증명 공급자를 만듭니다. 공급업체의 AWS 계정 ID와 사용자 이름을 제공합니다. 벤더가 요구하는 권한에 대해 적절한
IAM 정책을 새 제공자에 연결하십시오.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q356
회사에서 고가용성 SFTP 서비스를 실행합니다. SFTP 서비스는 탄력적 IP 주소로 실행되는 두 개의 Amazon EC2 Linux 인스턴스를 사용하여 인터넷에서 신뢰할 수 있는 IP 소스의 트래 픽을 허용합니다. SFTP 서비스는 인스턴스에 연결된 공유 스토리지에서 지원합니다. 사용자 계정은 SFTP 서버에서 Linux 사용자로 생성되고 관리됩니다. 회사는 높은 IOPS 성능과 고도로 구성 가능한 보안을 제공하는 서버리스 옵션을 원합니다. 회사는 또한 사용자 권한에 대한 제어를 유지하기를 원합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 암호화된 Amazon Elastic Block Store(Amazon EBS) 볼륨을 생성합니다. 신뢰할 수 있는 IP 주소만 허용하는 퍼블릭 엔드포인트로 AWS Transfer Family SFTP 서비스를 생
성합니다. EBS 볼륨을 SFTP 서비스 엔드포인트에 연결합니다. 사용자에게 SFTP 서비스에 대한 액세스 권한을 부여합니다.
B. 암호화된 Amazon Elastic File System(Amazon EFS) 볼륨을 생성합니다. 탄력적 IP 주소와 인터넷 연결 액세스가 있는 VPC 엔드포인트를 사용하여 AWS Transfer Family
SFTP 서비스를 생성합니다. 신뢰할 수 있는 IP 주소만 허용하는 엔드포인트에 보안 그룹을 연결합니다. EFS 볼륨을 SFTP 서비스 엔드포인트에 연결합니다. 사용자에게 SFTP 서비 스에 대한 액세스 권한을 부여합니다.
C. 기본 암호화가 활성화된 Amazon S3 버킷을 생성합니다. 신뢰할 수 있는 IP 주소만 허용하는 퍼블릭 엔드포인트로 AWS Transfer Family SFTP 서비스를 생성합니다. S3 버킷을
SFTP 서비스 엔드포인트에 연결합니다. 사용자에게 SFTP 서비스에 대한 액세스 권한을 부여합니다.
D. 기본 암호화가 활성화된 Amazon S3 버킷을 생성합니다. 프라이빗 서브넷에서 내부 액세스 권한이 있는 VPC 엔드포인트로 AWS Transfer Family SFTP 서비스를 생성합니다. 신
뢰할 수 있는 IP 주소만 허용하는 보안 그룹을 연결합니다. S3 버킷을 SFTP 서비스 엔드포인트에 연결합니다. 사용자에게 SFTP 서비스에 대한 액세스 권한을 부여합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q357
솔루션 설계자는 원하는 Amazon EC2 용량에 도달하기 전에 야간 배치 처리 작업이 1시간 동안 자동으로 확장되는 것을 관찰합니다. 최대 용량은 '매일 밤 동일하며 배치 작업은 항상 오전 1시에 시작됩니다. 솔루션 설계자는 원하는 EC2 용량에 빠르게 도달하고 배치 작업이 완료된 후 Auto Scaling 그룹이 축소될 수 있는 비용 효율적인 솔루션을 찾아야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Auto Scaling 그룹의 최소 용량을 늘립니다. 
B. Auto Scaling 그룹의 최대 용량을 늘립니다. 
C. 원하는 컴퓨팅 수준으로 확장하도록 예약된 확장을 구성합니다. 
D. 각 조정 작업 중에 더 많은 EC2 인스턴스를 추가하도록 조정 정책을 변경합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q358
회사에는 매일 동시에 실행되는 AWS Glue 추출, 변환 및 로드(ETL) 작업이 있습니다. 작업은 Amazon S3 버킷에 있는 XML 데이터를 처리합니다. S3 버킷에는 매일 새 데이터가 추가 됩니다. 솔루션 설계자는 각 실행 중에 AWS Glue가 모든 데이터를 처리하고 있음을 확인합니다. 솔루션 설계자는 AWS Glue가 오래된 데이터를 재처리하지 못하도록 어떻게 해야 합니까?
A. 작업 북마크를 사용하도록 작업을 편집합니다. 
B. 작업을 편집하여 데이터 처리 후 데이터를 삭제합니다. 
C. NumberOfWorkers 필드를 1로 설정하여 작업을 편집합니다. 
D. FindMatches 기계 학습(ML) 변환을 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q359
한 회사가 AWS 클라우드의 Auto Scaling 그룹에 속하는 Amazon EC2 인스턴스에서 게임 애플리케이션을 실행하려고 합니다. 애플리케이션은 UDP 패킷을 사용하여 데이터를 전송합 니다. 회사는 트래픽이 증가하거나 감소함에 따라 애플리케이션을 확장 및 축소할 수 있기를 원합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Auto Scaling 그룹에 Network Load Balancer를 연결합니다. 
B. Auto Scaling 그룹에 Application Load Balancer를 연결합니다. 
C. 트래픽을 적절하게 라우팅하기 위한 가중치 정책이 포함된 Amazon Route 53 레코드 세트를 배포합니다. 
D. Auto Scaling 그룹의 EC2 인스턴스에 대한 포트 전달로 구성된 NAT 인스턴스를 배포합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q360
회사의 애플리케이션은 데이터 수집을 위해 여러 SaaS(Software-as-a-Service) 소스와 통합됩니다. 회사는 Amazon EC2 인스턴스를 실행하여 데이터를 수신하고 분석을 위해 데이터 를 Amazon S3 버킷에 업로드합니다. 데이터를 수신하고 업로드하는 동일한 EC2 인스턴스도 업로드가 완료되면 사용자에게 알림을 보냅니다. 회사는 느린 응용 프로그램 성능을 발견했으 며 성능을 최대한 개선하고자 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 각 SaaS 소스와 S3 버킷 간에 데이터를 전송하는 Amazon AppFlow 흐름을 생성합니다. S3 버킷에 대한 업로드가 완료되면 Amazon Simple Notification Service(Amazon
SNS) 주제로 이벤트를 보내도록 S3 이벤트 알림을 구성합니다.
B. 각 SaaS 소스에 대한 Amazon EventBridge(Amazon CloudWatch Events) 규칙을 생성하여 출력 데이터를 보냅니다. S3 버킷을 규칙의 대상으로 구성합니다. S3 버킷에 대한
업로드가 완료되면 이벤트를 전송하는 두 번째 EventBridge(Cloud Watch Events) 규칙을 생성합니다. Amazon Simple Notification Service(Amazon SNS) 주제를 두 번째 규칙의 대상으로 구성합니다.
C. EC2 인스턴스 대신 사용할 Docker 컨테이너를 생성합니다. Amazon Elastic Container Service(Amazon ECS)에서 컨테이너화된 애플리케이션을 호스팅합니다. S3 버킷에 대
한 업로드가 완료되면 Amazon Simple Notification Service(Amazon SNS) 주제로 이벤트를 보내도록 Amazon CloudWatch Container Insights를 구성합니다.
D. EC2 인스턴스가 확장될 수 있도록 Auto Scaling 그룹을 생성합니다. S3 버킷에 대한 업로드가 완료되면 Amazon Simple Notification Service(Amazon SNS) 주제로 이벤트
를 보내도록 S3 이벤트 알림을 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q361
회사에서 온프레미스 데이터 세트의 보조 사본으로 Amazon S3를 사용하려고 합니다. 회사는 이 복사본에 액세스할 필요가 거의 없습니다. 스토리지 솔루션의 비용은 최소화되어야 합니다. 이러한 요구 사항을 충족하는 스토리지 솔루션은 무엇입니까?
A. S3 기준
B. S3 지능형 계층화
C. S3 Standard-Infrequent Access(S3 Standard-IA)
D. S3 One Zone-Infrequent Access(S3 One Zone-IA)

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q362
회사는 Amazon RDS에서 지원하는 웹 애플리케이션을 실행합니다. 새로운 데이터베이스 관리자가 실수로 데이터베이스 테이블의 정보를 편집하여 데이터 손실을 일으켰습니다. 이러한 유 형의 사고에서 복구하는 데 도움이 되도록 회사는 지난 30일 동안 변경이 발생하기 5분 전의 상태로 데이터베이스를 복원할 수 있는 기능을 원합니다. 이 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 기능을 디자인에 포함해야 합니까?
A. 읽기 복제본 
B. 수동 스냅샷 
C. 자동 백업 
D. 다중 AZ 배포

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q363
솔루션 설계자는 회사를 위한 다중 계층 애플리케이션을 설계하고 있습니다. 애플리케이션 사용자는 모바일 장치에서 이미지를 업로드합니다. 애플리케이션은 각 이미지의 썸네일을 생성하고 이미지가 성공적으로 업로드되었음을 확인하는 메시지를 사용자에게 반환합니다. 썸네일 생성에는 최대 60초가 소요될 수 있지만 회사는 사용자에게 원본 이미지가 수신되었음을 알리기 위해 더 빠른 응답 시간을 제공하고자 합니다. 솔루션 설계자는 서로 다른 애플리케이션 계층에 요청을 비동기식으로 전달하도록 애플리케이션을 설계해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 사용자 지정 AWS Lambda 함수를 작성하여 썸네일을 생성하고 사용자에게 알립니다. 이미지 업로드 프로세스를 이벤트 소스로 사용하여 Lambda 함수를 호출합니다. 
B. AWS Step Functions 워크플로를 생성합니다. 애플리케이션 계층 간의 오케스트레이션을 처리하고 썸네일 생성이 완료되면 사용자에게 알리도록 Step Functions를 구성합니다. 
C. Amazon Simple Queue Service(Amazon SQS) 메시지 대기열을 생성합니다. 이미지가 업로드되면 썸네일 생성을 위해 SQS 대기열에 메시지를 배치합니다. 이미지가 수신되었
음을 애플리케이션 메시지를 통해 사용자에게 알립니다.
D. Amazon Simple Notification Service(Amazon SNS) 알림 주제 및 구독을 생성합니다. 애플리케이션과 함께 하나의 구독을 사용하여 이미지 업로드가 완료된 후 썸네일을 생성하
십시오. 섬네일 생성이 완료된 후 푸시 알림을 통해 사용자의 모바일 앱에 메시지를 보내려면 두 번째 구독을 사용하십시오.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q364
솔루션 설계자는 웹, 애플리케이션 및 데이터베이스 계층으로 구성된 고가용성 애플리케이션을 설계해야 합니다. HTTPS 콘텐츠 전송은 전송 시간을 최소화하면서 가능한 한 에지에 가까워야 합니다. 이러한 요구 사항을 충족하고 가장 안전한 솔루션은 무엇입니까?
A. 퍼블릭 서브넷에서 여러 중복 Amazon EC2 인스턴스로 퍼블릭 Application Load Balancer(ALB)를 구성합니다. 퍼블릭 ALB를 오리진으로 사용하여 HTTPS 콘텐츠를 제공하도
록 Amazon CloudFront를 구성합니다.
B. 프라이빗 서브넷에서 여러 중복 Amazon EC2 인스턴스로 퍼블릭 Application Load Balancer를 구성합니다. EC2 인스턴스를 오리진으로 사용하여 HTTPS 콘텐츠를 제공하도록
Amazon CloudFront를 구성합니다.
C. 프라이빗 서브넷에서 여러 중복 Amazon EC2 인스턴스로 퍼블릭 ALB(Application Load Balancer)를 구성합니다. 퍼블릭 ALB를 오리진으로 사용하여 HTTPS 콘텐츠를 제공하
도록 Amazon CloudFront를 구성합니다.
D. 퍼블릭 서브넷에서 여러 중복 Amazon EC2 인스턴스로 퍼블릭 Application Load Balancer를 구성합니다. EC2 인스턴스를 오리진으로 사용하여 HTTPS 콘텐츠를 제공하도록
Amazon CloudFront를 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q365
회사는 중앙 집중식 AWS 계정을 사용하여 다양한 Amazon S3 버킷에 로그 데이터를 저장합니다. 솔루션 설계자는 데이터가 S3 버킷에 업로드되기 전에 미사용 데이터가 암호화되었는지 확인해야 합니다. 또한 데이터는 전송 중에 암호화되어야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 클라이언트 측 암호화를 사용하여 S3 버킷에 업로드되는 데이터를 암호화합니다. 
B. 서버 측 암호화를 사용하여 S3 버킷에 업로드되는 데이터를 암호화합니다. 
C. S3 업로드를 위해 S3 관리형 암호화 키(SSE-S3)로 서버 측 암호화를 사용해야 하는 버킷 정책을 만듭니다. 
D. 기본 AWS Key Management Service(AWS KMS) 키를 사용하여 S3 버킷을 암호화하는 보안 옵션을 활성화합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q366
대규모 미디어 회사는 AWS에서 웹 애플리케이션을 호스팅합니다. 회사는 전 세계 사용자가 파일에 안정적으로 액세스할 수 있도록 기밀 미디어 파일 캐싱을 시작하려고 합니다. 콘텐츠는 Amazon S3 버킷에 저장됩니다. 회사는 요청이 지리적으로 발생한 위치에 관계없이 콘텐츠를 신속하게 제공해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS DataSync를 사용하여 S3 버킷을 웹 애플리케이션에 연결합니다. 
B. AWS Global Accelerator를 배포하여 S3 버킷을 웹 애플리케이션에 연결합니다. 
C. Amazon CloudFront를 배포하여 S3 버킷을 CloudFront 에지 서버에 연결합니다. 
D. Amazon Simple Queue Service(Amazon SQS)를 사용하여 S3 버킷을 웹 애플리케이션에 연결합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q367
게임 회사에는 점수를 표시하는 웹 애플리케이션이 있습니다. 애플리케이션은 Application Load Balancer 뒤의 Amazon EC2 인스턴스에서 실행됩니다. 애플리케이션은 Amazon RDS for MySQL 데이터베이스에 데이터를 저장합니다. 사용자는 데이터베이스 읽기 성능으로 인해 긴 지연과 중단을 경험하기 시작했습니다. 회사는 애플리케이션 아키텍처의 변경을 최소 화하면서 사용자 경험을 개선하고자 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 데이터베이스 앞에서 Amazon ElastiCache를 사용하십시오. 
B. 애플리케이션과 데이터베이스 간에 RDS 프록시를 사용합니다. 
C. 애플리케이션을 EC2 인스턴스에서 AWS Lambda로 마이그레이션합니다. 
D. MySQL용 Amazon RDS에서 Amazon DynamoDB로 데이터베이스를 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q368
회사의 컨테이너화된 애플리케이션이 Amazon EC2 인스턴스에서 실행됩니다. 애플리케이션은 다른 비즈니스 애플리케이션과 통신하기 전에 보안 인증서를 다운로드해야 합니다. 회사는 거 의 실시간으로 인증서를 암호화하고 해독할 수 있는 매우 안전한 솔루션을 원합니다. 또한 솔루션은 데이터가 암호화된 후 고가용성 스토리지에 데이터를 저장해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 암호화된 인증서에 대한 AWS Secrets Manager 비밀을 생성합니다. 필요에 따라 인증서를 수동으로 업데이트합니다. 세분화된 IAM 액세스를 사용하여 데이터에 대한 액세스를 제어
합니다.
B. Python 암호화 라이브러리를 사용하여 암호화 작업을 수신하고 수행하는 AWS Lambda 함수를 생성합니다. Amazon S3 버킷에 함수를 저장합니다. 
C. AWS Key Management Service(AWS KMS) 고객 관리형 키를 생성합니다. EC2 역할이 암호화 작업에 KMS 키를 사용하도록 허용합니다. 암호화된 데이터를 Amazon S3에
저장합니다.
D. AWS Key Management Service(AWS KMS) 고객 관리형 키를 생성합니다. EC2 역할이 암호화 작업에 KMS 키를 사용하도록 허용합니다. 암호화된 데이터를 Amazon
Elastic Block Store(Amazon EBS) 볼륨에 저장합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q369
회사에서 해당 애플리케이션을 위한 스토리지 솔루션을 찾고 있습니다. 솔루션은 가용성과 확장성이 높아야 합니다. 또한 솔루션은 기본 프로토콜을 통해 AWS 및 온프레미스의 여러 Linux 인스턴스에 의해 마운트될 수 있고 최소 크기 요구 사항이 없는 파일 시스템으로 작동해야 합니다. 회사는 온프레미스 네트워크에서 VPC로 액세스하기 위해 사이트 간 VPN을 설정했습니다. 이러한 요구 사항을 충족하는 스토리지 솔루션은 무엇입니까?
A. Amazon FSx 다중 AZ 배포 
B. Amazon Elastic Block Store(Amazon EBS) 다중 연결 볼륨 
C. 탑재 대상이 여러 개인 Amazon Elastic File System(Amazon EFS) 
D. 단일 탑재 대상 및 여러 액세스 지점이 있는 Amazon Elastic File System(Amazon EFS)

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q370
비즈니스 애플리케이션은 Amazon EC2에서 호스팅되며 암호화된 객체 스토리지에 Amazon S3를 사용합니다. 최고 정보 보안 책임자는 두 서비스 간의 애플리케이션 트래픽이 공용 인터 넷을 통과해서는 안 된다고 지시했습니다. 규정 준수 요구 사항을 충족하기 위해 솔루션 설계자가 사용해야 하는 기능은 무엇입니까?
A. AWS 키 관리 서비스(AWS KMS) 
B. VPC 엔드포인트 
C. 사설 서브넷 
D. 가상 프라이빗 게이트웨이

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q371
한 전자상거래 회사에서 사용자 트래픽이 증가하고 있습니다. 회사의 스토어는 웹 계층과 별도의 데이터베이스 계층으로 구성된 2계층 웹 애플리케이션으로 Amazon EC2 인스턴스에 배포 됩니다. 트래픽이 증가함에 따라 회사는 아키텍처로 인해 사용자에게 적시에 마케팅 및 주문 확인 이메일을 보내는 데 상당한 지연이 발생하고 있음을 알게 되었습니다. 이 회사는 복잡한 이메 일 전송 문제를 해결하는 데 소요되는 시간을 줄이고 운영 오버헤드를 최소화하기를 원합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 이메일 처리 전용 EC2 인스턴스를 사용하여 별도의 애플리케이션 계층을 만듭니다. 
B. Amazon Simple Email Service(Amazon SES)를 통해 이메일을 보내도록 웹 인스턴스를 구성합니다. 
C. Amazon Simple Notification Service(Amazon SNS)를 통해 이메일을 보내도록 웹 인스턴스를 구성합니다. 
D. 이메일 처리 전용 EC2 인스턴스를 사용하여 별도의 애플리케이션 계층을 생성합니다. Auto Scaling 그룹에 인스턴스를 배치합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q372
회사에서 VPC의 컨테이너에서 실행되는 애플리케이션을 만들고 있습니다. 애플리케이션은 Amazon S3 버킷에 데이터를 저장하고 액세스합니다. 개발 단계에서 애플리케이션은 매일 Amazon S3에 1TB의 데이터를 저장하고 액세스합니다. 회사는 비용을 최소화하고 가능한 한 트래픽이 인터넷을 통과하지 못하도록 막고자 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. S3 버킷에 대해 S3 Intelligent-Tiering을 활성화합니다. 
B. S3 버킷에 대해 S3 Transfer Acceleration을 활성화합니다. 
C. Amazon S3용 게이트웨이 VPC 엔드포인트를 생성합니다. 이 엔드포인트를 VPC의 모든 라우팅 테이블과 연결합니다. 
D. VPC에서 Amazon S3에 대한 인터페이스 엔드포인트를 생성합니다. 이 엔드포인트를 VPC의 모든 라우팅 테이블과 연결합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q373
회사의 웹 애플리케이션은 AWS Lambda 함수 앞의 Amazon API Gateway API와 Amazon DynamoDB 데이터베이스로 구성됩니다. Lambda 함수는 비즈니스 로직을 처리하고 DynamoDB 테이블은 데이터를 호스팅합니다. 애플리케이션은 Amazon Cognito 사용자 풀을 사용하여 애플리케이션의 개별 사용자를 식별합니다. 솔루션 설계자는 구독이 있는 사용자만 프리미엄 콘텐츠에 액세스할 수 있도록 애플리케이션을 업데이트해야 합니다. 최소한의 운영 오버헤드로 이 요구 사항을 충족하는 솔루션은 무엇입니까?
A. API Gateway API에서 API 캐싱 및 제한을 활성화합니다. 
B. API Gateway API에서 AWS WAF를 설정합니다. 구독이 있는 사용자를 필터링하는 규칙을 만듭니다. 
C. DynamoDB 테이블의 프리미엄 콘텐츠에 세분화된 IAM 권한을 적용합니다. 
D. 구독하지 않은 사용자의 액세스를 제한하기 위해 API 사용 계획 및 API 키를 구현하십시오.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q374
트랜잭션 처리 회사에는 Amazon EC2 인스턴스에서 실행되는 매주 스크립팅된 배치 작업이 있습니다. EC2 인스턴스는 Auto Scaling 그룹에 있습니다. 트랜잭션 수는 다를 수 있지만 각 실행에서 기록되는 기준 CPU 사용률은 60% 이상입니다. 회사는 작업이 실행되기 30분 전에 용량을 프로비저닝해야 합니다. 현재 엔지니어는 Auto Scaling 그룹 파라미터를 수동으로 수정하여 이 작업을 완료합니다. 회사에는 Auto Scaling 그룹 수에 필요한 용량 추세를 분석할 리소스가 없습니다. 회사는 Auto Scaling 그룹의 원하는 용량을 수정하는 자동화된 방법이 필요합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Auto Scaling 그룹에 대한 동적 조정 정책을 생성합니다. CPU 사용률 메트릭을 기반으로 확장하도록 정책을 구성합니다. 지표의 대상 값을 60%로 설정합니다. 
B. Auto Scaling 그룹에 대한 예약 조정 정책을 생성합니다. 원하는 적정 용량, 최소 용량, 최대 용량을 설정합니다. 반복을 매주로 설정합니다. 일괄 작업이 실행되기 전 30분으로 시작 시
간을 설정합니다.
C. Auto Scaling 그룹에 대한 예측 조정 정책을 생성합니다. 예측을 기반으로 확장하도록 정책을 구성합니다. 스케일링 지표를 CPU 사용률로 설정합니다. 지표의 대상 값을 60%로 설정
합니다. 정책에서 작업이 실행되기 30분 전에 사전 실행되도록 인스턴스를 설정합니다.
D. Auto Scaling 그룹의 CPU 사용률 지표 값이 60%에 도달하면 AWS Lambda 함수를 호출하는 Amazon EventBridge 이벤트를 생성합니다. Auto Scaling 그룹의 원하는 용량
과 최대 용량을 20% 늘리도록 Lambda 함수를 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q375
온라인 학습 회사가 AWS 클라우드로 마이그레이션하고 있습니다. 회사는 PostgreSQL 데이터베이스에 학생 기록을 유지합니다. 회사는 여러 AWS 리전에서 데이터를 항상 온라인으로 사 용할 수 있는 솔루션이 필요합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. PostgreSQL 데이터베이스를 Amazon EC2 인스턴스의 PostgreSQL 클러스터로 마이그레이션합니다. 
B. PostgreSQL 데이터베이스를 다중 AZ 기능이 켜진 PostgreSQL DB 인스턴스용 Amazon RDS로 마이그레이션합니다. 
C. PostgreSQL 데이터베이스를 Amazon RDS for PostgreSQL DB 인스턴스로 마이그레이션합니다. 다른 리전에서 읽기 전용 복제본을 생성합니다. 
D. PostgreSQL 데이터베이스를 Amazon RDS for PostgreSQL DB 인스턴스로 마이그레이션합니다. 다른 리전에 복사할 DB 스냅샷을 설정합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q376
개발 팀은 성능 개선 도우미가 활성화된 MySQL DB 인스턴스용 범용 Amazon RDS에서 매월 리소스 집약적인 테스트를 실행합니다. 테스트는 한 달에 한 번 48시간 동안 진행되며 데이 터베이스를 사용하는 유일한 프로세스입니다. 팀은 DB 인스턴스의 컴퓨팅 및 메모리 속성을 줄이지 않고 테스트 실행 비용을 줄이려고 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 테스트가 완료되면 DB 인스턴스를 중지합니다. 필요한 경우 DB 인스턴스를 다시 시작합니다. 
B. DB 인스턴스와 함께 Auto Scaling 정책을 사용하여 테스트가 완료되면 자동으로 조정합니다. 
C. 테스트가 완료되면 스냅샷을 생성합니다. 필요한 경우 DB 인스턴스를 종료하고 스냅샷을 복원합니다. 
D. 테스트가 완료되면 DB 인스턴스를 저용량 인스턴스로 수정한다. 필요한 경우 DB 인스턴스를 다시 수정합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q377
한 회사에서 최근 3계층 애플리케이션을 VPC로 마이그레이션하는 것을 검토하고 있습니다. 보안 팀은 최소 권한 원칙이 애플리케이션 계층 간의 Amazon EC2 보안 그룹 수신 및 송신 규칙 에 적용되지 않는다는 사실을 발견했습니다. 솔루션 설계자는 이 문제를 해결하기 위해 무엇을 해야 합니까?
A. 인스턴스 ID를 소스 또는 대상으로 사용하여 보안 그룹 규칙을 생성합니다. 
B. 보안 그룹 ID를 소스 또는 대상으로 사용하여 보안 그룹 규칙을 생성합니다. 
C. VPC CIDR 블록을 소스 또는 대상으로 사용하여 보안 그룹 규칙을 생성합니다. 
D. 서브넷 CIDR 블록을 소스 또는 대상으로 사용하여 보안 그룹 규칙을 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q378
회사는 여러 Amazon EC2 인스턴스에서 웹 애플리케이션을 호스팅합니다. EC2 인스턴스는 사용자 요구에 따라 확장되는 Auto Scaling 그룹에 있습니다. 회사는 장기적인 약정 없이 비 용 절감을 최적화하기를 원합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자가 권장해야 하는 EC2 인스턴스 구매 옵션은 무엇입니까?
A. 전용 인스턴스만 해당 
B. 온디맨드 인스턴스 전용 
C. 온디맨드 인스턴스와 스팟 인스턴스의 혼합 
D. 온디맨드 인스턴스와 예약 인스턴스의 혼합

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q379
회사에서 레거시 애플리케이션을 사용하여 데이터를 CSV 형식으로 생성합니다. 레거시 애플리케이션은 출력 데이터를 Amazon S3에 저장합니다. 이 회사는 복잡한 SQL 쿼리를 수행하여 Amazon Redshift 및 Amazon S3에만 저장된 데이터를 분석할 수 있는 새로운 상용 기성품(COTS) 애플리케이션을 배포하고 있습니다. 그러나 COTS 애플리케이션은 레거시 애플리케 이션이 생성하는 .csv 파일을 처리할 수 없습니다. 회사는 레거시 애플리케이션을 업데이트하여 다른 형식으로 데이터를 생성할 수 없습니다. 회사는 COTS 애플리케이션이 레거시 애플리케이션이 생성하는 데이터를 사용할 수 있도록 솔루션 을 구현해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 일정에 따라 실행되는 AWS Glue 추출, 변환 및 로드(ETL) 작업을 생성합니다. .csv 파일을 처리하고 처리된 데이터를 Amazon Redshift에 저장하도록 ETL 작업을 구성합니다. 
B. Amazon EC2 인스턴스에서 실행되는 Python 스크립트를 개발하여 .csv 파일을 .sql 파일로 변환합니다. Cron 일정에서 Python 스크립트를 호출하여 출력 파일을 Amazon S3에
저장합니다.
C. AWS Lambda 함수와 Amazon DynamoDB 테이블을 생성합니다. S3 이벤트를 사용하여 Lambda 함수를 호출합니다. ETL(추출, 변환 및 로드) 작업을 수행하여 .csv 파일을 처
리하고 처리된 데이터를 DynamoDB 테이블에 저장하도록 Lambda 함수를 구성합니다.
D. Amazon EventBridge를 사용하여 매주 일정에 따라 Amazon EMR 클러스터를 시작합니다. 추출, 변환 및 로드(ETL) 작업을 수행하여 .csv 파일을 처리하고 처리된 데이터를
Amazon Redshift 테이블에 저장하도록 EMR 클러스터를 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q380
솔루션 아키텍트가 MySQL 데이터베이스로 복잡한 Java 애플리케이션을 구현하고 있습니다. Java 애플리케이션은 Apache Tomcat에 배포되어야 하며 고가용성이어야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS Lambda에 애플리케이션을 배포합니다. Lambda 함수와 연결하도록 Amazon API Gateway API를 구성합니다. 
B. AWS Elastic Beanstalk를 사용하여 애플리케이션을 배포합니다. 부하 분산 환경 및 롤링 배포 정책을 구성합니다. 
C. 데이터베이스를 Amazon ElastiCache로 마이그레이션합니다. 애플리케이션에서 액세스를 허용하도록 ElastiCache 보안 그룹을 구성합니다. 
D. Amazon EC2 인스턴스를 시작합니다. EC2 인스턴스에 MySQL 서버를 설치합니다. 서버에서 애플리케이션을 구성합니다. AMI를 생성합니다. AMI를 사용하여 Auto Scaling 그룹
으로 시작 템플릿을 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q381
회사에는 Amazon S3에 백업되는 대량의 시간에 민감한 데이터를 생성하는 온프레미스 애플리케이션이 있습니다. 애플리케이션이 성장했고 인터넷 대역폭 제한에 대한 사용자 불만이 있습 니다. 솔루션 설계자는 Amazon S3에 적시에 백업하고 내부 사용자의 인터넷 연결에 미치는 영향을 최소화할 수 있는 장기 솔루션을 설계해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS VPN 연결을 설정하고 VPC 게이트웨이 엔드포인트를 통해 모든 트래픽을 프록시합니다. 
B. 새로운 AWS Direct Connect 연결을 설정하고 이 새로운 연결을 통해 백업 트래픽을 전달합니다. 
C. 매일 AWS Snowball 디바이스를 주문합니다. Snowball 디바이스에 데이터를 로드하고 디바이스를 매일 AWS에 반환합니다. 
D. AWS Management Console을 통해 지원 티켓을 제출합니다. 계정에서 S3 서비스 제한 제거를 요청합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q382
회사의 시설에는 건물 전체의 모든 입구에 배지 판독기가 있습니다. 배지를 스캔하면 판독기가 HTTPS를 통해 메시지를 보내 누가 해당 입구에 액세스하려고 시도했는지 나타냅니다. 솔루션 설계자는 센서에서 보내는 이러한 메시지를 처리하는 시스템을 설계해야 합니다. 솔루션은 가용성이 높아야 하며 회사의 보안 팀이 분석할 수 있도록 결과를 제공해야 합니다. 솔루션 설계자는 어떤 시스템 아키텍처를 추천해야 합니까?
A. Amazon EC2 인스턴스를 시작하여 HTTPS 엔드포인트 역할을 하고 메시지를 처리합니다. 결과를 Amazon S3 버킷에 저장하도록 EC2 인스턴스를 구성합니다. 
B. Amazon API Gateway에서 HTTPS 엔드포인트를 생성합니다. AWS Lambda 함수를 호출하여 메시지를 처리하고 결과를 Amazon DynamoDB 테이블에 저장하도록 API
Gateway 엔드포인트를 구성합니다.
C. Amazon Route 53을 사용하여 들어오는 센서 메시지를 AWS Lambda 함수로 보냅니다. 메시지를 처리하고 결과를 Amazon DynamoDB 테이블에 저장하도록 Lambda 함수를
구성합니다.
D. Amazon S3용 게이트웨이 VPC 엔드포인트를 생성합니다. 센서 데이터가 VPC 엔드포인트를 통해 S3 버킷에 직접 기록될 수 있도록 시설 네트워크에서 VPC로의 Site-to-Site
VPN 연결을 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q383
회사는 Amazon EC2 인스턴스와 AWS Lambda 함수를 사용하여 애플리케이션을 실행합니다. 이 회사는 AWS 계정에 퍼블릭 서브넷과 프라이빗 서브넷이 있는 VPC가 있습니다. EC2 인스턴스는 VPC 중 하나의 프라이빗 서브넷에서 실행됩니다. 애플리케이션이 작동하려면 Lambda 함수가 EC2 인스턴스에 대한 직접적인 네트워크 액세스가 필요합니다. 응용 프로그램은 최소 1년 동안 실행됩니다. 회사는 해당 시간 동안 애플리케이션이 사용하는 Lambda 함수의 수가 증가할 것으로 예상합니다. 회사는 모든 애플리케이션 리소스에 대한 절감 효과를 극대화하고 서비스 간의 네트워크 대기 시간을 낮게 유지하려고 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. EC2 Instance Savings Plan 구매 Lambda 함수의 지속 시간, 메모리 사용량 및 호출 수를 최적화합니다. EC2 인스턴스가 포함된 프라이빗 서브넷에 Lambda 함수를 연결합니다
.
B. EC2 Instance Savings Plan 구매 Lambda 함수의 기간 및 메모리 사용량, 호출 수 및 전송되는 데이터 양을 최적화합니다. EC2 인스턴스가 실행되는 동일한 VPC의 퍼블릭 서브
넷에 Lambda 함수를 연결합니다.
C. Compute Savings Plan을 구매합니다. Lambda 함수의 기간 및 메모리 사용량, 호출 수 및 전송되는 데이터 양을 최적화합니다. EC2 인스턴스가 포함된 프라이빗 서브넷에
Lambda 함수를 연결합니다.
D. Compute Savings Plan을 구매합니다. Lambda 함수의 기간 및 메모리 사용량, 호출 수 및 전송되는 데이터 양을 최적화합니다. Lambda 서비스 VPC에 Lambda 함수를 유지합
니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q384
미디어 회사는 온프레미스에서 사용자 활동 데이터를 수집하고 분석합니다. 회사는 이 기능을 AWS로 마이그레이션하려고 합니다. 사용자 활동 데이터 저장소는 계속해서 성장하여 크기가 페 타바이트가 될 것입니다. 회사는 SQL을 사용하여 기존 데이터 및 새 데이터의 온디맨드 분석을 용이하게 하는 고가용성 데이터 수집 솔루션을 구축해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 활동 데이터를 Amazon Kinesis 데이터 스트림으로 보냅니다. 데이터를 Amazon S3 버킷으로 전달하도록 스트림을 구성합니다. 
B. 활동 데이터를 Amazon Kinesis Data Firehose 전송 스트림으로 보냅니다. 데이터를 Amazon Redshift 클러스터로 전달하도록 스트림을 구성합니다. 
C. 활동 데이터를 Amazon S3 버킷에 배치합니다. 데이터가 S3 버킷에 도착하면 데이터에서 AWS Lambda 함수를 실행하도록 Amazon S3를 구성합니다. 
D. 여러 가용 영역에 분산된 Amazon EC2 인스턴스에서 수집 서비스를 생성합니다. 데이터를 Amazon RDS 다중 AZ 데이터베이스로 전달하도록 서비스를 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q385
한 회사에서 MySQL DB 인스턴스용 Amazon RDS를 출시했습니다. 데이터베이스에 대한 대부분의 연결은 서버리스 애플리케이션에서 발생합니다. 데이터베이스에 대한 애플리케이션 트 래픽은 임의의 간격으로 크게 변경됩니다. 수요가 많을 때 사용자는 애플리케이션에 데이터베이스 연결 거부 오류가 발생한다고 보고합니다. 최소한의 운영 오버헤드로 이 문제를 해결하는 솔루션은 무엇입니까?
A. RDS Proxy에서 프록시를 생성합니다. RDS Proxy를 통해 DB 인스턴스를 사용하도록 사용자 애플리케이션을 구성합니다. 
B. 사용자 애플리케이션과 DB 인스턴스 간에 Amazon ElastiCache for Memcached를 배포합니다. 
C. I/O 용량이 더 큰 다른 인스턴스 클래스로 DB 인스턴스를 마이그레이션합니다. 새 DB 인스턴스를 사용하도록 사용자 애플리케이션을 구성합니다. 
D. DB 인스턴스에 대한 다중 AZ를 구성합니다. DB 인스턴스 간에 전환하도록 사용자 애플리케이션을 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q386
회사의 웹 사이트는 사용자에게 다운로드 가능한 과거 실적 보고서를 제공합니다. 웹 사이트에는 전 세계적으로 회사의 웹 사이트 요구 사항을 충족하도록 확장할 수 있는 솔루션이 필요합니다. 솔루션은 비용 효율적이어야 하고 인프라 리소스의 프로비저닝을 제한하며 가능한 가장 빠른 응답 시간을 제공해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 어떤 조합을 권장해야 합니까?
A. Amazon CloudFront 및 Amazon S3 
B. AWS Lambda 및 Amazon DynamoDB 
C. Amazon EC2 Auto Scaling을 사용하는 애플리케이션 로드 밸런서 
D. 내부 Application Load Balancer가 있는 Amazon Route 53

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q387
애플리케이션은 프라이빗 서브넷의 Amazon EC2 인스턴스에서 실행됩니다. 애플리케이션은 Amazon DynamoDB 테이블에 액세스해야 합니다. 트래픽이 AWS 네트워크를 벗어나지 않도록 하면서 테이블에 액세스하는 가장 안전한 방법은 무엇입니까?
A. DynamoDB용 VPC 엔드포인트를 사용합니다. 
B. 퍼블릭 서브넷에서 NAT 게이트웨이를 사용합니다. 
C. 프라이빗 서브넷에서 NAT 인스턴스를 사용합니다. 
D. VPC에 연결된 인터넷 게이트웨이를 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q388
회사에서 Windows 기반 애플리케이션을 온프레미스에서 AWS 클라우드로 마이그레이션하려고 합니다. 애플리케이션에는 애플리케이션 계층, 비즈니스 계층 및 Microsoft SQL Server 가 포함된 데이터베이스 계층의 세 가지 계층이 있습니다. 회사는 기본 백업 및 데이터 품질 서비스와 같은 SQL Server의 특정 기능을 사용하려고 합니다. 또한 회사는 계층 간에 처리를 위해 파일을 공유해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 아키텍처를 어떻게 설계해야 합니까?
A. Amazon EC2 인스턴스에서 세 계층을 모두 호스팅합니다. 계층 간 파일 공유를 위해 Amazon FSx File Gateway를 사용합니다. 
B. Amazon EC2 인스턴스에서 세 계층을 모두 호스팅합니다. 계층 간 파일 공유를 위해 Amazon FSx for Windows File Server를 사용하십시오. 
C. Amazon EC2 인스턴스에서 애플리케이션 계층과 비즈니스 계층을 호스팅합니다. Amazon RDS에서 데이터베이스 계층을 호스팅합니다. 계층 간 파일 공유를 위해 Amazon
Elastic File System(Amazon EFS)을 사용합니다.
D. Amazon EC2 인스턴스에서 애플리케이션 계층과 비즈니스 계층을 호스팅합니다. Amazon RDS에서 데이터베이스 계층을 호스팅합니다. 계층 간 파일 공유를 위해 프로비저닝된
IOPS SSD(io2) Amazon Elastic Block Store(Amazon EBS) 볼륨을 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q389
회사는 PostgreSQL 단일 AZ DB 인스턴스용 Amazon RDS에 모든 주문을 저장하는 온라인 쇼핑 애플리케이션을 호스팅합니다. 경영진은 단일 실패 지점을 제거하기를 원하며 솔루션 설 계자에게 애플리케이션 코드를 변경하지 않고도 데이터베이스 다운타임을 최소화할 수 있는 접근 방식을 권장하도록 요청했습니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 데이터베이스 인스턴스를 수정하고 다중 AZ 옵션을 지정하여 기존 데이터베이스 인스턴스를 다중 AZ 배포로 변환합니다. 
B. 새로운 RDS 다중 AZ 배포를 생성합니다. 현재 RDS 인스턴스의 스냅샷을 만들고 스냅샷으로 새 다중 AZ 배포를 복원합니다. 
C. 다른 가용 영역에서 PostgreSQL 데이터베이스의 읽기 전용 복제본을 생성합니다. Amazon Route 53 가중 레코드 세트를 사용하여 데이터베이스 전체에 요청을 분산합니다. 
D. 최소 그룹 크기가 2인 Amazon EC2 Auto Scaling 그룹에 RDS for PostgreSQL 데이터베이스를 배치합니다. Amazon Route 53 가중 레코드 세트를 사용하여 인스턴스 간에
요청을 분산합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q390
회사는 여러 AWS 리전 및 계정에 걸쳐 리소스를 보유하고 있습니다. 새로 고용된 솔루션 설계자는 이전 직원이 리소스 인벤토리에 대한 세부 정보를 제공하지 않은 것을 발견했습니다. 솔루션 설계자는 모든 계정에서 다양한 워크로드의 관계 세부 정보를 구축하고 매핑해야 합니다. 운영상 가장 효율적인 방식으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Systems Manager Inventory를 사용하여 상세 보기 보고서에서 맵 보기를 생성합니다. 
B. AWS Step Functions를 사용하여 워크로드 세부 정보를 수집합니다. 워크로드의 아키텍처 다이어그램을 수동으로 작성합니다. 
C. Workload Discovery on AWS를 사용하여 워크로드의 아키텍처 다이어그램을 생성합니다. 
D. AWS X-Ray를 사용하여 워크로드 세부 정보를 봅니다. 관계를 사용하여 아키텍처 다이어그램을 구축합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q391
회사는 들어오는 요청을 처리하는 온프레미스 서버 플릿에서 컨테이너화된 웹 애플리케이션을 호스팅합니다. 요청 수가 빠르게 증가하고 있습니다. 온프레미스 서버는 증가된 요청 수를 처리할 수 없습니다. 이 회사는 최소한의 코드 변경과 최소한의 개발 노력으로 애플리케이션을 AWS로 옮기기를 원합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Elastic Container Service(Amazon ECS)에서 AWS Fargate를 사용하여 Service Auto Scaling으로 컨테이너화된 웹 애플리케이션을 실행합니다. Application
Load Balancer를 사용하여 들어오는 요청을 분산합니다.
B. 두 개의 Amazon EC2 인스턴스를 사용하여 컨테이너화된 웹 애플리케이션을 호스팅합니다. Application Load Balancer를 사용하여 들어오는 요청을 분산합니다. 
C. 지원되는 언어 중 하나를 사용하는 새 코드와 함께 AWS Lambda를 사용합니다. 로드를 지원하는 여러 Lambda 함수를 생성합니다. Amazon API Gateway를 Lambda 함수에 대
한 진입점으로 사용합니다.
D. AWS ParallelCluster와 같은 고성능 컴퓨팅(HPC) 솔루션을 사용하여 적절한 규모로 들어오는 요청을 처리할 수 있는 HPC 클러스터를 설정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q392
회사에서 온프레미스 데이터 센터를 AWS로 마이그레이션하려고 합니다. 데이터 센터는 NFS 기반 파일 시스템에 데이터를 저장하는 SFTP 서버를 호스팅합니다. 서버에는 전송해야 하는 200GB의 데이터가 있습니다. 서버는 Amazon Elastic File System(Amazon EFS) 파일 시스템을 사용하는 Amazon EC2 인스턴스에서 호스팅되어야 합니다. 이 작업을 자동화하기 위해 솔루션 설계자가 수행해야 하는 단계 조합은 무엇입니까? (두 가지를 선택하세요.)
A. EFS 파일 시스템과 동일한 가용 영역에서 EC2 인스턴스를 시작합니다. 
B. 온프레미스 데이터 센터에 AWS DataSync 에이전트를 설치합니다. 
C. 데이터를 위해 EC2 인스턴스에 보조 Amazon Elastic Block Store(Amazon EBS) 볼륨을 생성합니다. 
D. 운영 체제 복사 명령을 수동으로 사용하여 데이터를 EC2 인스턴스로 푸시합니다. 
E. AWS DataSync를 사용하여 온프레미스 SFTP 서버에 적합한 위치 구성을 생성합니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q393
주로 온프레미스에서 애플리케이션 서버를 실행하는 회사가 AWS로 마이그레이션하기로 결정했습니다. 회사는 온프레미스에서 iSCSI(Internet Small Computer Systems Interface) 스토리지를 확장해야 할 필요성을 최소화하려고 합니다. 회사는 최근에 액세스한 데이터만 로컬에 저장하기를 원합니다. 회사는 이러한 요구 사항을 충족하기 위해 어떤 AWS 솔루션을 사용해야 합니까?
A. Amazon S3 파일 게이트웨이 
B. AWS Storage Gateway 테이프 게이트웨이 
C. AWS Storage Gateway 볼륨 게이트웨이 저장 볼륨 
D. AWS Storage Gateway 볼륨 게이트웨이 캐시 볼륨

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q394
회사는 MySQL 데이터베이스를 실행하는 자체 Amazon EC2 인스턴스를 관리합니다. 회사는 수요가 증가하거나 감소함에 따라 복제 및 확장을 수동으로 관리하고 있습니다. 회사는 필요에 따라 데이터베이스 계층에서 컴퓨팅 용량을 추가하거나 제거하는 프로세스를 간소화하는 새로운 솔루션이 필요합니다. 또한 솔루션은 최소한의 운영 노력으로 향상된 성능, 확장성 및 내구성을 제공해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 데이터베이스를 Aurora MySQL용 Amazon Aurora Serverless로 마이그레이션합니다. 
B. 데이터베이스를 Aurora PostgreSQL용 Amazon Aurora Serverless로 마이그레이션합니다. 
C. 데이터베이스를 하나의 더 큰 MySQL 데이터베이스로 결합합니다. 더 큰 EC2 인스턴스에서 더 큰 데이터베이스를 실행합니다. 
D. 데이터베이스 계층에 대한 EC2 Auto Scaling 그룹을 생성합니다. 기존 데이터베이스를 새 환경으로 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q395
이미지 호스팅 회사는 대규모 자산을 Amazon S3 Standard 버킷에 업로드합니다. 회사는 S3 API를 사용하여 멀티파트 업로드를 병렬로 사용하고 동일한 객체가 다시 업로드되면 덮어씁 니다. 업로드 후 처음 30일 동안 개체에 자주 액세스합니다. 개체는 30일 후에 덜 자주 사용되지만 각 개체에 대한 액세스 패턴은 일관되지 않습니다. 회사는 저장된 자산의 고가용성과 탄력성 을 유지하면서 S3 스토리지 비용을 최적화해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자가 권장해야 하는 작업 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 30일 후에 자산을 S3 Intelligent-Tiering으로 이동합니다. 
B. 불완전한 멀티파트 업로드를 정리하도록 S3 수명 주기 정책을 구성합니다. 
C. 만료된 개체 삭제 마커를 정리하도록 S3 수명 주기 정책을 구성합니다. 
D. 30일 후에 자산을 S3 Standard-Infrequent Access(S3 Standard-IA)로 이동합니다. 
E. 30일 후 자산을 S3 One Zone-Infrequent Access(S3 One Zone-IA)로 이동합니다.

<details>
<summary>정답 보기</summary>

**AB**
</details>

---

### Q396
솔루션 설계자는 Amazon S3를 사용하여 새로운 디지털 미디어 애플리케이션의 스토리지 아키텍처를 설계하고 있습니다. 미디어 파일은 가용 영역 손실에 대한 복원력이 있어야 합니다. 일 부 파일은 자주 액세스되는 반면 다른 파일은 예측할 수 없는 패턴으로 거의 액세스되지 않습니다. 솔루션 설계자는 미디어 파일을 저장하고 검색하는 비용을 최소화해야 합니다. 이러한 요구 사항을 충족하는 스토리지 옵션은 무엇입니까?
A. S3 기준
B. S3 지능형 계층화
C. S3 Standard-Infrequent Access(S3 Standard-IA)
D. S3 One Zone-Infrequent Access(S3 One Zone-IA)

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q397
회사는 Application Load Balancer 뒤의 Amazon EC2 인스턴스에서 중요한 비즈니스 애플리케이션을 실행하고 있습니다. EC2 인스턴스는 Auto Scaling 그룹에서 실행되며 Amazon RDS DB 인스턴스에 액세스합니다. EC2 인스턴스와 DB 인스턴스가 모두 단일 가용 영역에 있기 때문에 설계가 운영 검토를 통과하지 못했습니다. 솔루션 설계자는 두 번째 가용 영역을 사용하도록 설계를 업데이트해야 합니다 . 애플리케이션의 가용성을 높이는 솔루션은 무엇입니까?
A. 각 가용 영역에서 서브넷을 프로비저닝합니다. 두 가용 영역에 EC2 인스턴스를 배포하도록 Auto Scaling 그룹을 구성합니다. 각 네트워크에 대한 연결로 DB 인스턴스를 구성합니다. 
B. 두 가용 영역에 걸쳐 확장되는 두 개의 서브넷을 프로비저닝합니다. 두 가용 영역에 EC2 인스턴스를 배포하도록 Auto Scaling 그룹을 구성합니다. 각 네트워크에 대한 연결로 DB 인스
턴스를 구성합니다.
C. 각 가용 영역에서 서브넷을 프로비저닝합니다. 두 가용 영역에 EC2 인스턴스를 배포하도록 Auto Scaling 그룹을 구성합니다. 다중 AZ 배포를 위해 DB 인스턴스를 구성합니다. 
D. 두 가용 영역에 걸쳐 확장되는 서브넷을 프로비저닝합니다. 두 가용 영역에 EC2 인스턴스를 배포하도록 Auto Scaling 그룹을 구성합니다. 다중 AZ 배포를 위해 DB 인스턴스를 구성합
니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q398
회사에는 AWS에서 실행되는 인기 있는 게임 플랫폼이 있습니다. 대기 시간은 사용자 경험에 영향을 미치고 일부 플레이어에게 부당한 이점을 제공할 수 있기 때문에 애플리케이션은 대기 시 간에 민감합니다. 애플리케이션은 모든 AWS 리전에 배포됩니다. Application Load Balancer(ALB) 뒤에 구성된 Auto Scaling 그룹의 일부인 Amazon EC2 인스턴스에서 실행됩니 다. 솔루션 설계자는 애플리케이션의 상태를 모니터링하고 트래픽을 정상 엔드포인트로 리디렉션하는 메커니즘을 구현해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS Global Accelerator에서 액셀러레이터를 구성합니다. 애플리케이션이 청취하는 포트에 대한 리스너를 추가하고 각 리전의 리전 엔드포인트에 연결합니다. ALB를 엔드포인트로
추가하십시오.
B. Amazon CloudFront 배포를 생성하고 ALB를 원본 서버로 지정합니다. 원본 캐시 헤더를 사용하도록 캐시 동작을 구성합니다. AWS Lambda 함수를 사용하여 트래픽을 최적화하십
시오.
C. Amazon CloudFront 배포를 생성하고 Amazon S3를 원본 서버로 지정합니다. 원본 캐시 헤더를 사용하도록 캐시 동작을 구성합니다. AWS Lambda 함수를 사용하여 트래픽을 최
적화하십시오.
D. 애플리케이션의 데이터 저장소 역할을 하도록 Amazon DynamoDB 데이터베이스를 구성합니다. 애플리케이션 데이터를 호스팅하는 DynamoDB의 인 메모리 캐시 역할을 할
DynamoDB Accelerator(DAX) 클러스터를 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q399
회사는 VPC에서 공용 3계층 웹 애플리케이션을 실행합니다. 애플리케이션은 여러 가용 영역의 Amazon EC2 인스턴스에서 실행됩니다. 프라이빗 서브넷에서 실행되는 EC2 인스턴스는 인터넷을 통해 라이선스 서버와 통신해야 합니다. 회사는 운영 유지 보수를 최소화하는 관리형 솔루션이 필요합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 퍼블릭 서브넷에서 NAT 인스턴스를 프로비저닝합니다. NAT 인스턴스를 가리키는 기본 경로로 각 프라이빗 서브넷의 경로 테이블을 수정합니다. 
B. 프라이빗 서브넷에서 NAT 인스턴스를 프로비저닝합니다. NAT 인스턴스를 가리키는 기본 경로로 각 프라이빗 서브넷의 경로 테이블을 수정합니다. 
C. 퍼블릭 서브넷에서 NAT 게이트웨이를 프로비저닝합니다. NAT 게이트웨이를 가리키는 기본 경로로 각 프라이빗 서브넷의 경로 테이블을 수정합니다. 
D. 프라이빗 서브넷에서 NAT 게이트웨이를 프로비저닝합니다. NAT 게이트웨이를 가리키는 기본 경로로 각 프라이빗 서브넷의 경로 테이블을 수정합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q400
한 회사에서 인기 있는 노래 클립으로 만든 벨소리를 판매합니다. 벨소리가 포함된 파일은 Amazon S3 Standard에 저장되며 크기는 128KB 이상입니다. 회사에는 수백만 개의 파일이 있 지만 90일보다 오래된 벨소리의 경우 다운로드가 자주 발생하지 않습니다. 회사는 사용자가 가장 많이 액세스하는 파일을 쉽게 사용할 수 있도록 유지하면서 스토리지 비용을 절감해야 합니다 . 이러한 요구 사항을 가장 비용 효율적으로 충족하기 위해 회사는 어떤 조치를 취해야 합니까?
A. 객체의 초기 스토리지 계층에 대해 S3 Standard-Infrequent Access(S3 Standard-IA) 스토리지를 구성합니다. 
B. 파일을 S3 Intelligent-Tiering으로 이동하고 90일 후에 개체를 더 저렴한 스토리지 계층으로 이동하도록 구성합니다. 
C. 개체를 관리하도록 S3 인벤토리를 구성하고 90일 후에 개체를 S3 Standard-Infrequent Access(S3 Standard-1A)로 이동합니다. 
D. 90일 후에 객체를 S3 Standard에서 S3 Standard-Infrequent Access(S3 Standard-1A)로 이동하는 S3 수명 주기 정책을 구현합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q401
글로벌 회사는 ALB(Application Load Balancer) 뒤의 Amazon EC2 인스턴스에서 웹 애플리케이션을 호스팅합니다. 웹 애플리케이션에는 정적 데이터와 동적 데이터가 있습니다. 회사 는 정적 데이터를 Amazon S3 버킷에 저장합니다. 회사는 정적 데이터 및 동적 데이터의 성능을 개선하고 대기 시간을 줄이려고 합니다. 회사는 Amazon Route 53에 등록된 자체 도메인 이름을 사용하고 있습니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. S3 버킷과 ALB를 원본으로 하는 Amazon CloudFront 배포를 생성합니다. 트래픽을 CloudFront 배포로 라우팅하도록 Route 53을 구성합니다. 
B. ALB를 오리진으로 하는 Amazon CloudFront 배포를 생성합니다. 엔드포인트로 S3 버킷이 있는 AWS Global Accelerator 표준 가속기를 생성합니다. 트래픽을 CloudFront 배
포로 라우팅하도록 Route 53을 구성합니다.
C. S3 버킷을 오리진으로 하는 Amazon CloudFront 배포를 생성합니다. ALB 및 CloudFront 배포를 엔드포인트로 포함하는 AWS Global Accelerator 표준 액셀러레이터를 생성합
니다. 가속기 DNS 이름을 가리키는 사용자 지정 도메인 이름을 만듭니다. 사용자 지정 도메인 이름을 웹 애플리케이션의 엔드포인트로 사용합니다.
D. ALB를 오리진으로 하는 Amazon CloudFront 배포를 생성합니다. S3 버킷을 엔드포인트로 포함하는 AWS Global Accelerator 표준 액셀러레이터를 생성합니다. 두 개의 도메인
이름을 만듭니다. 동적 콘텐츠에 대한 하나의 도메인 이름이 CloudFront DNS 이름을 가리킵니다. 다른 도메인 이름은 정적 콘텐츠에 대한 액셀러레이터 DNS 이름을 가리킵니다. 도메 인 이름을 웹 애플리케이션의 끝점으로 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q402
회사는 Amazon EC2 인스턴스에서 Amazon S3 버킷으로 데이터를 이동해야 합니다. 회사는 API 호출 및 데이터가 공용 인터넷 경로를 통해 라우팅되지 않도록 해야 합니다. EC2 인스 턴스만 S3 버킷에 데이터를 업로드할 수 있는 액세스 권한을 가질 수 있습니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. EC2 인스턴스가 있는 서브넷에서 Amazon S3에 대한 인터페이스 VPC 엔드포인트를 생성합니다. 리소스 정책을 S3 버킷에 연결하여 EC2 인스턴스의 IAM 역할만 액세스하도록 허
용합니다.
B. EC2 인스턴스가 있는 가용 영역에서 Amazon S3에 대한 게이트웨이 VPC 엔드포인트를 생성합니다. 엔드포인트에 적절한 보안 그룹을 연결합니다. 리소스 정책을 S3 버킷에 연결하
여 EC2 인스턴스의 IAM 역할만 액세스하도록 허용합니다.
C. EC2 인스턴스 내부에서 nslookup 도구를 실행하여 S3 버킷 서비스 API 엔드포인트의 프라이빗 IP 주소를 얻습니다. S3 버킷에 대한 액세스 권한을 EC2 인스턴스에 제공하기 위해
VPC 경로 테이블에 경로를 생성합니다. 리소스 정책을 S3 버킷에 연결하여 EC2 인스턴스의 IAM 역할만 액세스하도록 허용합니다.
D. AWS에서 제공하고 공개적으로 사용 가능한 ip-ranges.json 파일을 사용하여 S3 버킷 서비스 API 엔드포인트의 프라이빗 IP 주소를 얻습니다. S3 버킷에 대한 액세스 권한을 EC2
인스턴스에 제공하기 위해 VPC 경로 테이블에 경로를 생성합니다. 리소스 정책을 S3 버킷에 연결하여 EC2 인스턴스의 IAM 역할만 액세스하도록 허용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q403
한 회사에서 AWS에서 호스팅되는 서비스 솔루션으로서 고성능 컴퓨팅(HPC) 워크로드를 구축할 계획입니다. 16개의 Amazon EC2 Linux 인스턴스 그룹은 노드 간 통신을 위해 가능한 가장 낮은 지연 시간이 필요합니다. 인스턴스에는 고성능 스토리지를 위한 공유 블록 장치 볼륨도 필요합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 클러스터 배치 그룹을 사용하십시오. Amazon EBS 다중 연결을 사용하여 단일 프로비저닝된 IOPS SSD Amazon Elastic Block Store(Amazon EBS) 볼륨을 모든 인스턴스에
연결합니다.
B. 클러스터 배치 그룹을 사용하십시오. Amazon Elastic File System(Amazon EFS)을 사용하여 인스턴스 간에 공유 파일 시스템을 생성합니다. 
C. 파티션 배치 그룹을 사용하십시오. Amazon Elastic File System(Amazon EFS)을 사용하여 인스턴스 간에 공유 파일 시스템을 생성합니다. 
D. 스프레드 배치 그룹을 사용하십시오. Amazon EBS 다중 연결을 사용하여 단일 프로비저닝된 IOPS SSD Amazon Elastic Block Store(Amazon EBS) 볼륨을 모든 인스턴스에
연결합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q404
회사에서 데이터 관리 애플리케이션을 AWS로 이전하고 있습니다. 회사는 이벤트 기반 아키텍처로 전환하려고 합니다. 아키텍처는 워크플로의 다양한 측면을 수행하면서 더 많이 분산되고 서 버리스 개념을 사용해야 합니다. 회사는 또한 운영 오버헤드를 최소화하기를 원합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Glue에서 워크플로를 구축합니다. AWS Glue를 사용하여 AWS Lambda 함수를 호출하여 워크플로 단계를 처리합니다. 
B. AWS Step Functions에서 워크플로를 구축합니다. Amazon EC2 인스턴스에 애플리케이션을 배포합니다. Step Functions를 사용하여 EC2 인스턴스에서 워크플로 단계를 호출
합니다.
C. Amazon EventBridge에서 워크플로를 구축합니다. EventBridge를 사용하여 일정에 따라 AWS Lambda 함수를 호출하여 워크플로 단계를 처리합니다. 
D. AWS Step Functions에서 워크플로를 구축합니다. Step Functions를 사용하여 상태 머신을 생성합니다. 상태 시스템을 사용하여 AWS Lambda 함수를 호출하여 워크플로 단계
를 처리합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q405
회사는 여러 벤더를 사용하여 Amazon S3 버킷에 저장된 디지털 자산을 배포합니다. 이 회사는 벤더 AWS 계정이 이러한 S3 버킷에서 객체를 다운로드하는 데 필요한 최소한의 액세스 권 한을 갖도록 하려고 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 익명의 읽기 권한과 모든 버킷을 나열할 수 있는 권한이 있는 버킷 정책을 설계합니다. 
B. 사용자에게 읽기 전용 액세스 권한을 부여하는 버킷 정책을 설계합니다. IAM 엔터티를 보안 주체로 지정합니다. 
C. IAM 역할에 대해 지정된 읽기 전용 액세스 정책이 있는 교차 계정 IAM 역할을 생성합니다. 
D. 공급업체 사용자에게 읽기 전용 액세스 권한을 부여하는 사용자 정책 및 공급업체 사용자 그룹을 만듭니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q406
회사에서 API로 구동되는 클라우드 통신 플랫폼을 설계하고 있습니다. 애플리케이션은 NLB(Network Load Balancer) 뒤의 Amazon EC2 인스턴스에서 호스팅됩니다. 이 회사는 Amazon API Gateway를 사용하여 외부 사용자에게 API를 통해 애플리케이션에 대한 액세스 권한을 제공합니다. 이 회사는 SQL 인젝션과 같은 웹 익스플로잇으로부터 플랫폼을 보호하 고 대규모의 정교한 DDoS 공격을 감지하고 완화하기를 원합니다. 어떤 솔루션 조합이 MOST 보호를 제공합니까? (두 가지를 선택하세요.)
A. AWS WAF를 사용하여 NLB를 보호하십시오. 
B. NLB와 함께 AWS Shield Advanced를 사용합니다. 
C. AWS WAF를 사용하여 Amazon API Gateway를 보호합니다. 
D. AWS Shield Standard와 함께 Amazon GuardDuty 사용 
E. Amazon API Gateway와 함께 AWS Shield Standard를 사용합니다.

<details>
<summary>정답 보기</summary>

**BC**
</details>

---

### Q407
솔루션 설계자는 Windows 인터넷 정보 서비스(IIS) 웹 애플리케이션을 AWS로 마이그레이션해야 합니다. 애플리케이션은 현재 사용자의 온프레미스 NAS(Network-Attached Storage)에서 호스팅되는 파일 공유에 의존합니다. 솔루션 설계자는 IIS 웹 서버를 스토리지 솔루션에 연결된 여러 가용 영역의 Amazon EC2 인스턴스로 마이그레이션하고 인스턴스에 연 결된 Elastic Load Balancer를 구성할 것을 제안했습니다. 온프레미스 파일 공유에 대한 어떤 대체가 가장 탄력적이고 내구성이 있습니까?
A. 파일 공유를 Amazon RDS로 마이그레이션합니다. 
B. 파일 공유를 AWS Storage Gateway로 마이그레이션합니다. 
C. 파일 공유를 Amazon FSx for Windows File Server로 마이그레이션합니다. 
D. 파일 공유를 Amazon Elastic File System(Amazon EFS)으로 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q408
전자 상거래 회사는 Amazon RDS 기반 웹 애플리케이션의 성능 저하를 발견했습니다. 성능 저하의 원인은 비즈니스 분석가가 트리거하는 읽기 전용 SQL 쿼리 수가 증가했기 때문입니다. 솔루션 설계자는 기존 웹 애플리케이션에 대한 최소한의 변경으로 문제를 해결해야 합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. 데이터를 Amazon DynamoDB로 내보내고 비즈니스 분석가가 쿼리를 실행하도록 합니다. 
B. Amazon ElastiCache에 데이터를 로드하고 비즈니스 분석가가 쿼리를 실행하도록 합니다. 
C. 기본 데이터베이스의 읽기 복제본을 생성하고 비즈니스 분석가가 쿼리를 실행하도록 합니다. 
D. 데이터를 Amazon Redshift 클러스터로 복사하고 비즈니스 분석가가 쿼리를 실행하도록 합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q409
빠르게 성장하고 있는 음식 배달 서비스를 제공하는 회사가 있습니다. 성장으로 인해 회사의 주문 처리 시스템은 최대 트래픽 시간 동안 확장 문제를 겪고 있습니다. 현재 아키텍처에는 다음이 포함됩니다. * 애플리케이션에서 주문을 수집하기 위해 Amazon EC2 Auto Scaling 그룹에서 실행되는 Amazon EC2 인스턴스 그룹 * 주문을 이행하기 위해 Amazon EC2 Auto Scaling 그룹에서 실행되는 다른 EC2 인스턴스 그룹 주문 수집 프로세스는 빠르게 진행되지만 주문 이행 프로세스는 더 오래 걸릴 수 있습니다. 스케일링 이벤트로 인해 데이터가 손실되어서는 안 됩니다. 솔루션 설계자는 주문 수집 프로세스와 주문 이행 프로세스가 트래픽이 가장 많은 시간에 적절하게 확장될 수 있는지 확인해야 합니다. 솔루션은 회사의 AWS 리소스 활용을 최적화해야 합니 다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon CloudWatch 지표를 사용하여 Auto Scaling 그룹에 있는 각 인스턴스의 CPU를 모니터링합니다. 최대 워크로드 값에 따라 각 Auto Scaling 그룹의 최소 용량을 구성합니
다.
B. Amazon CloudWatch 지표를 사용하여 Auto Scaling 그룹에 있는 각 인스턴스의 CPU를 모니터링합니다. 요청 시 추가 Auto Scaling 그룹을 생성하는 Amazon Simple
Notification Service(Amazon SNS) 주제를 호출하도록 CloudWatch 경보를 구성합니다.
C. 두 개의 Amazon Simple Queue Service(Amazon SQS) 대기열을 프로비저닝합니다. 하나는 주문 수집용이고 다른 하나는 주문 이행용입니다. 각 대기열을 폴링하도록 EC2 인스
턴스를 구성합니다. 대기열이 보내는 알림을 기반으로 Auto Scaling 그룹을 조정합니다.
D. 2개의 Amazon Simple Queue Service(Amazon SQS) 대기열을 프로비저닝합니다. 하나는 주문 수집용이고 다른 하나는 주문 이행용입니다. 각 대기열을 폴링하도록 EC2 인스
턴스를 구성합니다. 인스턴스 계산당 백로그를 기반으로 지표를 만듭니다. 이 지표를 기반으로 Auto Scaling 그룹을 조정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q410
소셜 미디어 회사는 사용자가 웹 사이트에 이미지를 업로드할 수 있도록 합니다. 웹 사이트는 Amazon EC2 인스턴스에서 실행됩니다. 업로드 요청 중에 웹 사이트는 이미지 크기를 표준 크 기로 조정하고 크기 조정된 이미지를 Amazon S3에 저장합니다. 사용자가 웹 사이트에 대한 느린 업로드 요청을 경험하고 있습니다. 회사는 애플리케이션 내 결합을 줄이고 웹 사이트 성능을 개선해야 합니다. 솔루션 설계자는 이미지 업로드를 위해 운영상 가장 효율적인 프로세스를 설계해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 작업 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. S3 Glacier에 이미지를 업로드하도록 애플리케이션을 구성합니다. 
B. 원본 이미지를 Amazon S3에 업로드하도록 웹 서버를 구성합니다. 
C. 미리 서명된 URL을 사용하여 각 사용자의 브라우저에서 Amazon S3로 직접 이미지를 업로드하도록 애플리케이션을 구성합니다. 
D. 이미지가 업로드될 때 AWS Lambda 함수를 호출하도록 S3 이벤트 알림을 구성합니다. 기능을 사용하여 이미지 크기를 조정하십시오. 
E. 업로드된 이미지의 크기를 조정하기 위해 일정에 따라 AWS Lambda 함수를 호출하는 Amazon EventBridge(Amazon CloudWatch Events) 규칙을 생성합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q411
회사는 AWS 클라우드에서 호스팅되는 게임 애플리케이션을 위한 공유 스토리지 솔루션을 설계하고 있습니다. 회사는 SMB 클라이언트를 사용하여 데이터에 액세스할 수 있는 기능이 필요합 니다. 솔루션은 완전히 관리되어야 합니다. 어떤 AWS 솔루션이 이러한 요구 사항을 충족합니까?
A. 탑재 가능한 파일 시스템으로 데이터를 공유하는 AWS DataSync 작업을 생성합니다. 파일 시스템을 애플리케이션 서버에 마운트하십시오. 
B. Amazon EC2 Windows 인스턴스를 생성합니다. 인스턴스에 Windows 파일 공유 역할을 설치하고 구성합니다. 응용 프로그램 서버를 파일 공유에 연결합니다. 
C. Windows 파일 서버 파일 시스템용 Amazon FSx를 생성합니다. 원본 서버에 파일 시스템을 연결합니다. 애플리케이션 서버를 파일 시스템에 연결하십시오. 
D. Amazon S3 버킷을 생성합니다. 애플리케이션에 IAM 역할을 할당하여 S3 버킷에 대한 액세스 권한을 부여합니다. S3 버킷을 애플리케이션 서버에 마운트합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q412
회사에서 보고용으로 50TB의 데이터를 사용합니다. 회사는 이 데이터를 온프레미스에서 AWS로 이동하려고 합니다. 회사 데이터 센터의 맞춤형 애플리케이션은 매주 데이터 변환 작업을 실 행합니다. 회사는 데이터 전송이 완료될 때까지 애플리케이션을 일시 중지할 계획이며 가능한 한 빨리 전송 프로세스를 시작해야 합니다. 데이터 센터에는 추가 워크로드에 사용할 수 있는 네트워크 대역폭이 없습니다. 솔루션 설계자는 데이터를 전송하고 변환 작업이 AWS 클라우드에서 계속 실행되도록 구성해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS DataSync를 사용하여 데이터를 이동하십시오. AWS Glue를 사용하여 사용자 지정 변환 작업을 생성합니다. 
B. 데이터를 이동할 AWS Snowcone 디바이스를 주문합니다. 장치에 변환 응용 프로그램을 배포합니다. 
C. AWS Snowball Edge Storage Optimized 디바이스를 주문합니다. 데이터를 장치에 복사합니다. AWS Glue를 사용하여 사용자 지정 변환 작업을 생성합니다. 
D. Amazon EC2 컴퓨팅을 포함하는 AWS Snowball Edge Storage Optimized 디바이스를 주문합니다. 데이터를 장치에 복사합니다. AWS에서 새 EC2 인스턴스를 생성하여 변환
애플리케이션을 실행합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q413
회사는 가까운 장래에 급속한 성장을 기대하고 있습니다. 솔루션 설계자는 기존 사용자를 구성하고 AWS에서 새 사용자에게 권한을 부여해야 합니다. 솔루션 설계자는 IAM 그룹을 만들기로 결정했습니다. 솔루션 설계자는 부서를 기반으로 IAM 그룹에 새 사용자를 추가합니다. 새 사용자에게 권한을 부여하는 가장 안전한 추가 작업은 무엇입니까?
A. 서비스 제어 정책(SCP)을 적용하여 액세스 권한 관리 
B. 최소 권한이 있는 IAM 역할을 생성합니다. IAM 그룹에 역할 연결 
C. 최소 권한을 부여하는 IAM 정책을 생성합니다. 정책을 IAM 그룹에 연결 
D. IAM 역할을 생성합니다. 최대 권한을 정의하는 권한 경계와 역할 연결

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q414
회사는 Application Load Balancer 뒤의 Amazon EC2 인스턴스에서 글로벌 웹 애플리케이션을 실행합니다. 애플리케이션은 Amazon Aurora에 데이터를 저장합니다. 회사는 재해 복 구 솔루션을 만들어야 하며 최대 30분의 다운타임과 잠재적인 데이터 손실을 허용할 수 있습니다. 솔루션은 기본 인프라가 정상일 때 부하를 처리할 필요가 없습니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 필요한 인프라 요소가 있는 애플리케이션을 배치합니다. Amazon Route 53을 사용하여 활성-수동 장애 조치를 구성합니다. 두 번째 AWS 리전에서 Aurora 복제본을 생성합니다. 
B. 두 번째 AWS 리전에서 애플리케이션의 축소된 배포를 호스팅합니다. Amazon Route 53을 사용하여 활성-활성 장애 조치를 구성합니다. 두 번째 리전에서 Aurora 복제본을 생성합니
다.
C. 두 번째 AWS 리전에서 기본 인프라를 복제합니다. Amazon Route 53을 사용하여 활성-활성 장애 조치를 구성합니다. 최신 스냅샷에서 복원된 Aurora 데이터베이스를 생성합니다. 
D. AWS Backup으로 데이터를 백업합니다. 백업을 사용하여 두 번째 AWS 리전에 필요한 인프라를 생성합니다. Amazon Route 53을 사용하여 활성-수동 장애 조치를 구성합니다. 두
번째 리전에서 Aurora 두 번째 기본 인스턴스를 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q415
한 회사가 AWS에서 자체 관리형 DNS 서비스를 구현했습니다. 이 솔루션은 다음으로 구성됩니다. * 서로 다른 AWS 리전의 Amazon EC2 인스턴스 * AWS Global Accelerator의 표준 가속기 엔드포인트 회사는 DDoS 공격으로부터 솔루션을 보호하려고 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS Shield Advanced에 가입하십시오. 보호할 리소스로 액셀러레이터를 추가합니다. 
B. AWS Shield Advanced에 가입합니다. 보호할 리소스로 EC2 인스턴스를 추가합니다. 
C. 속도 기반 규칙을 포함하는 AWS WAF 웹 ACL을 생성합니다. 웹 ACL을 가속기와 연결합니다. 
D. 비율 기반 규칙을 포함하는 AWS WAF 웹 ACL을 생성합니다. 웹 ACL을 EC2 인스턴스와 연결합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q416
의료 기록 회사는 Amazon EC2 인스턴스에서 애플리케이션을 호스팅하고 있습니다. 애플리케이션은 Amazon S3에 저장된 고객 데이터 파일을 처리합니다. EC2 인스턴스는 퍼블릭 서브 넷에서 호스팅됩니다. EC2 인스턴스는 인터넷을 통해 Amazon S3에 액세스하지만 다른 네트워크 액세스는 필요하지 않습니다. 새로운 요구 사항은 파일 전송을 위한 네트워크 트래픽이 개인 경로를 사용하고 인터넷을 통해 전송되지 않도록 요구합니다. 솔루션 설계자가 이 요구 사항을 충족하기 위해 권장해야 하는 네트워크 아키텍처 변경 사항은 무엇입니까?
A. NAT 게이트웨이를 생성합니다. NAT 게이트웨이를 통해 트래픽을 Amazon S3로 보내도록 퍼블릭 서브넷에 대한 라우팅 테이블을 구성합니다. 
B. S3 접두사 목록에 대한 트래픽만 허용되도록 아웃바운드 트래픽을 제한하도록 EC2 인스턴스에 대한 보안 그룹을 구성합니다. 
C. EC2 인스턴스를 프라이빗 서브넷으로 이동합니다. Amazon S3에 대한 VPC 엔드포인트를 생성하고 엔드포인트를 프라이빗 서브넷의 라우팅 테이블에 연결합니다. 
D. VPC에서 인터넷 게이트웨이를 제거합니다. AWS Direct Connect 연결을 설정하고 Direct Connect 연결을 통해 트래픽을 Amazon S3로 라우팅합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q417
한 회사는 최근 Amazon EC2 인스턴스에 대해 운영 체제 버전, 패치 및 설치된 소프트웨어에 대한 정보를 중앙 집중화하기 위해 새로운 감사 시스템을 배포했습니다. 솔루션 설계자는 EC2 Auto Scaling 그룹을 통해 프로비저닝된 모든 인스턴스가 시작 및 종료되는 즉시 성공적으로 감사 시스템에 보고서를 보내도록 해야 합니다. 이러한 목표를 가장 효율적으로 달성하는 솔루션은 무엇입니까?
A. 예약된 AWS Lambda 함수를 사용하고 모든 EC2 인스턴스에서 원격으로 스크립트를 실행하여 데이터를 감사 시스템으로 보냅니다. 
B. EC2 Auto Scaling 수명 주기 후크를 사용하여 인스턴스가 시작되고 종료될 때 감사 시스템에 데이터를 보내는 사용자 지정 스크립트를 실행합니다. 
C. EC2 Auto Scaling 시작 구성을 사용하여 사용자 데이터를 통해 사용자 지정 스크립트를 실행하여 인스턴스가 시작되고 종료될 때 감사 시스템에 데이터를 보냅니다. 
D. 인스턴스 운영 체제에서 사용자 지정 스크립트를 실행하여 데이터를 감사 시스템으로 보냅니다. 인스턴스가 시작되고 종료될 때 EC2 Auto Scaling 그룹에서 호출할 스크립트를 구성합
니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q418
회사는 Application Load Balancer(ALB) 뒤에 있는 Amazon EC2 인스턴스에서 웹 사이트를 호스팅합니다. 웹 사이트는 정적 콘텐츠를 제공합니다. 웹 사이트 트래픽이 증가하고 있으 며 회사는 잠재적인 비용 증가에 대해 우려하고 있습니다. 웹사이트 비용을 줄이기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. Amazon CloudFront 배포를 생성하여 엣지 위치에서 정적 파일을 캐싱합니다. 
B. Amazon ElastiCache 클러스터를 생성합니다. ALB를 ElastiCache 클러스터에 연결하여 캐싱된 파일을 제공합니다. 
C. AWS WAF 웹 ACL을 생성하고 ALB와 연결합니다. 웹 ACL에 규칙을 추가하여 정적 파일을 캐시합니다. 
D. 대체 AWS 리전에서 두 번째 ALB를 생성합니다. 사용자 트래픽을 가장 가까운 리전으로 라우팅하여 데이터 전송 비용을 최소화합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q419
회사는 AWS에서 온라인 마켓플레이스 웹 애플리케이션을 실행합니다. 이 응용 프로그램은 피크 시간 동안 수십만 명의 사용자에게 서비스를 제공합니다. 이 회사는 수백만 건의 금융 거래 세 부 정보를 다른 여러 내부 애플리케이션과 공유하기 위해 확장 가능한 실시간에 가까운 솔루션이 필요합니다. 짧은 대기 시간 검색을 위해 문서 데이터베이스에 저장되기 전에 민감한 데이터를 제거하기 위해 트랜잭션을 처리해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. 트랜잭션 데이터를 Amazon DynamoDB에 저장합니다. 쓰기 시 모든 트랜잭션에서 중요한 데이터를 제거하도록 DynamoDB에서 규칙을 설정합니다. DynamoDB Streams를 사
용하여 트랜잭션 데이터를 다른 애플리케이션과 공유합니다.
B. 트랜잭션 데이터를 Amazon Kinesis Data Firehose로 스트리(cid:1535)하여 Amazon DynamoDB 및 Amazon S3에 데이터를 저장합니다. Kinesis Data Firehose와 AWS
Lambda 통합을 사용하여 민감한 데이터를 제거합니다. 다른 애플리케이션은 Amazon S3에 저장된 데이터를 사용할 수 있습니다.
C. 트랜잭션 데이터를 Amazon Kinesis Data Streams로 스트리(cid:1535)합니다. AWS Lambda 통합을 사용하여 모든 트랜잭션에서 민감한 데이터를 제거한 다음 트랜잭션 데이터를
Amazon DynamoDB에 저장합니다. 다른 애플리케이션은 Kinesis 데이터 스트림 외부에서 트랜잭션 데이터를 사용할 수 있습니다.
D. 배치 트랜잭션 데이터를 Amazon S3에 파일로 저장합니다. Amazon S3에서 파일을 업데이트하기 전에 AWS Lambda를 사용하여 모든 파일을 처리하고 민감한 데이터를 제거하십
시오. 그런 다음 Lambda 함수는 Amazon DynamoDB에 데이터를 저장합니다. 다른 애플리케이션은 Amazon S3에 저장된 트랜잭션 파일을 사용할 수 있습니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q420
회사에서 Oracle 데이터베이스를 AWS로 마이그레이션하려고 합니다. 데이터베이스는 지리 코드로 식별되는 고해상도 지리 정보 시스템(GIS) 이미지 수백만 개가 포함된 단일 테이블로 구 성됩니다. 자연 재해가 발생하면 몇 분마다 수만 개의 이미지가 업데이트됩니다. 각 지리적 코드에는 연결된 단일 이미지 또는 행이 있습니다. 회사는 이러한 이벤트 중에 가용성과 확장성이 뛰어난 솔루 션을 원합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 이미지와 지리적 코드를 데이터베이스 테이블에 저장합니다. Amazon RDS 다중 AZ DB 인스턴스에서 실행되는 Oracle을 사용합니다. 
B. Amazon S3 버킷에 이미지를 저장합니다. 지리적 코드를 키로, 이미지 S3 URL을 값으로 사용하여 Amazon DynamoDB를 사용합니다. 
C. Amazon DynamoDB 테이블에 이미지와 지리적 코드를 저장합니다. 부하가 높은 시간 동안 DynamoDB Accelerator(DAX)를 구성합니다. 
D. Amazon S3 버킷에 이미지를 저장합니다. 지리 코드와 이미지 S3 URL을 데이터베이스 테이블에 저장합니다. Amazon RDS 다중 AZ DB 인스턴스에서 실행되는 Oracle을 사용합
니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q421
회사는 AWS에서 워크로드를 실행합니다. 회사는 외부 공급자의 서비스에 연결해야 합니다. 서비스는 공급자의 VPC에서 호스팅됩니다. 회사의 보안 팀에 따르면 연결은 비공개여야 하며 대 상 서비스로 제한되어야 합니다. 연결은 회사의 VPC에서만 시작되어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 회사의 VPC와 공급자의 VPC 간에 VPC 피어링 연결을 생성합니다. 대상 서비스에 연결하도록 라우팅 테이블을 업데이트합니다. 
B. 공급자에게 VPC에 가상 프라이빗 게이트웨이를 생성하도록 요청하십시오. AWS PrivateLink를 사용하여 대상 서비스에 연결합니다. 
C. 대상 서비스에 연결하기 위해 회사의 VPUpdate 라우팅 테이블의 퍼블릭 서브넷에 NAT 게이트웨이를 생성합니다. 
D. 공급자에게 대상 서비스에 대한 VPC 끝점을 생성하도록 요청하십시오. AWS PrivateLink를 사용하여 대상 서비스에 연결합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q422
회사는 Amazon EC2 인스턴스에서 배치 애플리케이션을 실행하고 있습니다. 애플리케이션은 여러 Amazon RDS 데이터베이스가 있는 백엔드로 구성됩니다. 응용 프로그램으로 인해 데 이터베이스에서 많은 수의 읽기가 발생하고 있습니다. 솔루션 설계자는 고가용성을 보장하면서 데이터베이스 읽기 수를 줄여야 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Amazon RDS 읽기 전용 복제본을 추가합니다. 
B. Redis용 Amazon ElastiCache를 사용합니다. 
C. Amazon Route 53 DNS 캐싱 사용 
D. Memcached용 Amazon ElastiCache를 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q423
회사는 AWS에서 서버리스 애플리케이션을 호스팅합니다. 이 애플리케이션은 Amazon API Gateway, AWS Lambda 및 Amazon RDS for PostgreSQL 데이터베이스를 사용합니 다. 회사는 최대 트래픽 또는 예측할 수 없는 트래픽 시간 동안 데이터베이스 연결 시간 초과로 인해 발생하는 애플리케이션 오류의 증가를 확인했습니다. 회사는 최소한의 코드 변경으로 애플 리케이션 오류를 줄이는 솔루션이 필요합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Lambda 동시성 비율을 줄입니다. 
B. RDS DB 인스턴스에서 RDS 프록시를 활성화합니다. 
C. 더 많은 연결을 허용하도록 RDS DB 인스턴스 클래스의 크기를 조정합니다. 
D. 온디맨드 확장을 통해 데이터베이스를 Amazon DynamoDB로 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q424
한 회사에 단일 AWS 리전에서 실행되는 리전 구독 기반 스트리(cid:1535) 서비스가 있습니다. 아키텍처는 Amazon EC2 인스턴스의 웹 서버와 애플리케이션 서버로 구성됩니다. EC2 인스턴스는 Elastic Load Balancer 뒤의 Auto Scaling 그룹에 있습니다. 아키텍처에는 여러 가용 영역에 걸쳐 확장되는 Amazon Aurora 글로벌 데이터베이스 클러스터가 포함됩니다. 이 회사는 전 세계적으로 확장하고 응용 프로그램의 가동 중지 시간을 최소화하기를 원합니다. 어떤 솔루션이 가장 내결함성을 제공합니까?
A. 웹 계층 및 애플리케이션 계층에 대한 Auto Scaling 그룹을 확장하여 두 번째 리전의 가용 영역에 인스턴스를 배포합니다. Aurora 글로벌 데이터베이스를 사용하여 기본 리전과 두 번째
리전에 데이터베이스를 배포합니다. 두 번째 리전에 대한 장애 조치 라우팅 정책과 함께 Amazon Route 53 상태 확인을 사용합니다.
B. 웹 계층과 애플리케이션 계층을 두 번째 리전에 배포합니다. 두 번째 리전에 Aurora PostgreSQL 교차 리전 Aurora 복제본을 추가합니다. 두 번째 리전에 대한 장애 조치 라우팅 정책
과 함께 Amazon Route 53 상태 확인을 사용합니다. 필요에 따라 보조를 기본으로 승격합니다.
C. 웹 계층과 애플리케이션 계층을 두 번째 리전에 배포합니다. 두 번째 리전에서 Aurora PostgreSQL 데이터베이스를 생성합니다. AWS Database Migration Service(AWS
DMS)를 사용하여 기본 데이터베이스를 두 번째 리전에 복제합니다. 두 번째 리전에 대한 장애 조치 라우팅 정책과 함께 Amazon Route 53 상태 확인을 사용합니다.
D. 웹 계층과 애플리케이션 계층을 두 번째 지역에 배포합니다. Amazon Aurora 글로벌 데이터베이스를 사용하여 기본 리전과 두 번째 리전에 데이터베이스를 배포합니다. 두 번째 리전에
대한 장애 조치 라우팅 정책과 함께 Amazon Route 53 상태 확인을 사용합니다. 필요에 따라 보조를 기본으로 승격합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q425
회사에는 AWS Lake Formation에서 관리하는 Amazon S3 데이터 레이크가 있습니다. 이 회사는 데이터 레이크의 데이터를 Amazon Aurora MySQL 데이터베이스에 저장된 운영 데 이터와 결합하여 Amazon QuickSight에서 시각화를 생성하려고 합니다. 회사는 회사의 마케팅 팀이 데이터베이스의 열 하위 집합에만 액세스할 수 있도록 열 수준 권한을 적용하려고 합니 다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon EMR을 사용하여 데이터베이스에서 QuickSight SPICE 엔진으로 직접 데이터를 수집하십시오. 필요한 열만 포함합니다. 
B. AWS Glue Studio를 사용하여 데이터베이스에서 S3 데이터 레이크로 데이터를 수집합니다. IAM 정책을 QuickSight 사용자에게 연결하여 열 수준 액세스 제어를 적용합니다.
QuickSight에서 Amazon S3를 데이터 원본으로 사용합니다.
C. AWS Glue Elastic Views를 사용하여 Amazon S3의 데이터베이스에 대한 구체화된 보기를 생성합니다. QuickSight 사용자에 대한 열 수준 액세스 제어를 적용하려면 S3 버킷 정
책을 생성합니다. QuickSight에서 Amazon S3를 데이터 원본으로 사용합니다.
D. Lake Formation 청사진을 사용하여 데이터베이스에서 S3 데이터 레이크로 데이터를 수집합니다. Lake Formation을 사용하여 QuickSight 사용자에 대한 열 수준 액세스 제어를
적용합니다. QuickSight에서 Amazon Athena를 데이터 원본으로 사용합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q426
회사는 Application Load Balancer 뒤의 Amazon EC2 인스턴스에서 전자상거래 애플리케이션을 실행합니다. 인스턴스는 여러 가용 영역에 걸쳐 Amazon EC2 Auto Scaling 그룹 에서 실행됩니다. Auto Scaling 그룹은 CPU 사용률 지표를 기반으로 확장됩니다. 전자 상거래 애플리케이션은 대규모 EC2 인스턴스에서 호스팅되는 MySQL 8.0 데이터베이스에 트랜잭 션 데이터를 저장합니다. 애플리케이션 로드가 증가하면 데이터베이스 성능이 빠르게 저하됩니다. 애플리케이션은 쓰기 트랜잭션보다 더 많은 읽기 요청을 처리합니다. 회사는 고가용성을 유지하면서 예측할 수 없는 읽 기 워크로드의 수요를 충족하기 위해 데이터베이스를 자동으로 확장하는 솔루션을 원합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 리더 및 컴퓨팅 기능을 위해 단일 노드와 함께 Amazon Redshift를 사용하십시오. 
B. 단일 AZ 배포와 함께 Amazon RDS 사용 Amazon RDS를 구성하여 다른 가용 영역에 리더 인스턴스를 추가합니다. 
C. 다중 AZ 배포와 함께 Amazon Aurora를 사용합니다. Aurora 복제본으로 Aurora Auto Scaling을 구성합니다. 
D. EC2 스팟 인스턴스와 함께 Memcached용 Amazon ElastiCache를 사용합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q427
회사에서 온프레미스 Oracle 데이터베이스를 Amazon Aurora PostgreSQL로 이전하고 있습니다. 데이터베이스에는 동일한 테이블에 쓰는 여러 응용 프로그램이 있습니다. 응용 프로그 램은 각 마이그레이션 사이에 한 달씩 하나씩 마이그레이션해야 합니다. 경영진은 데이터베이스에 많은 수의 읽기 및 쓰기가 있다는 우려를 표명했습니다. 데이터는 마이그레이션하는 동안 두 데이터베이스에서 동기화 상태를 유지해야 합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. 초기 마이그레이션에는 AWS DataSync를 사용하십시오. AWS Database Migration Service(AWS DMS)를 사용하여 변경 데이터 캡처(CDC) 복제 작업 및 테이블 매핑을 생
성하여 모든 테이블을 선택합니다.
B. 초기 마이그레이션에 AWS DataSync를 사용합니다. AWS Database Migration Service(AWS DMS)를 사용하여 전체 로드 및 변경 데이터 캡처(CDC) 복제 작업과 테이블 매
핑을 생성하여 모든 테이블을 선택합니다.
C. 메모리 최적화 복제 인스턴스를 사용하여 AWS DMS(AWS Database Migration Service)와 함께 AWS Schema Conversion Tool을 사용합니다. 전체 로드 및 CDC(변경 데
이터 캡처) 복제 작업과 테이블 매핑을 생성하여 모든 테이블을 선택합니다.
D. 컴퓨팅 최적화 복제 인스턴스를 사용하여 AWS DMS(AWS Database Migration Service)와 함께 AWS Schema Conversion Tool을 사용합니다. 전체 로드 및 변경 데이터
캡처(CDC) 복제 작업과 테이블 매핑을 생성하여 가장 큰 테이블을 선택합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q428
개발 팀이 개발 VPC 내부의 Amazon EC2 인스턴스에서 호스팅되는 새로운 애플리케이션을 출시했습니다. 솔루션 설계자는 동일한 계정에 새 VPC를 생성해야 합니다. 새 VPC는 개발 VPC와 피어링됩니다. 개발용 VPC의 VPC CIDR 블록은 192.168.0.0/24입니다. 솔루션 설계자는 새 VPC에 대한 CIDR 블록을 생성해야 합니다. CIDR 블록은 개발 VPC에 대한 VPC 피어링 연결에 대해 유효해야 합니다. 이러한 요구 사항을 충족하는 가장 작은 CIDR 블록은 무엇입니까?
A. 10.0.1.0/32 
B. 192.168.0.0/24 
C. 192.168.1.0/32 
D. 10.0.1.0/24

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q429
회사에서 다중 계층 웹 애플리케이션에 Amazon ElastiCache를 사용할 계획입니다. 솔루션 설계자는 ElastiCache 클러스터용 캐시 VPC와 애플리케이션의 Amazon EC2 인스턴스용 앱 VPC를 생성합니다. 두 VPC 모두 us-east-1 리전에 있습니다. 솔루션 설계자는 애플리케이션의 EC2 인스턴스에 ElastiCache 클러스터에 대한 액세스 권한을 제공하는 솔루션을 구현해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. VPC 간에 피어링 연결을 생성합니다. 두 VPC 모두에서 피어링 연결을 위한 라우팅 테이블 항목을 추가합니다. 애플리케이션의 보안 그룹에서 인바운드 연결을 허용하도록
ElastiCache 클러스터의 보안 그룹에 대한 인바운드 규칙을 구성합니다.
B. 전송 VPC를 생성합니다. 전송 VPC를 통해 트래픽을 라우팅하도록 캐시 VPC 및 앱 VPC의 VPC 라우팅 테이블을 업데이트합니다. 애플리케이션의 보안 그룹에서 인바운드 연결을 허
용하도록 ElastiCache 클러스터의 보안 그룹에 대한 인바운드 규칙을 구성합니다.
C. VPC 간에 피어링 연결을 생성합니다. 두 VPC 모두에서 피어링 연결을 위한 라우팅 테이블 항목을 추가합니다. 애플리케이션의 보안 그룹에서 인바운드 연결을 허용하도록 피어링 연결
의 보안 그룹에 대한 인바운드 규칙을 구성합니다.
D. 전송 VPC를 생성합니다. 전송 VPC를 통해 트래픽을 라우팅하도록 캐시 VPC 및 앱 VPC의 VPC 라우팅 테이블을 업데이트합니다. 애플리케이션의 보안 그룹에서 인바운드 연결을 허
용하도록 Transit VPC의 보안 그룹에 대한 인바운드 규칙을 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q430
회사에서 Windows 컨테이너 아래의 .NET 6 Framework에서 실행되는 Windows 작업을 컨테이너화했습니다. 회사는 AWS 클라우드에서 이 작업을 실행하려고 합니다. 작업은 10분 마다 실행됩니다. 작업의 실행 시간은 1분에서 3분 사이입니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 작업의 컨테이너 이미지를 기반으로 AWS Lambda 함수를 생성합니다. 10분마다 함수를 호출하도록 Amazon EventBridge를 구성합니다. 
B. AWS Batch를 사용하여 AWS Fargate 리소스를 사용하는 작업을 생성합니다. 10분마다 실행되도록 작업 일정을 구성합니다. 
C. AWS Fargate에서 Amazon Elastic Container Service(Amazon ECS)를 사용하여 작업을 실행합니다. 10분마다 실행할 작업의 컨테이너 이미지를 기반으로 예약된 작업을 만
듭니다.
D. AWS Fargate에서 Amazon Elastic Container Service(Amazon ECS)를 사용하여 작업을 실행합니다. 작업의 컨테이너 이미지를 기반으로 독립 실행형 작업을 생성합니다.
Windows 작업 스케줄러를 사용하여 10분마다 작업을 실행합니다

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q431
회사는 Amazon S3에 데이터를 저장하고 데이터가 변경되지 않도록 해야 합니다. 회사는 Amazon S3에 업로드된 새 객체가 회사에서 객체를 수정하기로 결정할 때까지 불특정한 시간 동 안 변경 불가능한 상태로 유지되기를 원합니다. 회사 AWS 계정의 특정 사용자만 개체를 삭제할 수 있습니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. S3 Glacier 볼트를 생성합니다. 개체에 WORM(Write-Once, Read-Many) 볼트 잠금 정책을 적용합니다. 
B. S3 객체 잠금이 활성화된 S3 버킷을 생성합니다. 버전 관리를 활성화합니다. 보존 기간을 100년으로 설정합니다. 거버넌스 모드를 새 객체에 대한 S3 버킷의 기본 보관 모드로 사용합니
다.
C. S3 버킷을 생성합니다. AWS CloudTrail을 사용하여 객체를 수정하는 모든 S3 API 이벤트를 추적합니다. 알림을 받으면 회사가 가지고 있는 모든 백업 버전에서 수정된 개체를 복원합
니다.
D. S3 객체 잠금이 활성화된 S3 버킷을 생성합니다. 버전 관리를 활성화합니다. 객체에 법적 보존을 추가합니다. 객체를 삭제해야 하는 사용자의 IAM 정책에 s3:PutObjectLegalHold 권
한을 추가합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q432
한 회사가 최근 전 세계 고객을 대상으로 소매 웹 사이트를 배포한다고 발표했습니다. 웹 사이트는 Elastic Load Balancer 뒤에 있는 여러 Amazon EC2 인스턴스에서 실행됩니다. 인스 턴스는 여러 가용 영역의 Auto Scaling 그룹에서 실행됩니다. 회사는 고객이 웹 사이트에 액세스하는 데 사용하는 장치에 따라 다양한 버전의 콘텐츠를 고객에게 제공하려고 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 작업 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. 여러 버전의 콘텐츠를 캐시하도록 Amazon CloudFront를 구성합니다. 
B. 트래픽을 다른 인스턴스로 전달하도록 Network Load Balancer에서 호스트 헤더를 구성합니다. 
C. User-Agent 헤더를 기반으로 사용자에게 특정 객체를 보내도록 Lambda@Edge 함수를 구성합니다 . 
D. AWS Global Accelerator를 구성합니다. NLB(Network Load Balancer)에 요청을 전달합니다. 다른 EC2 인스턴스에 대한 호스트 기반 라우팅을 설정하도록 NLB를 구성합니다
.
E. AWS Global Accelerator를 구성합니다. NLB(Network Load Balancer)에 요청을 전달합니다. 다른 EC2 인스턴스에 대한 경로 기반 라우팅을 설정하도록 NLB를 구성합니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q433
회사는 사용 중인 두 개의 NAT 인스턴스가 더 이상 회사 애플리케이션에 필요한 트래픽을 지원할 수 없을 것이라고 우려하고 있습니다. 솔루션 설계자는 가용성이 높고 내결함성이 있으며 자 동으로 확장 가능한 솔루션을 구현하려고 합니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. 2개의 NAT 인스턴스를 제거하고 동일한 가용 영역에 있는 2개의 NAT 게이트웨이로 교체합니다. 
B. 다른 가용 영역의 NAT 인스턴스에 대해 Network Load Balancer와 함께 Auto Scaling 그룹을 사용합니다. 
C. 2개의 NAT 인스턴스를 제거하고 서로 다른 가용 영역에 있는 2개의 NAT 게이트웨이로 교체합니다. 
D. 두 개의 NAT 인스턴스를 서로 다른 가용 영역의 스팟 인스턴스로 교체하고 Network Load Balancer를 배포합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q434
한 회사에 두 개의 Amazon EC2 인스턴스에서 호스팅되는 동적 웹 애플리케이션이 있습니다. 회사에는 SSL 종료를 수행하기 위해 각 인스턴스에 있는 자체 SSL 인증서가 있습니다. 최근 트래픽이 증가했으며 운영 팀은 SSL 암호화 및 암호 해독으로 인해 웹 서버의 컴퓨팅 용량이 최대 한도에 도달했다고 판단했습니다. 애플리케이션의 성능을 높이려면 솔루션 설계자가 무엇을 해야 합니까?
A. AWS Certificate Manager(ACM)를 사용하여 새 SSL 인증서를 생성합니다. 각 인스턴스에 ACM 인증서를 설치합니다. 
B. Amazon S3 버킷 생성 SSL 인증서를 S3 버킷으로 마이그레이션합니다. SSL 종료를 위해 버킷을 참조하도록 EC2 인스턴스를 구성합니다. 
C. 다른 EC2 인스턴스를 프록시 서버로 생성합니다. SSL 인증서를 새 인스턴스로 마이그레이션하고 기존 EC2 인스턴스에 직접 연결하도록 구성합니다. 
D. SSL 인증서를 AWS Certificate Manager(ACM)로 가져옵니다. ACM의 SSL 인증서를 사용하는 HTTPS 리스너로 Application Load Balancer를 생성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q435
전자상거래 회사는 AWS 클라우드에서 분석 애플리케이션을 호스팅합니다. 이 애플리케이션은 매월 약 300MB의 데이터를 생성합니다. 데이터는 JSON 형식으로 저장됩니다. 회사는 데이 터 백업을 위한 재해 복구 솔루션을 평가하고 있습니다. 데이터는 필요한 경우 밀리초 단위로 액세스할 수 있어야 하며 데이터는 30일 동안 보관되어야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. Amazon OpenSearch 서비스(Amazon Elasticsearch 서비스)
B. Amazon S3 Glacier
C. Amazon S3 표준
D. PostgreSQL용 Amazon RDS

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q436
최근에 AWS로 마이그레이션한 회사에서 프로덕션 VPC로 들어오고 나가는 트래픽을 보호하기 위한 솔루션을 구현하려고 합니다. 이 회사는 온프레미스 데이터 센터에 검사 서버를 가지고 있었습니다. 검사 서버는 트래픽 흐름 검사 및 트래픽 필터링과 같은 특정 작업을 수행했습니다. 회사는 AWS 클라우드에서 동일한 기능을 갖기를 원합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 프로덕션 VPC에서 트래픽 검사 및 트래픽 필터링에 Amazon GuardDuty를 사용하십시오. 
B. 트래픽 미러링을 사용하여 트래픽 검사 및 필터링을 위해 프로덕션 VPC의 트래픽을 미러링합니다. 
C. AWS Network Firewall을 사용하여 프로덕션 VPC에 대한 트래픽 검사 및 트래픽 필터링에 필요한 규칙을 생성합니다. 
D. AWS Firewall Manager를 사용하여 프로덕션 VPC에 대한 트래픽 검사 및 트래픽 필터링에 필요한 규칙을 생성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q437
회사에서 3계층 웹 애플리케이션을 사용하여 신입 직원에게 교육을 제공합니다. 애플리케이션은 매일 12시간 동안만 액세스됩니다. 이 회사는 Amazon RDS for MySQL DB 인스턴스를 사용하여 정보를 저장하고 비용을 최소화하려고 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS Systems Manager Session Manager에 대한 IAM 정책을 구성합니다. 정책에 대한 IAM 역할을 생성합니다. 역할의 신뢰 관계를 업데이트합니다. DB 인스턴스에 대한 자동
시작 및 중지를 설정합니다.
B. DB 인스턴스가 중지될 때 사용자가 캐시에서 데이터에 액세스할 수 있는 기능을 제공하는 Redis용 Amazon ElastiCache 캐시 클러스터를 생성합니다. DB 인스턴스가 시작된 후 캐
시를 무효화합니다.
C. Amazon EC2 인스턴스를 시작합니다. Amazon RDS에 대한 액세스 권한을 부여하는 IAM 역할을 생성합니다. 역할을 EC2 인스턴스에 연결합니다. 원하는 일정에 따라 EC2 인스
턴스를 시작 및 중지하도록 cron 작업을 구성합니다.
D. DB 인스턴스를 시작하고 중지하는 AWS Lambda 함수를 생성합니다. Amazon EventBridge(Amazon CloudWatch Events) 예약 규칙을 생성하여 Lambda 함수를 호출합니
다. 규칙에 대한 이벤트 대상으로 Lambda 함수를 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q438
솔루션 설계자는 Amazon S3 버킷을 저장용으로 사용하여 문서 검토 애플리케이션을 구현하고 있습니다. 솔루션은 우발적인 문서 삭제를 방지하고 문서의 모든 버전을 사용할 수 있도록 보 장해야 합니다. 사용자는 문서를 다운로드, 수정 및 업로드할 수 있어야 합니다. 이러한 요구 사항을 충족하려면 어떤 조합의 조치를 취해야 합니까? (두 가지를 선택하세요.)
A. 읽기 전용 버킷 ACL을 활성화합니다.
B. 버킷에서 버전 관리를 활성화합니다.
C. IAM 정책을 버킷에 연결합니다.
D. 버킷에서 MFA 삭제를 활성화합니다.
E. AWS KMS를 사용하여 버킷을 암호화합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q439
회사는 데이터를 Amazon S3 버킷에 PDF 형식으로 저장합니다. 회사는 모든 신규 및 기존 데이터를 Amazon S3에 7년 동안 보관해야 한다는 법적 요구 사항을 따라야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. S3 버킷에 대한 S3 버전 관리 기능을 켭니다. 7년 후 데이터를 삭제하도록 S3 수명 주기를 구성합니다. 모든 S3 객체에 대한 MFA(Multi-Factor Authentication) 삭제를 구성합니다
.
B. S3 버킷에 대한 거버넌스 보존 모드로 S3 객체 잠금을 켭니다. 7년 후에 만료되도록 보존 기간을 설정합니다. 모든 기존 개체를 다시 복사하여 기존 데이터를 준수하도록 합니다. 
C. S3 버킷에 대해 규정 준수 보존 모드로 S3 객체 잠금을 켭니다. 7년 후에 만료되도록 보존 기간을 설정합니다. 모든 기존 개체를 다시 복사하여 기존 데이터를 준수하도록 합니다. 
D. S3 버킷에 대해 규정 준수 보존 모드로 S3 객체 잠금을 켭니다. 7년 후에 만료되도록 보존 기간을 설정합니다. S3 배치 작업을 사용하여 기존 데이터를 규정에 맞게 가져옵니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q440
회사는 AWS 비즈니스 지원 계획에 가입되어 있습니다. 규정상 배포를 진행하기 전에 AWS 인프라 상태를 확인해야 합니다. 회사는 새로운 배포가 시작될 때마다 프로그램적이고 자동화된 방식으로 인프라 상태를 확인할 필요가 있습니다. 어떤 솔루션이 이러한 요구사항을 충족시킬까요?
A. 각 배포 시작 시 AWS Trusted Advisor API를 사용하고, API가 문제를 반환하면 모든 새로운 배포를 중지합니다. 
B. 각 배포 시작 시 AWS Health API를 사용하고, API가 문제를 반환하면 모든 새로운 배포를 중지합니다. 
C. 각 배포 시작 시 AWS Support API를 쿼리하고, API가 열려 있는 문제를 반환하면 모든 새로운 배포를 중지합니다. 
D. 각 워크로드에 API 호출을 보내고, API 호출이 실패하면 배포를 중지합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q441
솔루션 아키텍트가 회사의 고객 대면 애플리케이션을 설계하고 있습니다. 응용 프로그램의 데이터베이스는 일년 내내 명확하게 정의된 액세스 패턴을 가지며 연중 시간에 따라 가변적인 읽기 및 쓰기 횟수를 갖게 됩니다. 회사는 데이터베이스에 대한 감사 기록을 7일 동안 보관해야 합니다. RPO(복구 지점 목표)는 5시간 미만이어야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Auto Scaling과 함께 Amazon DynamoDB 사용 온디맨드 백업 및 Amazon DynamoDB 스트림을 사용합니다.
B. Amazon Redshift를 사용하십시오. 동시성 확장을 구성합니다. 감사 로깅을 활성화합니다. 4시간마다 데이터베이스 스냅샷을 수행합니다.
C. 프로비저닝된 IOPS와 함께 Amazon RDS 사용 데이터베이스 감사 매개변수 활성화 5시간마다 데이터베이스 스냅샷을 수행합니다.
D. Auto Scaling과 함께 Amazon Aurora MySQL을 사용합니다. 데이터베이스 감사 매개변수를 활성화하십시오.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q442
회사는 고객이 재무 정보를 검색할 수 있도록 고객에게 API 인터페이스를 제공합니다. 회사는 연중 사용량이 가장 많은 시간에 더 많은 수의 요청을 예상합니다. 회사는 API가 고객 만족을 보장하기 위해 낮은 대기 시간으로 일관되게 응답하도록 요구합니다. 회사는 API에 컴퓨팅 호스트를 제공해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Application Load Balancer 및 Amazon Elastic Container Service(Amazon ECS)를 사용합니다. 
B. 프로비저닝된 동시성과 함께 Amazon API Gateway 및 AWS Lambda 함수를 사용합니다. 
C. Application Load Balancer 및 Amazon Elastic Kubernetes Service(Amazon EKS) 클러스터를 사용합니다. 
D. 예약된 동시성과 함께 Amazon API Gateway 및 AWS Lambda 함수를 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q443
솔루션 아키텍트가 새로운 VPC 디자인을 만들고 있습니다. 로드 밸런서용 퍼블릭 서브넷 2개, 웹 서버용 프라이빗 서브넷 2개, MySQL용 프라이빗 서브넷 2개가 있습니다. 웹 서버는 HTTPS만 사용합니다. 솔루션 설계자는 이미 0.0.0.0/0에서 포트 443을 허용하는 로드 밸런서용 보안 그룹을 생성했습니다. 회사 정책에서는 각 리소스가 작업을 수행하는 데 필요한 최소 한의 액세스 권한을 갖도록 요구합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자가 사용해야 하는 추가 구성 전략은 무엇입니까?
A. 웹 서버용 보안 그룹을 생성하고 0.0.0.0/0에서 포트 443을 허용합니다. MySQL 서버용 보안 그룹을 만들고 웹 서버 보안 그룹에서 포트 3306을 허용합니다. 
B. 웹 서버용 네트워크 ACL을 생성하고 0.0.0.0/0에서 포트 443을 허용합니다. MySQL 서버용 네트워크 ACL을 생성하고 웹 서버 보안 그룹에서 포트 3306을 허용합니다. 
C. 웹 서버용 보안 그룹을 만들고 로드 밸런서에서 포트 443을 허용합니다. MySQL 서버용 보안 그룹을 만들고 웹 서버 보안 그룹에서 포트 3306을 허용합니다. 
D. 웹 서버에 대한 네트워크 ACL을 생성하고 로드 밸런서에서 포트 443을 허용합니다. MySQL 서버용 네트워크 ACL을 생성하고 웹 서버 보안 그룹에서 포트 3306을 허용합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q444
회사는 여러 가용 영역에 걸쳐 Amazon EC2 Linux 인스턴스에서 애플리케이션을 실행합니다. 애플리케이션에는 고가용성 및 POSIX(Portable Operating System Interface) 호환 스토리지 계층이 필요합니다. 스토리지 계층은 최대 데이터 내구성을 제공해야 하며 EC2 인스턴스 간에 공유 가능해야 합니다. 저장소 계층의 데이터는 처음 30일 동안 자주 액세스되고 그 이 후에는 드물게 액세스됩니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. Amazon S3 Standard 스토리지 클래스를 사용하십시오. S3 수명 주기 정책을 생성하여 자주 액세스하지 않는 데이터를 S3 Glacier로 이동합니다. 
B. Amazon S3 Standard 스토리지 클래스를 사용합니다. S3 수명 주기 정책을 생성하여 자주 액세스하지 않는 데이터를 S3 Standard-Infrequent Access(S3 Standard-IA)로 이
동합니다.
C. Amazon Elastic File System(Amazon EFS) Standard 스토리지 클래스를 사용합니다. 자주 액세스하지 않는 데이터를 EFS Standard-Infrequent Access(EFS
Standard-IA)로 이동하는 수명 주기 관리 정책을 만듭니다.
D. Amazon Elastic File System(Amazon EFS) One Zone 스토리지 클래스를 사용합니다. 자주 액세스하지 않는 데이터를 EFS One Zone-Infrequent Access(EFS One
Zone-IA)로 이동하는 수명 주기 관리 정책을 만듭니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q445
회사는 30일 이내에 데이터 센터에서 AWS 클라우드로 20TB의 데이터를 마이그레이션해야 합니다. 회사의 네트워크 대역폭은 15Mbps로 제한되며 사용률이 70%를 초과할 수 없습니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS Snowball을 사용하십시오. 
B. AWS DataSync를 사용합니다. 
C. 안전한 VPN 연결을 사용하십시오. 
D. Amazon S3 Transfer Acceleration을 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q446
한 회사에서 단일 가용 영역과 Amazon RDS 다중 AZ DB 인스턴스에서 Amazon EC2를 사용하는 상태 비저장 2계층 애플리케이션을 설계했습니다. 새로운 회사 경영진은 애플리케이션 의 가용성을 높이려고 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 다중 AZ EC2 Auto Scaling을 사용하도록 애플리케이션을 구성하고 Application Load Balancer를 생성합니다. 
B. EC2 인스턴스의 스냅샷을 찍어 다른 AWS 리전으로 보내도록 애플리케이션을 구성합니다. 
C. Amazon Route 53 대기 시간 기반 라우팅을 사용하여 애플리케이션에 요청을 제공하도록 애플리케이션을 구성합니다. 
D. 들어오는 요청을 처리하고 다중 AZ 애플리케이션 로드 밸런서를 생성하도록 Amazon Route 53 규칙을 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q447
한 회사에 AWS에 배포된 3계층 웹 애플리케이션이 있습니다. 웹 서버는 VPC의 퍼블릭 서브넷에 배포됩니다. 애플리케이션 서버와 데이터베이스 서버는 동일한 VPC의 프라이빗 서브넷에 배포됩니다. 이 회사는 검사 VPC의 AWS Marketplace에서 타사 가상 방화벽 어플라이언스를 배포했습니다. 기기는 IP 패킷을 수락할 수 있는 IP 인터페이스로 구성됩니다. 솔루션 설계자는 트래픽이 웹 서버에 도달하기 전에 애플리케이션에 대한 모든 트래픽을 검사하기 위해 웹 애플리케이션을 어플라이언스와 통합해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 애플리케이션 VPC의 퍼블릭 서브넷에 Network Load Balancer를 생성하여 패킷 검사를 위해 어플라이언스로 트래픽을 라우팅합니다. 
B. 애플리케이션 VPC의 퍼블릭 서브넷에 Application Load Balancer를 생성하여 패킷 검사를 위해 트래픽을 어플라이언스로 라우팅합니다. 
C. Transit Gateway를 통해 들어오는 패킷을 라우팅하도록 라우팅 테이블을 구성하는 검사 VPC에 Transit Gateway를 배포합니다. 
D. 검사 VPC에 게이트웨이 로드 밸런서를 배포합니다. 수신 패킷을 수신하고 패킷을 어플라이언스로 전달하기 위한 게이트웨이 로드 밸런서 엔드포인트를 생성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q448
솔루션 설계자는 소프트웨어 데모 환경을 위한 아키텍처를 설계하고 있습니다. 환경은 Application Load Balancer(ALB) 뒤에 있는 Auto Scaling 그룹의 Amazon EC2 인스턴스에서 실행됩니다. 시스템은 근무 시간 동안 트래픽이 크게 증가하지만 주말에는 작동하지 않아도 됩니다. 수요에 맞게 시스템을 확장할 수 있도록 하기 위해 솔루션 설계자는 어떤 조치 조합을 취해야 합니까? (두 가지를 선택하세요.)
A. AWS Auto Scaling을 사용하여 요청 속도에 따라 ALB 용량을 조정하십시오. 
B. AWS Auto Scaling을 사용하여 VPC 인터넷 게이트웨이의 용량을 확장합니다. 
C. 여러 AWS 지역에서 EC2 인스턴스를 시작하여 여러 지역에 로드를 분산합니다. 
D. 대상 추적 조정 정책을 사용하여 인스턴스 CPU 사용률을 기반으로 Auto Scaling 그룹을 조정합니다. 
E. 예약된 조정을 사용하여 Auto Scaling 그룹의 최소, 최대 및 원하는 용량을 주말 동안 0으로 변경합니다. 주의 시작 시 기본값으로 되돌립니다.

<details>
<summary>정답 보기</summary>

**DE**
</details>

---

### Q449
애플리케이션은 VPC의 Amazon EC2 인스턴스에서 실행됩니다. 애플리케이션은 Amazon S3 버킷에 저장된 로그를 처리합니다. EC2 인스턴스는 인터넷 연결 없이 S3 버킷에 액세스해 야 합니다. Amazon S3에 프라이빗 네트워크 연결을 제공하는 솔루션은 무엇입니까?
A. S3 버킷에 대한 게이트웨이 VPC 엔드포인트를 생성합니다. 
B. 로그를 Amazon CloudWatch Logs로 스트리(cid:1535)합니다. 로그를 S3 버킷으로 내보냅니다. 
C. Amazon EC2에서 인스턴스 프로필을 생성하여 S3 액세스를 허용합니다. 
D. S3 엔드포인트에 액세스하기 위한 프라이빗 링크가 있는 Amazon API Gateway API를 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q450
회사는 Amazon S3 버킷에서 웹 애플리케이션을 호스팅하고 있습니다. 이 애플리케이션은 Amazon Cognito를 자격 증명 공급자로 사용하여 사용자를 인증하고 다른 S3 버킷에 저장된 보호된 리소스에 대한 액세스를 제공하는 JSON 웹 토큰(JWT)을 반환합니다. 응용 프로그램 배포 시 사용자는 오류를 보고하고 보호된 콘텐츠에 액세스할 수 없습니다. 솔루션 설계자는 사용자가 보호된 콘텐츠에 액세스할 수 있도록 적절한 권한을 제공하여 이 문제를 해 결해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon Cognito 자격 증명 풀을 업데이트하여 보호된 콘텐츠에 액세스하기 위한 적절한 IAM 역할을 맡습니다. 
B. 애플리케이션이 보호된 콘텐츠에 액세스할 수 있도록 S3 ACL을 업데이트합니다. 
C. 애플리케이션을 Amazon S3에 재배포하여 S3 버킷의 최종적으로 일관된 읽기가 보호된 콘텐츠에 액세스하는 사용자의 기능에 영향을 미치지 않도록 합니다. 
D. 자격 증명 풀 내에서 사용자 지정 속성 매핑을 사용하고 사용자에게 보호된 콘텐츠에 액세스할 수 있는 적절한 권한을 부여하도록 Amazon Cognito 풀을 업데이트합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q451
회사에서 Amazon EC2 인스턴스 플릿을 사용하여 온프레미스 데이터 소스에서 데이터를 수집하고 있습니다. 데이터는 JSON 형식이며 수집 속도는 최대 1MB/s입니다. EC2 인스턴스가 재부팅되면 진행 중인 데이터가 손실됩니다. 회사의 데이터 과학 팀은 거의 실시간으로 수집된 데이터를 쿼리하려고 합니다. 데이터 손실을 최소화하면서 확장 가능한 거의 실시간 데이터 쿼리를 제공하는 솔루션은 무엇입니까?
A. Amazon Kinesis Data Streams에 데이터를 게시하고 Kinesis Data Analytics를 사용하여 데이터를 쿼리합니다. 
B. Amazon Redshift를 대상으로 사용하여 Amazon Kinesis Data Firehose에 데이터를 게시합니다. Amazon Redshift를 사용하여 데이터를 쿼리합니다. 
C. 수집된 데이터를 EC2 인스턴스 스토어에 저장합니다. Amazon S3를 대상으로 Amazon Kinesis Data Firehose에 데이터를 게시합니다. Amazon Athena를 사용하여 데이터를
쿼리합니다.
D. 수집된 데이터를 Amazon Elastic Block Store(Amazon EBS) 볼륨에 저장합니다. Redis용 Amazon ElastiCache에 데이터를 게시합니다. Redis 채널을 구독하여 데이터를
쿼리합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q452
회사는 온프레미스 위치에서 Amazon S3 버킷으로 100GB의 기록 데이터를 마이그레이션하려고 합니다. 이 회사는 온프레미스에 100Mbps 인터넷 연결을 갖추고 있습니다. 회사는 S3 버킷으로 전송되는 데이터를 암호화해야 합니다. 회사는 새로운 데이터를 Amazon S3에 직접 저장합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS CLI에서 s3 sync 명령을 사용하여 데이터를 S3 버킷으로 직접 이동합니다. 
B. AWS DataSync를 사용하여 온프레미스 위치에서 S3 버킷으로 데이터 마이그레이션 
C. AWS Snowball을 사용하여 데이터를 S3 버킷으로 이동 
D. 온프레미스 위치에서 AWS로 IPsec VPN을 설정합니다. AWS CLI에서 s3 cp 명령을 사용하여 데이터를 S3 버킷으로 직접 이동

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q453
회사는 AWS Lambda와 통합된 Amazon API Gateway API 백엔드를 사용하는 프런트엔드 애플리케이션을 호스팅합니다. API가 요청을 받으면 Lambda 함수는 많은 라이브러리를 로드합니다. 그런 다음 Lambda 함수는 Amazon RDS 데이터베이스에 연결하여 데이터를 처리하고 프런트엔드 애플리케이션에 데이터를 반환합니다. 회사는 회사 운영에 대한 변경 횟수 를 최소화하면서 모든 사용자의 응답 대기 시간을 가능한 한 낮추고자 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. API를 우회하여 쿼리 속도를 높이려면 프런트엔드 애플리케이션과 데이터베이스 사이에 연결을 설정합니다. 
B. 요청을 처리하는 Lambda 함수에 대해 프로비저닝된 동시성을 구성합니다. 
C. 유사한 데이터 세트를 더 빠르게 검색하기 위해 쿼리 결과를 Amazon S3에 캐시합니다. 
D. Lambda가 한 번에 설정할 수 있는 연결 수를 늘리려면 데이터베이스 크기를 늘립니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q454
회사에서 새로운 비즈니스 애플리케이션을 구현하고 있습니다. 이 애플리케이션은 두 개의 Amazon EC2 인스턴스에서 실행되며 문서 저장을 위해 Amazon S3 버킷을 사용합니다. 솔루션 설계자는 EC2 인스턴스가 S3 버킷에 액세스할 수 있는지 확인해야 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. S3 버킷에 대한 액세스 권한을 부여하는 IAM 역할을 생성합니다. 역할을 EC2 인스턴스에 연결합니다. 
B. S3 버킷에 대한 액세스 권한을 부여하는 IAM 정책을 생성합니다. 정책을 EC2 인스턴스에 연결합니다. 
C. S3 버킷에 대한 액세스 권한을 부여하는 IAM 그룹을 생성합니다. 그룹을 EC2 인스턴스에 연결합니다. 
D. S3 버킷에 대한 액세스 권한을 부여하는 IAM 사용자를 생성합니다. 사용자 계정을 EC2 인스턴스에 연결합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q455
회사에 Amazon DynamoDB 기반 데이터 저장소가 있는 모바일 채팅 애플리케이션이 있습니다. 사용자는 가능한 한 짧은 대기 시간으로 새 메시지를 읽기를 원합니다. 솔루션 설계자는 최 소한의 애플리케이션 변경이 필요한 최적의 솔루션을 설계해야 합니다. 솔루션 설계자는 어떤 방법을 선택해야 합니까?
A. 새 메시지 테이블에 대해 Amazon DynamoDB Accelerator(DAX)를 구성합니다. DAX 끝점을 사용하도록 코드를 업데이트합니다. 
B. 증가된 읽기 로드를 처리하기 위해 DynamoDB 읽기 복제본을 추가합니다. 읽기 전용 복제본의 읽기 엔드포인트를 가리키도록 애플리케이션을 업데이트합니다. 
C. DynamoDB의 새 메시지 테이블에 대한 읽기 용량 단위 수를 두 배로 늘립니다. 기존 DynamoDB 엔드포인트를 계속 사용합니다. 
D. Redis 캐시용 Amazon ElastiCache를 애플리케이션 스택에 추가합니다. DynamoDB 대신 Redis 캐시 엔드포인트를 가리키도록 애플리케이션을 업데이트합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q456
전자상거래 회사는 테라바이트 규모의 고객 데이터를 AWS 클라우드에 저장합니다. 데이터에는 개인 식별 정보(PII)가 포함되어 있습니다. 회사는 세 가지 응용 프로그램에서 데이터를 사용하 려고 합니다. 애플리케이션 중 하나만 PII를 처리해야 합니다. 다른 두 애플리케이션이 데이터를 처리하기 전에 PII를 제거해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon DynamoDB 테이블에 데이터를 저장합니다. 각 애플리케이션이 요청하는 데이터를 가로채서 처리할 프록시 애플리케이션 계층을 생성합니다.
B. 데이터를 Amazon S3 버킷에 저장합니다. 요청 애플리케이션에 데이터를 반환하기 전에 S3 객체 Lambda를 사용하여 데이터를 처리하고 변환합니다.
C. 데이터를 처리하고 변환된 데이터를 3개의 개별 Amazon S3 버킷에 저장하여 각 애플리케이션이 고유한 사용자 지정 데이터 세트를 갖도록 합니다. 각 애플리케이션이 해당 S3 버킷을
가리키도록 합니다.
D. 데이터를 처리하고 변환된 데이터를 3개의 별도 Amazon DynamoDB 테이블에 저장하여 각 애플리케이션이 자체 사용자 지정 데이터 세트를 갖도록 합니다. 각 애플리케이션이 해당
DynamoDB 테이블을 가리키도록 합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q457
회사에서 기존 온프레미스 모놀리식 애플리케이션을 AWS로 마이그레이션하려고 합니다. 회사는 프런트엔드 코드와 백엔드 코드를 최대한 많이 유지하려고 합니다. 그러나 회사는 응용 프로 그램을 더 작은 응용 프로그램으로 나누기를 원합니다. 다른 팀이 각 애플리케이션을 관리합니다. 이 회사는 운영 오버헤드를 최소화하는 확장성이 뛰어난 솔루션이 필요합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Lambda에서 애플리케이션을 호스팅합니다. 애플리케이션을 Amazon API Gateway와 통합합니다. 
B. AWS Amplify로 애플리케이션을 호스팅합니다. AWS Lambda와 통합된 Amazon API Gateway API에 애플리케이션을 연결합니다. 
C. Amazon EC2 인스턴스에서 애플리케이션을 호스팅합니다. Auto Scaling 그룹의 EC2 인스턴스를 대상으로 하는 Application Load Balancer를 설정합니다. 
D. Amazon Elastic Container Service(Amazon ECS)에서 애플리케이션을 호스팅합니다. Amazon ECS를 대상으로 하는 Application Load Balancer를 설정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q458
회사의 규정 준수 팀은 파일 공유를 AWS로 이동해야 합니다. 공유는 Windows Server SMB 파일 공유에서 실행됩니다. 자체 관리형 온프레미스 Active Directory는 파일 및 폴더에 대 한 액세스를 제어합니다. 이 회사는 Windows File Server용 Amazon FSx를 솔루션의 일부로 사용하려고 합니다. 회사는 온프레미스 Active Directory 그룹이 AWS로 이동한 후 FSx for Windows File Server SMB 규정 준수 공유, 폴더 및 파일에 대한 액세스를 제한하는지 확인해야 합니다. 이 회사는 Windows 파일 서버 파일 시스템용 FSx를 만들었습니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Active Directory에 연결할 Active Directory 커넥터를 만듭니다. Active Directory 그룹을 IAM 그룹에 매핑하여 액세스를 제한합니다. 
B. 제한 태그 키와 규정 준수 태그 값을 사용하여 태그를 할당합니다. Active Directory 그룹을 IAM 그룹에 매핑하여 액세스를 제한합니다. 
C. 액세스를 제한하기 위해 FSx for Windows File Server에 직접 연결된 IAM 서비스 연결 역할을 생성합니다. 
D. 파일 시스템을 Active Directory에 연결하여 액세스를 제한합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q459
한 회사에 Auto Scaling 그룹의 여러 Amazon EC2 인스턴스에 배포된 다중 계층 애플리케이션이 있습니다. Amazon RDS for Oracle 인스턴스는 Oracle 관련 PL/SQL 기능을 사용 하는 애플리케이션의 데이터 계층입니다. 애플리케이션에 대한 트래픽은 꾸준히 증가하고 있습니다. 이로 인해 EC2 인스턴스가 과부하되고 RDS 인스턴스의 스토리지가 부족해집니다. Auto Scaling 그룹에는 조정 지표가 없으며 최소 정상 인스턴스 수만 정의합니다. 이 회사는 트래픽이 안정되기 전에 꾸준하지만 예측할 수 없는 속도로 계속 증가할 것이라고 예측합니다. 증가된 트래픽에 대해 시스템이 자동으로 확장될 수 있도록 하려면 솔루션 설계자가 무엇을 해야 합니까? (두 가지를 선택하세요.)
A. RDS for Oracle 인스턴스에서 스토리지 Auto Scaling을 구성합니다. 
B. Auto Scaling 스토리지를 사용하려면 데이터베이스를 Amazon Aurora로 마이그레이션하십시오. 
C. 사용 가능한 저장 공간 부족에 대해 Oracle 인스턴스용 RDS에서 경보를 구성합니다. 
D. 평균 CPU를 조정 지표로 사용하도록 Auto Scaling 그룹을 구성합니다. 
E. 평균 여유 메모리를 조정 지표로 사용하도록 Auto Scaling 그룹을 구성합니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q460
AWS에서 웹 애플리케이션을 호스팅하는 회사는 모든 Amazon EC2 인스턴스를 보장하려고 합니다. Amazon RDS DB 인스턴스. Amazon Redshift 클러스터는 태그로 구성됩니다. 회사는 이 검사를 구성하고 운영하는 노력을 최소화하기를 원합니다. 이를 달성하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. AWS Config 규칙을 사용하여 적절하게 태그가 지정되지 않은 리소스를 정의하고 감지합니다. 
B. Cost Explorer를 사용하여 태그가 제대로 지정되지 않은 리소스를 표시합니다. 해당 리소스에 수동으로 태그를 지정합니다. 
C. 적절한 태그 할당을 위해 모든 리소스를 확인하는 API 호출을 작성합니다. EC2 인스턴스에서 주기적으로 코드를 실행합니다. 
D. 적절한 태그 할당을 위해 모든 리소스를 확인하는 API 호출을 작성합니다. 코드를 주기적으로 실행하도록 Amazon CloudWatch를 통해 AWS Lambda 함수를 예약합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q461
회사는 직원들에게 기밀 및 민감한 파일에 대한 안전한 액세스를 제공해야 합니다. 회사는 권한이 있는 사용자만 파일에 액세스할 수 있기를 원합니다. 파일은 직원의 장치에 안전하게 다운로드 되어야 합니다. 파일은 온프레미스 Windows 파일 서버에 저장됩니다. 그러나 원격 사용량의 증가로 인해 파일 서버의 용량이 부족합니다. . 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 파일 서버를 퍼블릭 서브넷의 Amazon EC2 인스턴스로 마이그레이션합니다. 인바운드 트래픽을 직원의 IP 주소로 제한하도록 보안 그룹을 구성합니다. 
B. 파일을 Amazon FSx for Windows File Server 파일 시스템으로 마이그레이션합니다. Amazon FSx 파일 시스템을 온프레미스 Active Directory와 통합합니다. AWS 클라이언
트 VPN을 구성합니다.
C. 파일을 Amazon S3로 마이그레이션하고 프라이빗 VPC 엔드포인트를 생성합니다. 다운로드를 허용하려면 서명된 URL을 만듭니다. 
D. 파일을 Amazon S3로 마이그레이션하고 퍼블릭 VPC 엔드포인트를 생성합니다. 직원이 AWS IAM Identity Center(AWS Single Sign-On)로 로그인하도록 허용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q462
한 회사가 AWS 클라우드에서 공개 웹 애플리케이션을 출시할 준비를 하고 있습니다. 아키텍처는 ELB(Elastic Load Balancer) 뒤에 있는 VPC 내의 Amazon EC2 인스턴스로 구성됩 니다. 타사 서비스가 DNS에 사용됩니다. 회사의 솔루션 설계자는 대규모 DDoS 공격을 탐지하고 방어하는 솔루션을 추천해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 계정에서 Amazon GuardDuty를 활성화합니다. 
B. EC2 인스턴스에서 Amazon Inspector를 활성화합니다. 
C. AWS Shield를 활성화하고 여기에 Amazon Route 53을 할당합니다. 
D. AWS Shield Advanced를 활성화하고 여기에 ELB를 할당합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q463
회사는 Amazon S3에 데이터를 저장합니다. 규정에 따르면 데이터에는 개인 식별 정보(PII)가 포함되어서는 안 됩니다. 이 회사는 최근 S3 버킷에 PII가 포함된 일부 개체가 있음을 발견했 습니다. 회사는 S3 버킷에서 PII를 자동으로 감지하고 회사의 보안 팀에 알려야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Macie를 사용하십시오. Amazon EventBridge 규칙을 생성하여 Macie 결과에서 SensitiveData 이벤트 유형을 필터링하고 보안 팀에 Amazon Simple Notification
Service(Amazon SNS) 알림을 보냅니다.
B. Amazon GuardDuty를 사용합니다. GuardDuty 결과에서 중요한 이벤트 유형을 필터링하고 보안 팀에 Amazon Simple Notification Service(Amazon SNS) 알림을 보내는
Amazon EventBridge 규칙을 생성합니다.
C. Amazon Macie를 사용합니다. Amazon EventBridge 규칙을 생성하여 Macie 결과에서 SensitiveData:S3Object/Personal 이벤트 유형을 필터링하고 보안 팀에 Amazon
Simple Queue Service(Amazon SQS) 알림을 보냅니다.
D. Amazon GuardDuty를 사용합니다. GuardDuty 결과에서 중요한 이벤트 유형을 필터링하고 보안 팀에 Amazon Simple Queue Service(Amazon SQS) 알림을 보내는
Amazon EventBridge 규칙을 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q464
회사는 Amazon API Gateway 및 AWS Lambda를 사용하여 AWS에서 내부 서버리스 애플리케이션을 호스팅합니다. 회사 직원들은 매일 애플리케이션을 사용하기 시작할 때 대기 시간 이 길어지는 문제를 보고합니다. 회사는 대기 시간을 줄이고 싶어합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. API 게이트웨이 조절 한도를 늘리십시오.
B. 직원이 매일 애플리케이션을 사용하기 전에 Lambda 프로비저닝 동시성을 높이기 위해 예약된 조정을 설정합니다.
C. Amazon CloudWatch 경보를 생성하여 매일 시작 시 경보 대상으로 Lambda 함수를 시작합니다.
D. Lambda 함수 메모리를 늘립니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q465
솔루션 설계자는 정적 웹 사이트를 저장하기 위해 Amazon S3 오리진과 함께 Amazon CloudFront를 사용하는 솔루션을 설계해야 합니다. 회사의 보안 정책에 따라 모든 웹 사이트 트래 픽은 AWS WAF에서 검사해야 합니다. 솔루션 설계자는 이러한 요구 사항을 어떻게 준수해야 합니까?
A. AWS WAF Amazon 리소스 이름(ARN)에서만 오는 요청을 수락하도록 S3 버킷 정책을 구성합니다. 
B. S3 오리진에서 콘텐츠를 요청하기 전에 모든 수신 요청을 AWS WAF로 전달하도록 Amazon CloudFront를 구성합니다. 
C. Amazon CloudFront IP 주소가 Amazon S3에만 액세스하도록 허용하는 보안 그룹을 구성합니다. AWS WAF를 CloudFront에 연결합니다. 
D. 원본 액세스 ID(OAI)를 사용하여 S3 버킷에 대한 액세스를 제한하도록 Amazon CloudFront 및 Amazon S3를 구성합니다. 배포에서 AWS WAF를 활성화합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q466
회사가 AWS에서 모바일 앱을 구축하고 있습니다. 회사는 수백만 명의 사용자에게 도달 범위를 확장하려고 합니다. 회사는 승인된 사용자가 모바일 장치에서 회사의 콘텐츠를 볼 수 있도록 플 랫폼을 구축해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. 퍼블릭 Amazon S3 버킷에 콘텐츠를 게시합니다. AWS Key Management Service(AWS KMS) 키를 사용하여 콘텐츠를 스트리(cid:1535)합니다. 
B. 모바일 앱과 AWS 환경 간에 IPsec VPN을 설정하여 콘텐츠를 스트리(cid:1535)합니다. 
C. Amazon CloudFront를 사용합니다. 스트리(cid:1535) 콘텐츠에 서명된 URL을 제공합니다. 
D. 모바일 앱과 AWS 환경 간에 AWS Client VPN을 설정하여 콘텐츠를 스트리(cid:1535)합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q467
병원은 환자 기록을 Amazon S3 버킷에 저장해야 합니다. 병원의 규정 준수 팀은 모든 PHI(보호된 건강 정보)가 전송 및 저장 중에 암호화되도록 해야 합니다. 규정 준수 팀은 미사용 데이터 에 대한 암호화 키를 관리해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Certificate Manager(ACM)에서 퍼블릭 SSL/TLS 인증서를 생성합니다. 인증서를 Amazon S3와 연결합니다. AWS KMS 키(SSE-KMS)로 서버 측 암호화를 사용하도
록 각 S3 버킷에 대한 기본 암호화를 구성합니다. KMS 키를 관리할 규정 준수 팀을 할당합니다.
B. S3 버킷 정책에서 aws:SecureTransport 조건을 사용하여 HTTPS(TLS)를 통한 암호화된 연결만 허용합니다. S3 관리형 암호화 키(SSE-S3)로 서버 측 암호화를 사용하도록 각
S3 버킷에 대한 기본 암호화를 구성합니다. SSE-S3 키를 관리할 규정 준수 팀을 할당합니다.
C. S3 버킷 정책에서 aws:SecureTransport 조건을 사용하여 HTTPS(TLS)를 통한 암호화된 연결만 허용합니다. AWS KMS 키(SSE-KMS)로 서버 측 암호화를 사용하도록 각 S3
버킷에 대한 기본 암호화를 구성합니다. KMS 키를 관리할 규정 준수 팀을 할당합니다.
D. S3 버킷 정책에서 aws:SecureTransport 조건을 사용하여 HTTPS(TLS)를 통한 암호화된 연결만 허용합니다. Amazon Macie를 사용하여 Amazon S3에 저장된 민감한 데이터
를 보호하십시오. Macie를 관리할 규정 준수 팀을 지정합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q468
한 회사가 AWS Lake Formation을 사용하여 AWS에 데이터 분석 플랫폼을 구축하고 있습니다. 플랫폼은 Amazon S3 및 Amazon RDS와 같은 다양한 소스에서 데이터를 수집합니다 . 회사에는 민감한 정보가 포함된 데이터 부분에 대한 액세스를 방지하기 위한 보안 솔루션이 필요합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Lake Formation 테이블에 액세스할 수 있는 권한이 포함된 IAM 역할을 생성합니다. 
B. 행 수준 보안과 셀 수준 보안을 구현하기 위한 데이터 필터를 만듭니다. 
C. Lake Formation이 데이터를 수집하기 전에 민감한 정보를 제거하는 AWS Lambda 함수를 생성합니다. 
D. Lake Formation 테이블에서 민감한 정보를 주기적으로 쿼리하고 제거하는 AWS Lambda 함수를 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q469
한 회사가 최근 단일 AWS 리전의 Amazon EC2 인스턴스에서 애플리케이션을 다시 호스팅하여 웹 애플리케이션을 AWS로 마이그레이션했습니다. 이 회사는 응용 프로그램 아키텍처를 고가용성 및 내결함성을 갖도록 재설계하려고 합니다. 트래픽은 실행 중인 모든 EC2 인스턴스에 무작위로 도달해야 합니다. 회사는 이러한 요구 사항을 충족하기 위해 어떤 조합의 단계를 수행해야 합니까? (두 가지를 선택하세요.)
A. Amazon Route 53 장애 조치 라우팅 정책을 만듭니다. 
B. Amazon Route 53 가중 라우팅 정책을 생성합니다. 
C. Amazon Route 53 다중값 응답 라우팅 정책을 생성합니다. 
D. 3개의 EC2 인스턴스를 시작합니다. 하나의 가용 영역에 있는 2개의 인스턴스와 다른 가용 영역에 있는 하나의 인스턴스입니다. 
E. 4개의 EC2 인스턴스를 시작합니다. 하나의 가용 영역에 2개의 인스턴스와 다른 가용 영역에 2개의 인스턴스가 있습니다.

<details>
<summary>정답 보기</summary>

**CE**
</details>

---

### Q470
솔루션 아키텍트는 AWS 클라우드에 배포되는 새 애플리케이션의 아키텍처를 설계하고 있습니다. 애플리케이션은 Amazon EC2 온디맨드 인스턴스에서 실행되며 여러 가용 영역에서 자동 으로 확장됩니다. EC2 인스턴스는 하루 종일 자주 확장 및 축소됩니다. Application Load Balancer(ALB)는 부하 분산을 처리합니다. 아키텍처는 분산 세션 데이터 관리를 지원해야 합니 다. 회사는 필요한 경우 기꺼이 코드를 변경할 수 있습니다. 아키텍처가 분산 세션 데이터 관리를 지원하도록 하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. Amazon ElastiCache를 사용하여 세션 데이터를 관리하고 저장합니다. 
B. ALB의 세션 선호도(스티키 세션)를 사용하여 세션 데이터를 관리합니다. 
C. AWS Systems Manager의 Session Manager를 사용하여 세션을 관리합니다. 
D. AWS Security Token Service(AWS STS)에서 GetSessionToken API 작업을 사용하여 세션을 관리합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q471
회사에서 단일 Amazon EC2 인스턴스에서 실행되는 콘텐츠 관리 시스템을 사용하고 있습니다. EC2 인스턴스에는 웹 서버와 데이터베이스 소프트웨어가 모두 포함되어 있습니다. 회사는 웹 사이트 플랫폼을 고가용성으로 만들고 사용자 요구에 맞게 웹 사이트를 확장할 수 있어야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. 데이터베이스를 Amazon RDS로 이동하고 자동 백업을 활성화합니다. 동일한 가용 영역에서 다른 EC2 인스턴스를 수동으로 시작합니다. 가용 영역에서 Application Load
Balancer를 구성하고 두 인스턴스를 대상으로 설정합니다.
B. 기존 EC2 인스턴스와 동일한 가용 영역에 있는 읽기 전용 복제본이 있는 Amazon Aurora 인스턴스로 데이터베이스를 마이그레이션합니다. 동일한 가용 영역에서 다른 EC2 인스턴스
를 수동으로 시작합니다. Application Load Balancer를 구성하고 두 개의 EC2 인스턴스를 대상으로 설정합니다.
C. 다른 가용 영역에 읽기 전용 복제본이 있는 Amazon Aurora로 데이터베이스를 이동합니다. EC2 인스턴스에서 Amazon 머신 이미지(AMI)를 생성합니다. 두 가용 영역에서
Application Load Balancer를 구성합니다. 두 가용 영역에서 AMI를 사용하는 Auto Scaling 그룹을 연결합니다.
D. 데이터베이스를 별도의 EC2 인스턴스로 이동하고 Amazon S3로 백업을 예약합니다. 원래 EC2 인스턴스에서 Amazon 머신 이미지(AMI)를 생성합니다. 두 가용 영역에서
Application Load Balancer를 구성합니다. 두 가용 영역에서 AMI를 사용하는 Auto Scaling 그룹을 연결합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q472
회사에는 데이터베이스에 주문을 작성하고 지불을 처리하기 위해 서비스를 호출하는 전자 상거래 체크아웃 워크플로우가 있습니다. 사용자는 체크아웃 프로세스 중에 시간 초과를 경험하고 있 습니다. 사용자가 체크아웃 양식을 다시 제출하면 동일한 원하는 거래에 대해 여러 고유 주문이 생성됩니다. 여러 주문 생성을 방지하기 위해 솔루션 설계자는 이 워크플로우를 어떻게 리팩터링해야 합니까?
A. Amazon Kinesis Data Firehose로 주문 메시지를 보내도록 웹 애플리케이션을 구성합니다. Kinesis Data Firehose에서 메시지를 검색하고 주문을 처리하도록 결제 서비스를 설
정합니다.
B. 로깅된 애플리케이션 경로 요청을 기반으로 AWS Lambda 함수를 호출하기 위해 AWS CloudTrail에서 규칙을 생성합니다. Lambda를 사용하여 데이터베이스를 쿼리하고 결제 서비
스를 호출하고 주문 정보를 전달합니다.
C. 데이터베이스에 주문을 저장합니다. 주문 번호가 포함된 메시지를 Amazon Simple Notification Service(Amazon SNS)로 보냅니다. Amazon SNS를 폴링하고 메시지를 검색하
고 주문을 처리하도록 결제 서비스를 설정합니다.
D. 데이터베이스에 주문을 저장합니다. 주문 번호가 포함된 메시지를 Amazon Simple Queue Service(Amazon SQS) FIFO 대기열로 보냅니다. 메시지를 검색하고 주문을 처리하도
록 결제 서비스를 설정합니다. 대기열에서 메시지를 삭제합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q473
회사에서 애플리케이션을 Amazon EC2 Linux 인스턴스로 마이그레이션했습니다. 이러한 EC2 인스턴스 중 하나는 일정에 따라 여러 개의 1시간 작업을 실행합니다. 이러한 작업은 서로 다른 팀에서 작성했으며 공통 프로그래(cid:1535) 언어가 없습니다. 회사는 이러한 작업이 단일 인스턴스에서 실행되는 동안 성능과 확장성에 대해 우려하고 있습니다. 솔루션 설계자는 이러한 문제를 해결하기 위한 솔루션을 구현해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Batch를 사용하여 작업을 작업으로 실행합니다. Amazon EventBridge(Amazon CloudWatch Events)를 사용하여 작업을 예약합니다. 
B. EC2 인스턴스를 컨테이너로 변환합니다. AWS App Runner를 사용하여 작업을 작업으로 실행할 온디맨드 컨테이너를 생성합니다. 
C. 작업을 AWS Lambda 함수에 복사합니다. Amazon EventBridge(Amazon CloudWatch Events)를 사용하여 Lambda 함수를 예약합니다. 
D. 작업을 실행하는 EC2 인스턴스의 Amazon 머신 이미지(AMI)를 생성합니다. AMI로 Auto Scaling 그룹을 생성하여 인스턴스의 여러 복사본을 실행합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q474
회사는 중요한 애플리케이션에 대한 애플리케이션 로그 파일을 10년 동안 보관해야 합니다. 애플리케이션 팀은 문제 해결을 위해 지난 달의 로그에 정기적으로 액세스하지만 한 달이 지난 로그 는 거의 액세스하지 않습니다. 애플리케이션은 매월 10TB 이상의 로그를 생성합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 스토리지 옵션은 무엇입니까?
A. Amazon S3에 로그를 저장합니다. AWS Backup을 사용하여 1개월 이상 된 로그를 S3 Glacier Deep Archive로 이동합니다. 
B. 로그를 Amazon S3에 저장합니다. S3 수명 주기 정책을 사용하여 1개월 이상 된 로그를 S3 Glacier Deep Archive로 이동합니다. 
C. Amazon CloudWatch Logs에 로그를 저장합니다. AWS Backup을 사용하여 1개월 이상 된 로그를 S3 Glacier Deep Archive로 이동합니다. 
D. Amazon CloudWatch Logs에 로그를 저장합니다. Amazon S3 수명 주기 정책을 사용하여 1개월 이상 된 로그를 S3 Glacier Deep Archive로 이동합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q475
회사에서 5개의 Amazon EC2 인스턴스에 애플리케이션을 배포합니다. ALB(Application Load Balancer)는 대상 그룹을 사용하여 인스턴스에 트래픽을 분산합니다. 각 인스턴스의 평 균 CPU 사용량은 대부분 10% 미만이며 때때로 65%까지 급증합니다. 솔루션 설계자는 애플리케이션의 확장성을 자동화하는 솔루션을 구현해야 합니다. 솔루션은 아키텍처의 비용을 최적화하고 급증이 발생할 때 애플리케이션에 충분한 CPU 리소스가 있는지 확 인해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. CPUUtilization 지표가 20% 미만일 때 ALARM 상태로 들어가는 Amazon CloudWatch 경보를 생성합니다. ALB 대상 그룹의 EC2 인스턴스 중 하나를 종료하기 위해
CloudWatch 경보가 호출하는 AWS Lambda 함수를 생성합니다.
B. EC2 Auto Scaling 그룹을 생성합니다. 기존 ALB를 로드 밸런서로 선택하고 기존 대상 그룹을 대상 그룹으로 선택하십시오. ASGAverageCPUUtilization 지표를 기반으로 하는 대
상 추적 조정 정책을 설정합니다. 최소 인스턴스를 2로, 원하는 용량을 3으로, 최대 인스턴스를 6으로, 목표 값을 50%로 설정합니다. Auto Scaling 그룹에 EC2 인스턴스를 추가합니다 .
C. EC2 Auto Scaling 그룹을 생성합니다. 기존 ALB를 로드 밸런서로 선택하고 기존 대상 그룹을 대상 그룹으로 선택하십시오. 최소 인스턴스를 2로, 원하는 용량을 3으로, 최대 인스턴스
를 6으로 설정합니다. Auto Scaling 그룹에 EC2 인스턴스를 추가합니다.
D. 두 개의 Amazon CloudWatch 경보를 생성합니다. 평균 CPUUtilization 지표가 20% 미만일 때 ALARM 상태로 들어가도록 첫 번째 CloudWatch 경보를 구성합니다. 평균
CPUUtilization 지표가 50%를 초과하면 ALARM 상태로 들어가도록 두 번째 CloudWatch 경보를 구성합니다. 이메일 메시지를 보내기 위해 Amazon Simple Notification Service(Amazon SNS) 주제에 게시하도록 경보를 구성합니다. 메시지를 받은 후 로그인하여 실행 중인 EC2 인스턴스 수를 줄이거나 늘립니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q476
회사는 Amazon EC2 인스턴스에서 고객을 위한 데모 환경을 실행합니다. 각 환경은 자체 VPC에서 격리됩니다. 환경에 대한 RDP 또는 SSH 액세스가 설정되면 회사의 운영 팀에 알려야 합니다.
A. RDP 또는 SSH 액세스가 감지되면 AWS Systems Manager OpsItems를 생성하도록 Amazon CloudWatch Application Insights를 구성합니다. 
B. AmazonSSMManagedInstanceCore 정책이 연결된 IAM 역할이 있는 IAM 인스턴스 프로필로 EC2 인스턴스를 구성합니다. 
C. Amazon CloudWatch Logs에 VPC 흐름 로그를 게시합니다. 필요한 메트릭 필터를 만듭니다. 경보가 ALARM 상태일 때 알림 작업이 포함된 Amazon CloudWatch 지표 경보를
생성합니다.
D. EC2 인스턴스 상태 변경 알림 유형의 이벤트를 수신하도록 Amazon EventBridge 규칙을 구성합니다. Amazon Simple Notification Service(Amazon SNS) 주제를 대상으로
구성합니다. 주제에 대한 운영 팀을 구독하십시오.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q477
회사는 AWS에서 전자상거래 애플리케이션을 실행합니다. 모든 새 주문은 단일 가용 영역의 Amazon EC2 인스턴스에서 실행되는 RabbitMQ 대기열에 메시지로 게시됩니다. 이러한 메시 지는 별도의 EC2 인스턴스에서 실행되는 다른 애플리케이션에 의해 처리됩니다. 이 애플리케이션은 다른 EC2 인스턴스의 PostgreSQL 데이터베이스에 세부 정보를 저장합니다. 모든 EC2 인스턴스는 동일한 가용 영역에 있습니다. 회사는 최소한의 운영 오버헤드로 최고의 가용성을 제공하도록 아키텍처를 재설계해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 대기열을 Amazon MQ에서 RabbitMQ 인스턴스의 중복 쌍(활성/대기)으로 마이그레이션합니다. 애플리케이션을 호스팅하는 EC2 인스턴스에 대한 다중 AZ Auto Scaling 그룹을
생성합니다. PostgreSQL 데이터베이스를 호스팅하는 EC2 인스턴스에 대한 또 다른 다중 AZ Auto Scaling 그룹을 생성합니다.
B. 대기열을 Amazon MQ에서 RabbitMQ 인스턴스의 중복 쌍(활성/대기)으로 마이그레이션합니다. 애플리케이션을 호스팅하는 EC2 인스턴스에 대한 다중 AZ Auto Scaling 그룹을
생성합니다. PostgreSQL용 Amazon RDS의 다중 AZ 배포에서 실행할 데이터베이스를 마이그레이션합니다.
C. RabbitMQ 대기열을 호스팅하는 EC2 인스턴스에 대한 다중 AZ Auto Scaling 그룹을 생성합니다. 애플리케이션을 호스팅하는 EC2 인스턴스에 대한 또 다른 다중 AZ Auto
Scaling 그룹을 생성합니다. PostgreSQL용 Amazon RDS의 다중 AZ 배포에서 실행할 데이터베이스를 마이그레이션합니다.
D. RabbitMQ 대기열을 호스팅하는 EC2 인스턴스에 대한 다중 AZ Auto Scaling 그룹을 생성합니다. 애플리케이션을 호스팅하는 EC2 인스턴스에 대한 또 다른 다중 AZ Auto
Scaling 그룹을 생성합니다. PostgreSQL 데이터베이스를 호스팅하는 EC2 인스턴스에 대한 세 번째 다중 AZ Auto Scaling 그룹을 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q478
전자상거래 회사는 AWS에서 다중 계층 애플리케이션을 실행하고 있습니다. 프런트 엔드 및 백엔드 계층은 모두 Amazon EC2에서 실행되고 데이터베이스는 Amazon RDS for MySQL 에서 실행됩니다. 백엔드 계층은 RDS 인스턴스와 통신합니다. 성능 저하를 일으키는 데이터베이스에서 동일한 데이터 세트를 반환하라는 호출이 자주 있습니다. 백엔드의 성능을 개선하려면 어떤 조치를 취해야 합니까?
A. Amazon SNS를 구현하여 데이터베이스 호출을 저장합니다. 
B. Amazon ElastiCache를 구현하여 대규모 데이터 세트를 캐싱합니다. 
C. 데이터베이스 호출을 캐시하기 위해 RDS for MySQL 읽기 전용 복제본을 구현합니다. 
D. Amazon Kinesis Data Firehose를 구현하여 호출을 데이터베이스로 스트리(cid:1535)합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q479
회사는 Amazon EC2 인스턴스 플릿에서 3계층 전자상거래 애플리케이션을 호스팅합니다. 인스턴스는 Application Load Balancer(ALB) 뒤의 Auto Scaling 그룹에서 실행됩니다. 모 든 전자상거래 데이터는 MariaDB 다중 AZ DB 인스턴스용 Amazon RDS에 저장됩니다. 회사는 트랜잭션 중에 고객 세션 관리를 최적화하려고 합니다. 애플리케이션은 세션 데이터를 지속적으로 저장해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까? (두 가지를 선택하세요.)
A. ALB에서 고정 세션 기능(세션 선호도)을 켭니다. 
B. Amazon DynamoDB 테이블을 사용하여 고객 세션 정보를 저장합니다. 
C. Amazon Cognito 사용자 풀을 배포하여 사용자 세션 정보를 관리합니다. 
D. Amazon ElastiCache for Redis 클러스터를 배포하여 고객 세션 정보를 저장합니다. 
E. 애플리케이션에서 AWS Systems Manager Application Manager를 사용하여 사용자 세션 정보를 관리합니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q480
한 회사에 많은 Amazon EC2 인스턴스를 사용하여 작업을 완료하는 매우 동적인 배치 처리 작업이 있습니다. 작업은 본질적으로 상태 비저장이며 부정적인 영향 없이 지정된 시간에 언제든 지 시작 및 중지할 수 있으며 일반적으로 완료하는 데 총 60분 이상 걸립니다. 회사는 솔루션 아키텍트에게 작업 요구 사항을 충족하는 확장 가능하고 비용 효율적인 솔루션을 설계하도록 요청 했습니다. 솔루션 설계자는 무엇을 추천해야 합니까?
A. EC2 스팟 인스턴스를 구현합니다. 
B. EC2 예약 인스턴스를 구매합니다. 
C. EC2 온디맨드 인스턴스를 구현합니다. 
D. AWS Lambda에서 처리를 구현합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q481
회사에서 이전 애플리케이션을 AWS로 마이그레이션하고 있습니다. 애플리케이션은 매시간 배치 작업을 실행하며 CPU를 많이 사용합니다. 배치 작업은 온프레미스 서버에서 평균 15분이 소요됩니다. 서버에는 64개의 가상 CPU(vCPU)와 512GiB의 메모리가 있습니다. 최소한의 운영 오버헤드로 15분 이내에 배치 작업을 실행하는 솔루션은 무엇입니까?
A. 기능적 확장과 함께 AWS Lambda를 사용하십시오. 
B. AWS Fargate와 함께 Amazon Elastic Container Service(Amazon ECS)를 사용합니다. 
C. AWS Auto Scaling과 함께 Amazon Lightsail을 사용합니다. 
D. Amazon EC2에서 AWS Batch를 사용합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q482
한 회사가 여러 가용 영역의 Amazon EC2 인스턴스에서 웹 애플리케이션을 실행합니다. EC2 인스턴스는 프라이빗 서브넷에 있습니다. 솔루션 설계자는 인터넷 연결 ALB(Application Load Balancer)를 구현하고 EC2 인스턴스를 대상 그룹으로 지정합니다. 그러나 인터넷 트래픽이 EC2 인스턴스에 도달하지 않습니다. 솔루션 설계자는 이 문제를 해결하기 위해 아키텍처를 어떻게 재구성해야 합니까?
A. ALB를 Network Load Balancer로 교체하십시오. 인터넷 트래픽을 허용하도록 퍼블릭 서브넷에서 NAT 게이트웨이를 구성합니다. 
B. EC2 인스턴스를 퍼블릭 서브넷으로 이동합니다. EC2 인스턴스의 보안 그룹에 규칙을 추가하여 0.0.0.0/0으로의 아웃바운드 트래픽을 허용합니다. 
C. 인터넷 게이트웨이 경로를 통해 0.0.0.0/0 트래픽을 보내도록 EC2 인스턴스의 서브넷에 대한 경로 테이블을 업데이트합니다. EC2 인스턴스의 보안 그룹에 규칙을 추가하여 0.0.0.0/0
으로의 아웃바운드 트래픽을 허용합니다.
D. 각 가용 영역에서 퍼블릭 서브넷을 생성합니다. 퍼블릭 서브넷을 ALB와 연결합니다. 프라이빗 서브넷에 대한 경로로 퍼블릭 서브넷에 대한 경로 테이블을 업데이트합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q483
회사의 웹 애플리케이션은 AWS Lambda 함수 앞의 Amazon API Gateway API와 Amazon DynamoDB 데이터베이스로 구성됩니다. Lambda 함수는 비즈니스 로직을 처리하고 DynamoDB 테이블은 데이터를 호스팅합니다. 애플리케이션은 Amazon Cognito 사용자 풀을 사용하여 애플리케이션의 개별 사용자를 식별합니다. 솔루션 설계자는 구독이 있는 사용자만 프리미엄 콘텐츠에 액세스할 수 있도록 애플리케이션을 업데이트해야 합니다. 최소한의 운영 오버헤드로 이 요구 사항을 충족하는 솔루션은 무엇입니까?
A. API Gateway API에서 API 캐싱 및 제한을 활성화합니다. 
B. API Gateway API에서 AWS WAF를 설정합니다. 구독이 있는 사용자를 필터링하는 규칙을 만듭니다. 
C. DynamoDB 테이블의 프리미엄 콘텐츠에 세분화된 IAM 권한을 적용합니다. 
D. 구독하지 않은 사용자의 액세스를 제한하기 위해 API 사용 계획 및 API 키를 구현하십시오.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q484
회사는 최근 웹 공격으로 인해 공용 웹 애플리케이션의 보안에 대해 우려하고 있습니다. 애플리케이션은 Application Load Balancer(ALB)를 사용합니다. 솔루션 설계자는 애플리케이션에 대한 DDoS 공격의 위험을 줄여야 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. ALB에 Amazon Inspector 에이전트를 추가합니다. 
B. 공격을 방지하도록 Amazon Macie를 구성합니다. 
C. 공격을 방지하려면 AWS Shield Advanced를 활성화하십시오. 
D. ALB를 모니터링하도록 Amazon GuardDuty를 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q485
한 글로벌 기업이 Amazon API Gateway를 사용하여 us-east-1 리전 및 ap-southeast-2 리전의 로열티 클럽 사용자를 위한 REST API를 설계하고 있습니다. 솔루션 설계자는 SQL 주입 및 교차 사이트 스크립팅 공격으로부터 여러 계정에 걸쳐 이러한 API Gateway 관리형 REST API를 보호하는 솔루션을 설계해야 합니다. 최소한의 관리 노력으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 두 리전에서 AWS WAF를 설정합니다. 리전 웹 ACL을 API 단계와 연결합니다. 
B. 두 리전에서 AWS Firewall Manager를 설정합니다. AWS WAF 규칙을 중앙에서 구성합니다. 
C. 목욕 지역에 AWS Shield를 설정하십시오. 리전 웹 ACL을 API 단계와 연결합니다. 
D. 리전 중 하나에 AWS Shield를 설정합니다. 리전 웹 ACL을 API 단계와 연결합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q486
회사는 사용자에게 항목 가격을 기반으로 세금 계산을 위한 조회를 자동화하는 API를 제공합니다. 회사는 연휴 기간에만 더 많은 수의 문의가 발생하여 응답 시간이 느려집니다. 솔루션 설계자 는 확장 가능하고 탄력적인 솔루션을 설계해야 합니다. 이를 달성하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. Amazon EC2 인스턴스에서 호스팅되는 API를 제공합니다. EC2 인스턴스는 API 요청이 있을 때 필요한 계산을 수행합니다. 
B. 항목 이름을 허용하는 Amazon API Gateway를 사용하여 REST API를 설계합니다. API Gateway는 세금 계산을 위해 항목 이름을 AWS Lambda에 전달합니다. 
C. 두 개의 Amazon EC2 인스턴스가 있는 Application Load Balancer를 생성합니다. EC2 인스턴스는 받은 항목 이름에 대한 세금을 계산합니다. 
D. Amazon EC2 인스턴스에서 호스팅되는 API와 연결되는 Amazon API Gateway를 사용하여 REST API를 설계합니다. API Gateway는 세금 계산을 위해 항목 이름을 수락하고
EC2 인스턴스에 전달합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q487
데이터 분석 회사에서 일괄 처리 시스템을 AWS로 마이그레이션하려고 합니다. 회사는 FTP를 통해 낮 동안 주기적으로 수천 개의 작은 데이터 파일을 받습니다. 온프레미스 일괄 작업은 밤 새 데이터 파일을 처리합니다. 그러나 일괄 작업 실행을 완료하는 데 몇 시간이 걸립니다. . 회사는 파일을 전송하는 FTP 클라이언트에 대한 최소한의 변경으로 수신 데이터 파일을 처리할 수 있는 AWS 솔루션을 원합니다. 솔루션은 파일이 성공적으로 처리된 수신 데이터 파일을 삭 제해야 합니다. 각 파일을 처리하는 데 3~8분이 소요됩니다. 운영상 가장 효율적인 방식으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. FTP 서버를 실행하는 Amazon EC2 인스턴스를 사용하여 수신 파일을 Amazon S3 Glacier Flexible Retrieval의 객체로 저장합니다. AWS Batch에서 작업 대기열을 구성합니
다. Amazon EventBridge 규칙을 사용하여 S3 Glacier Flexible Retrieval에서 야간에 객체를 처리하는 작업을 호출합니다. 작업이 개체를 처리한 후 개체를 삭제합니다.
B. FTP 서버를 실행하는 Amazon EC2 인스턴스를 사용하여 수신 파일을 Amazon Elastic Block Store(Amazon EBS) 볼륨에 저장합니다. AWS Batch에서 작업 대기열을 구성
합니다. Amazon EventBridge 규칙을 사용하여 야간에 EBS 볼륨에서 파일 프로세스를 호출합니다. 작업이 파일을 처리한 후 파일을 삭제합니다.
C. AWS Transfer Family를 사용하여 들어오는 파일을 Amazon Elastic Block Store(Amazon EBS) 볼륨에 저장할 FTP 서버를 생성합니다. AWS Batch에서 작업 대기열을 구
성합니다. 각 파일이 도착하면 Amazon S3 이벤트 알림을 사용하여 AWS Batch에서 작업을 호출합니다. 작업이 파일을 처리한 후 파일을 삭제합니다.
D. AWS Transfer Family를 사용하여 Amazon S3 Standard에 수신 파일을 저장할 FTP 서버를 생성합니다. 파일을 처리하고 파일이 처리된 후 파일을 삭제하는 AWS Lambda 함
수를 생성합니다. 파일이 도착하면 S3 이벤트 알림을 사용하여 람다 함수를 호출하십시오.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q488
한 회사가 이전에 데이터 웨어하우스 솔루션을 AWS로 마이그레이션했습니다. 회사에는 AWS Direct Connect 연결도 있습니다. 본사 사용자는 시각화 도구를 사용하여 데이터 웨어하우스 를 쿼리합니다. 데이터 웨어하우스에서 반환한 쿼리의 평균 크기는 50MB이고 시각화 도구에서 보낸 각 웹 페이지는 약 500KB입니다. 데이터 웨어하우스에서 반환된 결과 집합은 캐시되지 않습니다. 회사에 가장 낮은 데이터 전송 송신 비용을 제공하는 솔루션은 무엇입니까?
A. 온프레미스에서 시각화 도구를 호스팅하고 인터넷을 통해 직접 데이터 웨어하우스를 쿼리합니다. 
B. 데이터 웨어하우스와 동일한 AWS 리전에서 시각화 도구를 호스팅합니다. 인터넷을 통해 액세스하십시오. 
C. 온프레미스에서 시각화 도구를 호스팅하고 동일한 AWS 리전의 위치에서 Direct Connect 연결을 통해 직접 데이터 웨어하우스를 쿼리합니다. 
D. 데이터 웨어하우스와 동일한 AWS 리전에서 시각화 도구를 호스팅하고 동일한 리전의 위치에서 Direct Connect 연결을 통해 액세스합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q489
회사에는 동일한 AWS 계정에 있는 Amazon S3 버킷에 대한 읽기 액세스 권한이 필요한 AWS Lambda 함수가 있습니다. 가장 안전한 방식으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. S3 버킷에 대한 읽기 액세스 권한을 부여하는 S3 버킷 정책을 적용합니다. 
B. Lambda 함수에 IAM 역할을 적용합니다. 역할에 IAM 정책을 적용하여 S3 버킷에 대한 읽기 액세스 권한을 부여합니다. 
C. Lambda 함수의 코드에 액세스 키와 비밀 키를 내장하여 S3 버킷에 대한 읽기 액세스에 필요한 IAM 권한을 부여합니다. 
D. Lambda 함수에 IAM 역할을 적용합니다. 역할에 IAM 정책을 적용하여 계정의 모든 S3 버킷에 대한 읽기 액세스 권한을 부여합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q490
회사에는 처리할 페이로드가 포함된 메시지를 보내는 발신자 애플리케이션과 페이로드가 포함된 메시지를 수신하기 위한 처리 애플리케이션의 두 가지 애플리케이션이 있습니다. 회사는 두 애 플리케이션 간의 메시지를 처리하기 위해 AWS 서비스를 구현하려고 합니다. 발신자 애플리케이션은 매시간 약 1,000개의 메시지를 보낼 수 있습니다. 메시지를 처리하는 데 최대 2일이 걸 릴 수 있습니다. 메시지를 처리하지 못한 경우 나머지 메시지 처리에 영향을 주지 않도록 보관해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족하고 운영상 가장 효율적입니까?
A. Redis 데이터베이스를 실행하는 Amazon EC2 인스턴스를 설정합니다. 인스턴스를 사용하도록 두 애플리케이션을 모두 구성합니다. 메시지를 각각 저장, 처리 및 삭제합니다. 
B. Amazon Kinesis 데이터 스트림을 사용하여 발신자 애플리케이션에서 메시지를 수신합니다. 처리 애플리케이션을 Kinesis Client Library(KCL)와 통합합니다. 
C. 발신자 및 프로세서 애플리케이션을 Amazon Simple Queue Service(Amazon SQS) 대기열과 통합합니다. 처리에 실패한 메시지를 수집하도록 배달 못한 편지 대기열을 구성합니
다.
D. 처리할 알림을 수신하려면 처리 애플리케이션을 Amazon Simple Notification Service(Amazon SNS) 주제에 구독합니다. 발신자 애플리케이션을 통합하여 SNS 주제에 씁니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q491
회사는 AWS Organizations를 사용하여 각 사업부에 대한 전용 AWS 계정을 생성하여 요청 시 각 사업부의 계정을 독립적으로 관리합니다. 루트 이메일 수신자는 한 계정의 루트 사용자 이메일 주소로 전송된 알림을 놓쳤습니다. 회사는 향후 모든 알림을 놓치지 않기를 원합니다. 향후 알림은 계정 관리자로 제한되어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS 계정 루트 사용자 이메일 주소로 전송되는 알림 이메일 메시지를 조직의 모든 사용자에게 전달하도록 회사의 이메일 서버를 구성합니다. 
B. 모든 AWS 계정 루트 사용자 이메일 주소를 알림에 응답할 수 있는 소수의 관리자에게 전달되는 배포 목록으로 구성합니다. AWS Organizations 콘솔에서 또는 프로그래(cid:1535) 방식으로
AWS 계정 대체 연락처를 구성합니다.
C. 모든 AWS 계정 루트 사용자 이메일 메시지가 경고를 모니터링하고 해당 그룹에 해당 경고를 전달하는 역할을 담당하는 한 명의 관리자에게 전송되도록 구성합니다. 
D. 동일한 루트 사용자 이메일 주소를 사용하도록 모든 기존 AWS 계정과 새로 생성된 모든 계정을 구성합니다. AWS Organizations 콘솔에서 또는 프로그래(cid:1535) 방식으로 AWS 계정 대
체 연락처를 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q492
회사는 Amazon S3에서 정적 웹 사이트를 호스팅하고 DNS에 Amazon Route 53을 사용하고 있습니다. 웹 사이트는 전 세계적으로 수요가 증가하고 있습니다. 회사는 웹사이트에 접속하 는 사용자의 대기 시간을 줄여야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 웹사이트가 포함된 S3 버킷을 모든 AWS 리전에 복제합니다. Route 53 지리적 위치 라우팅 항목을 추가합니다. 
B. AWS Global Accelerator에서 액셀러레이터를 프로비저닝합니다. 제공된 IP 주소를 S3 버킷과 연결합니다. 가속기의 IP 주소를 가리키도록 Route 53 항목을 편집합니다. 
C. S3 버킷 앞에 Amazon CloudFront 배포를 추가합니다. CloudFront 배포를 가리키도록 Route 53 항목을 편집합니다. 
D. 버킷에서 S3 Transfer Acceleration을 활성화합니다. 새 엔드포인트를 가리키도록 Route 53 항목을 편집합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q493
회사에 개발 작업을 위한 여러 AWS 계정이 있습니다. 일부 직원은 지속적으로 대형 Amazon EC2 인스턴스를 사용하므로 회사가 개발 계정에 대한 연간 예산을 초과하게 됩니다. 회사는 이 러한 계정에서 AWS 리소스 생성을 중앙에서 제한하려고 합니다. 최소한의 개발 노력으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 승인된 EC2 생성 프로세스를 사용하는 AWS Systems Manager 템플릿을 개발합니다. 승인된 Systems Manager 템플릿을 사용하여 EC2 인스턴스를 프로비저닝합니다.
B. AWS Organizations를 사용하여 계정을 조직 단위(OU)로 구성합니다. 서비스 제어 정책(SCP)을 정의하고 연결하여 EC2 인스턴스 유형의 사용을 제어합니다.
C. EC2 인스턴스가 생성될 때 AWS Lambda 함수를 호출하는 Amazon EventBridge 규칙을 구성합니다. 허용되지 않는 EC2 인스턴스 유형을 중지합니다.
D. 직원이 허용되는 EC2 인스턴스 유형을 생성할 수 있도록 AWS Service Catalog 제품을 설정합니다. 직원이 서비스 카탈로그 제품을 사용해야만 EC2 인스턴스를 배포할 수 있는지
확인하십시오.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q494
회사에서 새로운 모바일 앱을 개발하고 있습니다. 회사는 교차 사이트 스크립팅 또는 SQL 주입과 같은 일반적인 애플리케이션 수준 공격으로부터 ALB(Application Load Balancer)를 보 호하기 위해 적절한 트래픽 필터링을 구현해야 합니다. 이 회사는 최소한의 인프라와 운영 인력을 보유하고 있습니다. 회사는 AWS 환경의 서버를 관리, 업데이트 및 보호하는 책임을 줄여야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. AWS WAF 규칙을 구성하고 이를 ALB와 연결합니다. 
B. 퍼블릭 호스팅이 활성화된 Amazon S3를 사용하여 애플리케이션을 배포합니다. 
C. AWS Shield Advanced를 배포하고 ALB를 보호된 리소스로 추가합니다. 
D. 타사 방화벽을 실행하는 Amazon EC2 인스턴스로 트래픽을 보낸 다음 트래픽을 현재 ALB로 전달하는 새 ALB를 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q495
회사는 2주 이내에 온프레미스 데이터 센터에서 AWS로 MySQL 데이터베이스를 마이그레이션해야 합니다. 데이터베이스 크기는 20TB입니다. 회사는 다운타임을 최소화하면서 마이그레이 션을 완료하기를 원합니다. 데이터베이스를 가장 비용 효율적으로 마이그레이션하는 솔루션은 무엇입니까?
A. AWS Snowball Edge Storage Optimized 디바이스를 주문합니다. AWS Schema Conversion Tool(AWS SCT)과 함께 AWS Database Migration Service(AWS
DMS)를 사용하여 진행 중인 변경 사항을 복제하여 데이터베이스를 마이그레이션합니다. Snowball Edge 디바이스를 AWS로 보내 마이그레이션을 완료하고 진행 중인 복제를 계속합 니다.
B. AWS Snowmobile 차량을 주문합니다. AWS Schema Conversion Tool(AWS SCT)과 함께 AWS Database Migration Service(AWS DMS)를 사용하여 지속적인 변경
사항이 있는 데이터베이스를 마이그레이션합니다. Snowmobile 차량을 다시 AWS로 보내 마이그레이션을 완료하고 진행 중인 복제를 계속합니다.
C. GPU 장치로 AWS Snowball Edge Compute Optimized를 주문합니다. AWS Schema Conversion Tool(AWS SCT)과 함께 AWS Database Migration Service
(AWS DMS)를 사용하여 지속적인 변경 사항이 있는 데이터베이스를 마이그레이션합니다. Snowball 디바이스를 AWS로 보내 마이그레이션을 완료하고 진행 중인 복제를 계속합니다.
D. 1GB 전용 AWS Direct Connect 연결을 주문하여 데이터 센터와의 연결을 설정합니다. AWS Schema Conversion Tool(AWS SCT)과 함께 AWS Database Migration
Service(AWS DMS)를 사용하여 진행 중인 변경 사항을 복제하여 데이터베이스를 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q496
회사에서 인공 지능 및 기계 학습(AI/ML)을 연구하는 고객에게 데이터 세트를 판매합니다. 데이터 세트는 us-east-1 리전의 Amazon S3 버킷에 저장되는 형식이 지정된 대용량 파일입니 다. 회사는 고객이 주어진 데이터 세트에 대한 액세스를 구매하는 데 사용하는 웹 애플리케이션을 호스팅합니다. 웹 애플리케이션은 Application Load Balancer 뒤의 여러 Amazon EC2 인스턴스에 배포됩니다. 구매 후 고객은 파일에 대한 액세스를 허용하는 S3 서명 URL을 받습니다. 고객은 북미와 유럽 전역에 분산되어 있습니다. 회사는 데이터 전송과 관련된 비용을 줄이고 성능을 유지하거나 개선하고자 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 기존 S3 버킷에서 S3 Transfer Acceleration을 구성합니다. 고객 요청을 S3 Transfer Acceleration 엔드포인트로 안내합니다. 액세스 제어를 위해 S3 서명 URL을 계속 사용하십
시오.
B. 기존 S3 버킷을 원본으로 사용하여 Amazon CloudFront 배포를 배포합니다. 고객 요청을 CloudFront URL로 전달합니다. 액세스 제어를 위해 CloudFront 서명 URL로 전환하십
시오.
C. 버킷 사이에 S3 교차 리전 복제가 있는 eu-central-1 리전에서 두 번째 S3 버킷을 설정합니다. 가장 가까운 지역으로 고객 요청을 전달합니다. 액세스 제어를 위해 S3 서명 URL을 계
속 사용하십시오.
D. 데이터세트를 최종 사용자에게 스트리(cid:1535)할 수 있도록 웹 애플리케이션을 수정합니다. 기존 S3 버킷에서 데이터를 읽도록 웹 애플리케이션을 구성합니다. 애플리케이션에서 직접 액세스 제
어를 구현합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q497
회사에 산발적인 사용 패턴을 가진 웹 애플리케이션이 있습니다. 매달 초에는 사용량이 많고, 매주 초에는 보통 사용량이 있으며, 주중에는 예측할 수 없는 사용량이 있습니다. 이 애플리케이션 은 웹 서버와 데이터 센터 내에서 실행되는 MySQL 데이터베이스 서버로 구성됩니다. 이 회사는 애플리케이션을 AWS 클라우드로 이동하려고 하며 데이터베이스 수정이 필요하지 않은 비용 효율적인 데이터베이스 플랫폼을 선택해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon DynamoDB 
B. MySQL용 Amazon RDS 
C. MySQL 호환 Amazon Aurora Serverless 
D. Auto Scaling 그룹의 Amazon EC2에 배포된 MySQL

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q498
회사는 기본 온프레미스 파일 스토리지 볼륨에 대한 재해 복구 계획을 구현하려고 합니다. 파일 스토리지 볼륨은 로컬 스토리지 서버의 iSCSI(Internet Small Computer Systems Interface) 장치에서 마운트됩니다. 파일 스토리지 볼륨은 수백 테라바이트(TB)의 데이터를 보유합니다. 회사는 최종 사용자가 대기 시간 없이 온프레미스 시스템의 모든 파일 유형에 즉시 액세스할 수 있기를 원합니다. 회사의 기존 인프라를 최소한으로 변경하면서 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 온프레미스에서 호스팅되는 가상 머신(VM)으로 Amazon S3 파일 게이트웨이를 프로비저닝합니다. 로컬 캐시를 10TB로 설정합니다. NFS 프로토콜을 통해 파일에 액세스하도록 기존
애플리케이션을 수정합니다. 재해에서 복구하려면 Amazon EC2 인스턴스를 프로비저닝하고 파일이 포함된 S3 버킷을 탑재합니다.
B. AWS Storage Gateway 테이프 게이트웨이를 프로비저닝합니다. 데이터 백업 솔루션을 사용하여 모든 기존 데이터를 가상 테이프 라이브러리에 백업하십시오. 초기 백업이 완료된 후
야간에 실행되도록 데이터 백업 솔루션을 구성합니다. 재해에서 복구하려면 Amazon EC2 인스턴스를 프로비저닝하고 가상 테이프 라이브러리의 볼륨에서 Amazon Elastic Block Store(Amazon EBS) 볼륨으로 데이터를 복원합니다.
C. AWS Storage Gateway 볼륨 게이트웨이 캐시 볼륨을 프로비저닝합니다. 로컬 캐시를 10TB로 설정합니다. iSCSI를 사용하여 볼륨 게이트웨이 캐싱 볼륨을 기존 파일 서버에 마운트
하고 모든 파일을 스토리지 볼륨에 복사합니다. 스토리지 볼륨의 예약된 스냅샷을 구성합니다. 재해에서 복구하려면 스냅샷을 Amazon Elastic Block Store(Amazon EBS) 볼륨으 로 복원하고 EBS 볼륨을 Amazon EC2 인스턴스에 연결합니다.
D. 기존 파일 스토리지 볼륨과 동일한 양의 디스크 공간으로 AWS Storage Gateway 볼륨 게이트웨이 저장 볼륨을 프로비저닝합니다. iSCSI를 사용하여 볼륨 게이트웨이 저장 볼륨을 기
존 파일 서버에 마운트하고 모든 파일을 스토리지 볼륨에 복사합니다. 스토리지 볼륨의 예약된 스냅샷을 구성합니다. 재해에서 복구하려면 스냅샷을 Amazon Elastic Block Store (Amazon EBS) 볼륨으로 복원하고 EBS 볼륨을 Amazon EC2 인스턴스에 연결합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q499
전자상거래 회사는 주문 처리 작업을 완료하기 위해 여러 서버리스 기능과 AWS 서비스를 포함하는 분산 애플리케이션을 구축하고 있습니다. 이러한 작업에는 워크플로의 일부로 수동 승인이 필요합니다. 솔루션 설계자는 주문 처리 애플리케이션을 위한 아키텍처를 설계해야 합니다. 솔루션은 여러 AWS Lambda 기능을 반응형 서버리스 애플리케이션으로 결합할 수 있어야 합니 다. 솔루션은 또한 Amazon EC2 인스턴스, 컨테이너 또는 온프레미스 서버에서 실행되는 데이터 및 서비스를 오케스트레이션해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Step Functions를 사용하여 애플리케이션을 구축하십시오. 
B. AWS Glue 작업에서 모든 애플리케이션 구성 요소를 통합합니다. 
C. Amazon Simple Queue Service(Amazon SQS)를 사용하여 애플리케이션을 구축합니다. 
D. AWS Lambda 함수와 Amazon EventBridge 이벤트를 사용하여 애플리케이션을 구축합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q500
회사에서 Amazon API Gateway 및 AWS Lambda를 사용하는 공개적으로 액세스 가능한 서버리스 애플리케이션을 실행하고 있습니다. 최근 애플리케이션의 트래픽이 봇넷의 사기성 요 청으로 인해 급증했습니다. 승인되지 않은 사용자의 요청을 차단하기 위해 솔루션 설계자는 어떤 단계를 수행해야 합니까? (두 가지를 선택하세요.)
A. 정품 사용자에게만 공유되는 API 키로 사용량 계획을 생성합니다. 
B. 사기성 IP 주소의 요청을 무시하도록 Lambda 함수 내에 논리를 통합합니다. 
C. 악성 요청을 대상으로 하는 AWS WAF 규칙을 구현하고 이를 필터링하는 작업을 트리거합니다. 
D. 기존 공개 API를 비공개 API로 전환합니다. DNS 레코드를 업데이트하여 사용자를 새 API 엔드포인트로 리디렉션합니다. 
E. API에 액세스를 시도하는 각 사용자에 대해 IAM 역할을 생성합니다. 사용자는 API 호출 시 역할을 맡게 됩니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q501
솔루션 설계자는 Amazon EC2 인스턴스를 호스팅하는 VPC 네트워크를 보호해야 합니다. EC2 인스턴스는 매우 민감한 데이터를 포함하고 프라이빗 서브넷에서 실행됩니다. 회사 정책에 따라 VPC에서 실행되는 EC2 인스턴스는 타사 URL을 사용하는 소프트웨어 제품 업데이트를 위해 인터넷에서 승인된 타사 소프트웨어 리포지토리에만 액세스할 수 있습니다. 다른 인터넷 트래픽은 차단되어야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 아웃바운드 트래픽을 AWS 네트워크 방화벽 방화벽으로 라우팅하도록 프라이빗 서브넷의 라우팅 테이블을 업데이트합니다. 도메인 목록 규칙 그룹을 구성합니다. 
B. AWS WAF 웹 ACL을 설정합니다. 소스 및 대상 IP 주소 범위 집합을 기반으로 트래픽 요청을 필터링하는 사용자 지정 규칙 집합을 만듭니다. 
C. 엄격한 인바운드 보안 그룹 규칙을 구현합니다. URL을 지정하여 인터넷에서 승인된 소프트웨어 리포지토리에 대한 트래픽만 허용하는 아웃바운드 규칙을 구성합니다. 
D. EC2 인스턴스 앞에 Application Load Balancer(ALB)를 구성합니다. 모든 아웃바운드 트래픽을 ALB로 보냅니다. 인터넷에 대한 아웃바운드 액세스를 위해 ALB의 대상 그룹에서
URL 기반 규칙 리스너를 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q502
회사는 데이터 객체를 Amazon S3 Standard 스토리지에 저장합니다. 한 솔루션 설계자는 데이터의 75%가 30일 후에 거의 액세스되지 않는다는 사실을 발견했습니다. 회사는 동일한 고 가용성 및 탄력성으로 모든 데이터에 즉시 액세스할 수 있어야 하지만 스토리지 비용을 최소화하기를 원합니다. 이러한 요구 사항을 충족하는 스토리지 솔루션은 무엇입니까?
A. 30일 후에 데이터 객체를 S3 Glacier Deep Archive로 이동합니다. 
B. 30일 후에 데이터 객체를 S3 Standard-Infrequent Access(S3 Standard-IA)로 이동합니다. 
C. 30일 후에 데이터 객체를 S3 One Zone-Infrequent Access(S3 One Zone-IA)로 이동합니다. 
D. 데이터 객체를 S3 One Zone-Infrequent Access(S3 One Zone-IA)로 즉시 이동합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q503
한 회사에서 로드 밸런싱된 프런트 엔드, 컨테이너 기반 애플리케이션 및 관계형 데이터베이스로 구성될 전자상거래 애플리케이션을 개발하고 있습니다. 솔루션 설계자는 가능한 한 적은 수동 개입으로 작동하는 고가용성 솔루션을 만들어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까? (두 가지를 선택하세요.)
A. 다중 AZ 모드에서 Amazon RDS DB 인스턴스를 생성합니다. 
B. 다른 가용 영역에서 Amazon RDS DB 인스턴스와 하나 이상의 복제본을 생성합니다. 
C. 동적 애플리케이션 로드를 처리하기 위해 Amazon EC2 인스턴스 기반 Docker 클러스터를 생성합니다. 
D. 동적 애플리케이션 로드를 처리하기 위해 Fargate 시작 유형으로 Amazon Elastic Container Service(Amazon ECS) 클러스터를 생성합니다. 
E. 동적 애플리케이션 로드를 처리하기 위해 Amazon EC2 시작 유형으로 Amazon Elastic Container Service(Amazon ECS) 클러스터를 생성합니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q504
회사는 AWS에서 다중 계층 애플리케이션을 호스팅합니다. 규정 준수, 거버넌스, 감사 및 보안을 위해 회사는 AWS 리소스에 대한 구성 변경을 추적하고 이러한 리소스에 대한 API 호출 기 록을 기록해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS CloudTrail을 사용하여 구성 변경을 추적하고 AWS Config를 사용하여 API 호출을 기록합니다. 
B. AWS Config를 사용하여 구성 변경을 추적하고 AWS CloudTrail을 사용하여 API 호출을 기록합니다. 
C. AWS Config를 사용하여 구성 변경을 추적하고 Amazon CloudWatch를 사용하여 API 호출을 기록합니다. 
D. AWS CloudTrail을 사용하여 구성 변경을 추적하고 Amazon CloudWatch를 사용하여 API 호출을 기록합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q505
한 회사가 AWS에서 전자상거래 웹 애플리케이션을 구축하고 있습니다. 애플리케이션은 새 주문에 대한 정보를 Amazon API Gateway REST API로 전송하여 처리합니다. 회사는 주문 이 접수된 순서대로 처리되기를 원합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 애플리케이션이 주문을 받으면 API Gateway 통합을 사용하여 Amazon Simple Notification Service(Amazon SNS) 주제에 메시지를 게시합니다. 처리를 수행할 주제에 대한
AWS Lambda 함수를 구독합니다.
B. 애플리케이션이 주문을 받으면 API Gateway 통합을 사용하여 Amazon Simple Queue Service(Amazon SQS) FIFO 대기열에 메시지를 보냅니다. 처리를 위해 AWS
Lambda 함수를 호출하도록 SQS FIFO 대기열을 구성합니다.
C. 애플리케이션이 주문을 처리하는 동안 API 게이트웨이 권한 부여자를 사용하여 모든 요청을 차단합니다. 
D. 애플리케이션이 주문을 받으면 API Gateway 통합을 사용하여 Amazon Simple Queue Service(Amazon SQS) 표준 대기열로 메시지를 보냅니다. 처리를 위해 AWS
Lambda 함수를 호출하도록 SQS 표준 대기열을 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q506
회사에는 Oracle 데이터베이스를 사용하여 고객 정보를 처리하고 저장하는 온프레미스 서버가 있습니다. 이 회사는 AWS 데이터베이스 서비스를 사용하여 더 높은 가용성을 달성하고 애플리 케이션 성능을 개선하고자 합니다. 회사는 또한 기본 데이터베이스 시스템에서 보고를 오프로드하려고 합니다. 운영상 가장 효율적인 방식으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Database Migration Service(AWS DMS)를 사용하여 여러 AWS 리전에서 Amazon RDS DB 인스턴스를 생성합니다. 보고 기능은 기본 DB 인스턴스와 별도의 DB 인
스턴스를 가리킵니다.
B. 단일 AZ 배포에서 Amazon RDS를 사용하여 Oracle 데이터베이스를 생성합니다. 기본 DB 인스턴스와 동일한 영역에 읽기 전용 복제본을 생성합니다. 보고 기능을 읽기 전용 복제본
으로 지정합니다.
C. 다중 AZ 클러스터 배포에 배포된 Amazon RDS를 사용하여 Oracle 데이터베이스를 생성합니다. 클러스터 배포에서 리더 인스턴스를 사용하도록 보고 기능에 지시합니다. 
D. 다중 AZ 인스턴스 배포에 배포된 Amazon RDS를 사용하여 Amazon Aurora 데이터베이스를 생성합니다. 보고 기능을 판독기 인스턴스에 지시합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q507
회사는 AWS 클라우드에서 다중 계층 전자 상거래 웹 애플리케이션을 실행하고 있습니다. 애플리케이션은 Amazon RDS for MySQL 다중 AZ DB 인스턴스와 함께 Amazon EC2 인스 턴스에서 실행됩니다. Amazon RDS는 범용 SSD(gp3) Amazon Elastic Block Store(Amazon EBS) 볼륨에 2,000GB의 스토리지가 있는 최신 세대 DB 인스턴스로 구성됩니다. 데이터베이스 성능은 수요가 많은 기간 동안 애플리케이션에 영향을 미칩니다. 데이터베이스 관리자는 Amazon CloudWatch Logs의 로그를 분석하고 읽기 및 쓰기 IOPS 수가 20,000보다 높을 때 애플리케이션 성능이 항상 저하됨을 발견합니다. 애플리케이션 성능을 향상시키기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. 볼륨을 마그네틱 볼륨으로 교체합니다. 
B. gp3 볼륨의 IOPS 수를 늘립니다. 
C. 프로비저닝된 IOPS SSD(io2) 볼륨으로 볼륨을 교체합니다. 
D. 2,000GB gp3 볼륨을 두 개의 1,000GB gp3 볼륨으로 교체합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q508
회사에는 탄력적 IP 주소가 있는 퍼블릭 서브넷의 Amazon EC2 인스턴스에서 실행되는 웹 서버가 있습니다. 기본 보안 그룹은 EC2 인스턴스에 할당됩니다. 모든 트래픽을 차단하도록 기본 네트워크 ACL이 수정되었습니다. 솔루션 설계자는 포트 443을 통해 어디에서나 웹 서버에 액세스할 수 있어야 합니다. 이 작업을 수행하는 단계 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 소스 0.0.0.0/0에서 TCP 포트 443을 허용하는 규칙으로 보안 그룹을 생성합니다. 
B. 대상 0.0.0.0/0에 대한 TCP 포트 443을 허용하는 규칙으로 보안 그룹을 생성합니다. 
C. 소스 0.0.0.0/0에서 TCP 포트 443을 허용하도록 네트워크 ACL을 업데이트합니다. 
D. 소스 0.0.0.0/0에서 대상 0.0.0.0/0으로 인바운드/아웃바운드 TCP 포트 443을 허용하도록 네트워크 ACL을 업데이트합니다. 
E. 소스 0.0.0.0/0에서 인바운드 TCP 포트 443을 허용하고 대상 0.0.0.0/0으로 아웃바운드 TCP 포트 32768-65535를 허용하도록 네트워크 ACL을 업데이트합니다.

<details>
<summary>정답 보기</summary>

**AE**
</details>

---

### Q509
회사는 온프레미스에서 다중 계층 웹 애플리케이션을 실행하고 있습니다. 웹 애플리케이션은 컨테이너화되어 있으며 사용자 레코드가 포함된 PostgreSQL 데이터베이스에 연결된 여러 Linux 호스트에서 실행됩니다. 인프라 및 용량 계획을 유지 관리하는 운영 오버헤드는 회사의 성장을 제한하고 있습니다. 솔루션 설계자는 애플리케이션의 인프라를 개선해야 합니다. 이를 달성하기 위해 솔루션 설계자는 어떤 작업 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. PostgreSQL 데이터베이스를 Amazon Aurora로 마이그레이션합니다. 
B. Amazon EC2 인스턴스에서 호스팅할 웹 애플리케이션을 마이그레이션합니다. 
C. 웹 애플리케이션 콘텐츠에 대한 Amazon CloudFront 배포를 설정합니다. 
D. 웹 애플리케이션과 PostgreSQL 데이터베이스 간에 Amazon ElastiCache를 설정합니다. 
E. Amazon Elastic Container Service(Amazon ECS)를 사용하여 AWS Fargate에서 호스팅할 웹 애플리케이션을 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**AE**
</details>

---

### Q510
회사에서 재무 위험 모델링을 위해 AWS에서 고성능 컴퓨팅(HPC) 인프라를 사용하려고 합니다. 회사의 HPC 워크로드는 Linux에서 실행됩니다. 각 HPC 워크플로는 수백 개의 Amazon EC2 스팟 인스턴스에서 실행되고 수명이 짧으며 궁극적으로 분석 및 향후 장기적 사용을 위해 영구 스토리지에 저장되는 수천 개의 출력 파일을 생성합니다. 이 회사는 모든 EC2 인스턴스에서 데이터를 처리할 수 있도록 온프레미스 데이터를 장기 영구 스토리지로 복사할 수 있는 클라우드 스토리지 솔루션을 찾고 있습니다. 솔루션은 또한 데이터 세트와 출력 파일을 읽고 쓰기 위해 영구 스토리지와 통합된 고성능 파일 시스템이어야 합니다. 이러한 요구 사항을 충족하는 AWS 서비스 조합은 무엇입니까?
A. Amazon S3와 통합된 Amazon FSx for Lustre 
B. Amazon S3와 통합된 Windows 파일 서버용 Amazon FSx 
C. Amazon Elastic Block Store(Amazon EBS)와 통합된 Amazon S3 Glacier 
D. Amazon Elastic Block Store(Amazon EBS) 범용 SSD(gp2) 볼륨과 통합된 VPC 엔드포인트가 있는 Amazon S3 버킷

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q511
솔루션 설계자가 새 AWS 계정을 생성했으며 AWS 계정 루트 사용자 액세스를 보호해야 합니다. 어떤 작업 조합이 이를 달성합니까? (두 가지를 선택하세요.)
A. 루트 사용자가 강력한 암호를 사용하는지 확인하십시오. 
B. 루트 사용자에 대한 다단계 인증을 활성화합니다. 
C. 암호화된 Amazon S3 버킷에 루트 사용자 액세스 키를 저장합니다. 
D. 관리 권한이 포함된 그룹에 루트 사용자를 추가합니다. 
E. 인라인 정책 문서를 사용하여 루트 사용자에게 필요한 권한을 적용합니다.

<details>
<summary>정답 보기</summary>

**AB**
</details>

---

### Q512
한 회사가 온프레미스에서 컨테이너화된 애플리케이션을 구축하고 애플리케이션을 AWS로 이전하기로 결정했습니다. 응용 프로그램은 배포된 직후 수천 명의 사용자를 보유하게 됩니다. 회사 는 규모에 맞게 컨테이너 배포를 관리하는 방법을 확신하지 못합니다. 회사는 운영 오버헤드를 최소화하는 고가용성 아키텍처에 컨테이너화된 애플리케이션을 배포해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Elastic Container Registry(Amazon ECR) 리포지토리에 컨테이너 이미지를 저장합니다. AWS Fargate 시작 유형과 함께 Amazon Elastic Container Service
(Amazon ECS) 클러스터를 사용하여 컨테이너를 실행합니다. 대상 추적을 사용하여 수요에 따라 자동으로 확장합니다.
B. 컨테이너 이미지를 Amazon Elastic Container Registry(Amazon ECR) 리포지토리에 저장합니다. Amazon EC2 시작 유형과 함께 Amazon Elastic Container Service
(Amazon ECS) 클러스터를 사용하여 컨테이너를 실행합니다. 대상 추적을 사용하여 수요에 따라 자동으로 확장합니다.
C. Amazon EC2 인스턴스에서 실행되는 리포지토리에 컨테이너 이미지를 저장합니다. 여러 가용 영역에 분산된 EC2 인스턴스에서 컨테이너를 실행합니다. Amazon CloudWatch에서
평균 CPU 사용률을 모니터링합니다. 필요에 따라 새 EC2 인스턴스를 시작합니다.
D. 컨테이너 이미지가 포함된 Amazon EC2 Amazon 머신 이미지(AMI)를 생성합니다. 여러 가용 영역의 Auto Scaling 그룹에서 EC2 인스턴스를 시작합니다. 평균 CPU 사용률 임계
값을 초과하면 Amazon CloudWatch 경보를 사용하여 EC2 인스턴스를 확장합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q513
회사에서 내부 브라우저 기반 애플리케이션을 실행합니다. 애플리케이션은 Application Load Balancer 뒤의 Amazon EC2 인스턴스에서 실행됩니다. 인스턴스는 여러 가용 영역에 걸쳐 Amazon EC2 Auto Scaling 그룹에서 실행됩니다. Auto Scaling 그룹은 근무 시간 동안 최대 20개의 인스턴스로 확장되지만 밤에는 2개의 인스턴스로 축소됩니다. 오전 중반까지는 잘 돌아가는데도 하루가 시작되면 애플리케이션이 매우 느리다고 직원들이 불평하고 있다. 직원 불만을 해결하고 비용을 최소화하기 위해 확장을 어떻게 변경해야 합니까?
A. 사무실이 열리기 직전에 원하는 수용 인원을 20명으로 설정하는 예약 작업을 구현합니다. 
B. 더 낮은 CPU 임계값에서 트리거되는 단계 조정 작업을 구현하고 휴지 기간을 줄입니다. 
C. 더 낮은 CPU 임계값에서 트리거되는 대상 추적 작업을 구현하고 휴지 기간을 줄입니다. 
D. 사무실이 열리기 직전에 최소 및 최대 수용 인원을 20명으로 설정하는 예약 조치를 구현합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q514
한 온라인 소매 회사는 5천만 명 이상의 활성 고객을 보유하고 있으며 매일 25,000건 이상의 주문을 받습니다. 회사는 고객의 구매 데이터를 수집하고 이 데이터를 Amazon S3에 저장합니 다. 추가 고객 데이터는 Amazon RDS에 저장됩니다. 회사는 팀이 분석을 수행할 수 있도록 다양한 팀에서 모든 데이터를 사용할 수 있도록 하려고 합니다. 솔루션은 데이터에 대한 세분화된 권한을 관리하는 기능을 제공하고 운영 오버헤드를 최소 화해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 구매 데이터를 마이그레이션하여 Amazon RDS에 직접 씁니다. RDS 액세스 제어를 사용하여 액세스를 제한하십시오. 
B. Amazon RDS에서 Amazon S3로 데이터를 주기적으로 복사하도록 AWS Lambda 함수를 예약합니다. AWS Glue 크롤러를 생성합니다. Amazon Athena를 사용하여 데이터를
쿼리합니다. S3 정책을 사용하여 액세스를 제한하십시오.
C. AWS Lake Formation을 사용하여 데이터 레이크를 생성합니다. Amazon RDS에 대한 AWS Glue JDBC 연결을 생성합니다. Lake Formation에 S3 버킷을 등록합니다.
Lake Formation 액세스 제어를 사용하여 액세스를 제한하십시오.
D. Amazon Redshift 클러스터를 생성합니다. Amazon S3 및 Amazon RDS에서 Amazon Redshift로 데이터를 주기적으로 복사하도록 AWS Lambda 함수를 예약합니다.
Amazon Redshift 액세스 제어를 사용하여 액세스를 제한하십시오.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q515
회사에서 애플리케이션을 설계하고 있습니다. 애플리케이션은 AWS Lambda 함수를 사용하여 Amazon API Gateway를 통해 정보를 수신하고 Amazon Aurora PostgreSQL 데이터 베이스에 정보를 저장합니다. 개념 증명 단계에서 회사는 데이터베이스에 로드해야 하는 대량의 데이터를 처리하기 위해 Lambda 할당량을 크게 늘려야 합니다. 솔루션 설계자는 확장성을 개선하고 구성 노력을 최소화하 기 위해 새로운 설계를 권장해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Lambda 함수 코드를 Amazon EC2 인스턴스에서 실행되는 Apache Tomcat 코드로 리팩터링합니다. 원시 JDBC(Java Database Connectivity) 드라이버를 사용하여 데이터
베이스를 연결하십시오.
B. Aurora에서 DynamoDB Accelerator(DAX) 클러스터를 Amazon DynamoDProvision으로 플랫폼을 변경합니다. DAX 클라이언트 SDK를 사용하여 DAX 클러스터에서 기존
DynamoDB API 호출을 가리킵니다.
C. 두 개의 Lambda 함수를 설정합니다. 정보를 수신하도록 하나의 기능을 구성합니다. 데이터베이스에 정보를 로드하도록 다른 기능을 구성하십시오. Amazon Simple Notification
Service(Amazon SNS)를 사용하여 Lambda 함수를 통합합니다.
D. 두 개의 Lambda 함수를 설정합니다. 정보를 수신하도록 하나의 기능을 구성합니다. 데이터베이스에 정보를 로드하도록 다른 기능을 구성하십시오. Amazon Simple Queue Service
(Amazon SQS) 대기열을 사용하여 Lambda 함수를 통합합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q516
회사는 다른 팀이 액세스할 수 있도록 하루에 한 번씩 데이터베이스를 Amazon S3로 내보내야 합니다. 내보낸 객체 크기는 2GB에서 5GB 사이입니다. 데이터에 대한 S3 액세스 패턴은 가 변적이며 빠르게 변화합니다. 데이터는 즉시 사용할 수 있어야 하며 최대 3개월 동안 액세스할 수 있어야 합니다. 회사에는 검색 시간을 늘리지 않는 가장 비용 효율적인 솔루션이 필요합니다. 이러한 요구 사항을 충족하려면 회사에서 어떤 S3 스토리지 클래스를 사용해야 합니까?
A. S3 지능형 계층화 
B. S3 Glacier 즉시 검색 
C. S3 표준 
D. S3 Standard-Infrequent Access(S3 스탠다드-IA)

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q517
회사는 단일 가용 영역의 Amazon RDS for MySQL DB 인스턴스에 저장된 온라인 광고 비즈니스용 대규모 데이터 세트를 보유하고 있습니다. 회사는 프로덕션 DB 인스턴스에 대한 쓰기 작업에 영향을 주지 않고 비즈니스 보고 쿼리를 실행하기를 원합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. RDS 읽기 복제본을 배포하여 비즈니스 보고 쿼리를 처리합니다. 
B. DB 인스턴스를 Elastic Load Balancer 뒤에 배치하여 수평으로 확장합니다. 
C. DB 인스턴스를 더 큰 인스턴스 유형으로 확장하여 쓰기 작업 및 쿼리를 처리합니다. 
D. 비즈니스 보고 쿼리를 처리하기 위해 여러 가용 영역에 DB 인스턴스를 배포합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q518
회사는 Application Load Balancer(ALB) 뒤에 있는 Amazon EC2 인스턴스 플릿에서 동적 웹 사이트를 제공합니다. 웹 사이트는 전 세계 고객에게 서비스를 제공하기 위해 여러 언어를 지원해야 합니다. 웹 사이트의 아키텍처는 us-west-1 지역에서 실행 중이며 세계의 다른 지역에 있는 사용자에 대해 높은 요청 지연 시간을 보이고 있습니다. 웹사이트는 사용자의 위치에 관계없이 빠르고 효율적으로 요청을 처리해야 합니다. 그러나 회사는 여러 지역에 걸쳐 기존 아키텍처를 다시 생성하기를 원하지 않습니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 기존 아키텍처를 Amazon S3 버킷에서 제공되는 웹 사이트로 교체하십시오. S3 버킷을 오리진으로 사용하여 Amazon CloudFront 배포를 구성합니다. Accept-Language 요청 헤
더를 기반으로 캐시 동작 설정을 캐시로 설정합니다.
B. ALB를 오리진으로 사용하여 Amazon CloudFront 배포를 구성합니다. Accept-Language 요청 헤더를 기반으로 캐시 동작 설정을 캐시로 설정합니다. 
C. ALB와 통합되는 Amazon API Gateway API를 생성합니다. HTTP 통합 유형을 사용하도록 API를 구성합니다. Accept-Language 요청 헤더를 기반으로 API 캐시를 활성화하도
록 API Gateway 단계를 설정합니다.
D. 각 추가 지역에서 EC2 인스턴스를 시작하고 해당 지역의 캐시 서버 역할을 하도록 NGINX를 구성합니다. 지리적 위치 라우팅 정책을 사용하여 Amazon Route 53 레코드 세트 뒤에
모든 EC2 인스턴스와 ALB를 배치합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q519
한 회사에서 여러 프로덕션 애플리케이션을 호스팅합니다. 애플리케이션 중 하나는 여러 AWS 리전에서 Amazon EC2, AWS Lambda, Amazon RDS, Amazon Simple Notification Service(Amazon SNS) 및 Amazon Simple Queue Service(Amazon SQS)의 리소스로 구성됩니다. 모든 회사 리소스에는 "응용 프로그램"이라는 태그 이름과 각 응 용 프로그램에 해당하는 값이 태그로 지정됩니다. 솔루션 설계자는 태그가 지정된 모든 구성 요소를 식별하기 위한 가장 빠른 솔루션을 제공해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS CloudTrail을 사용하여 애플리케이션 태그가 있는 리소스 목록을 생성합니다. 
B. AWS CLI를 사용하여 모든 리전에서 각 서비스를 쿼리하여 태그가 지정된 구성 요소를 보고합니다. 
C. Amazon CloudWatch Logs Insights에서 쿼리를 실행하여 애플리케이션 태그가 있는 구성 요소에 대해 보고합니다. 
D. AWS Resource Groups Tag Editor로 쿼리를 실행하여 애플리케이션 태그를 사용하여 전역적으로 리소스에 대해 보고합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q520
회사에 모바일 앱을 사용하는 백만 명의 사용자가 있습니다. 회사는 거의 실시간으로 데이터 사용량을 분석해야 합니다. 회사는 또한 거의 실시간으로 데이터를 암호화하고 추가 처리를 위해 데 이터를 Apache Parquet 형식의 중앙 위치에 저장해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Kinesis 데이터 스트림을 생성하여 Amazon S3에 데이터를 저장합니다. 데이터를 분석할 Amazon Kinesis Data Analytics 애플리케이션을 생성합니다. AWS
Lambda 함수를 호출하여 데이터를 Kinesis Data Analytics 애플리케이션으로 보냅니다.
B. Amazon Kinesis 데이터 스트림을 생성하여 Amazon S3에 데이터를 저장합니다. 데이터를 분석할 Amazon EMR 클러스터를 생성합니다. AWS Lambda 함수를 호출하여 데이
터를 EMR 클러스터로 보냅니다.
C. Amazon Kinesis Data Firehose 전송 스트림을 생성하여 Amazon S3에 데이터를 저장합니다. 데이터를 분석할 Amazon EMR 클러스터를 생성합니다. 
D. Amazon Kinesis Data Firehose 전송 스트림을 생성하여 Amazon S3에 데이터를 저장합니다. 데이터를 분석할 Amazon Kinesis Data Analytics 애플리케이션을 생성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q521
회사의 주문 시스템은 클라이언트의 요청을 Amazon EC2 인스턴스로 보냅니다. EC2 인스턴스는 주문을 처리한 다음 Amazon RDS의 데이터베이스에 주문을 저장합니다. 사용자는 시스 템이 실패하면 주문을 다시 처리해야 한다고 보고합니다. 회사는 시스템 중단이 발생할 경우 주문을 자동으로 처리할 수 있는 탄력적인 솔루션을 원합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. EC2 인스턴스를 Auto Scaling 그룹으로 이동합니다. Amazon Elastic Container Service(Amazon ECS) 작업을 대상으로 하는 Amazon EventBridge(Amazon
CloudWatch Events) 규칙을 생성합니다.
B. Application Load Balancer(ALB) 뒤에 있는 Auto Scaling 그룹으로 EC2 인스턴스를 이동합니다. ALB 엔드포인트에 메시지를 보내도록 주문 시스템을 업데이트합니다. 
C. EC2 인스턴스를 Auto Scaling 그룹으로 이동합니다. Amazon Simple Queue Service(Amazon SQS) 대기열로 메시지를 보내도록 주문 시스템을 구성합니다. 대기열의 메시지
를 사용하도록 EC2 인스턴스를 구성합니다.
D. Amazon Simple Notification Service(Amazon SNS) 주제를 생성합니다. AWS Lambda 함수를 생성하고 함수를 SNS 주제에 구독합니다. SNS 주제에 메시지를 보내도록 주
문 시스템을 구성합니다. AWS Systems Manager Run Command를 사용하여 메시지를 처리하도록 EC2 인스턴스에 명령을 보냅니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q522
회사에서 Amazon ECS를 사용하여 애플리케이션을 실행합니다. 애플리케이션은 원본 이미지의 크기가 조정된 버전을 생성한 다음 Amazon S3 API를 호출하여 크기가 조정된 이미지를 Amazon S3에 저장합니다. 솔루션 설계자는 애플리케이션이 Amazon S3에 액세스할 권한이 있는지 어떻게 확인할 수 있습니까?
A. Amazon ECS에서 읽기/쓰기 액세스를 허용하도록 AWS IAM에서 S3 역할을 업데이트한 다음 컨테이너를 다시 시작합니다. 
B. S3 권한이 있는 IAM 역할을 생성한 다음 작업 정의에서 해당 역할을 taskRoleArn으로 지정합니다. 
C. Amazon ECS에서 Amazon S3로의 액세스를 허용하는 보안 그룹을 생성하고 ECS 클러스터에서 사용하는 시작 구성을 업데이트합니다. 
D. S3 권한이 있는 IAM 사용자를 만든 다음 이 계정으로 로그인한 상태에서 ECS 클러스터에 대한 Amazon EC2 인스턴스를 다시 시작합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q523
회사에서 모바일 앱 사용자를 대상으로 하는 마케팅 커뮤니케이션 서비스를 개발하고 있습니다. 회사는 SMS(Short Message Service)를 통해 사용자에게 확인 메시지를 보내야 합니다. 사용자는 SMS 메시지에 회신할 수 있어야 합니다. 회사는 분석을 위해 응답을 1년 동안 저장해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Amazon Connect 통화 흐름을 생성하여 SMS 메시지를 보냅니다. AWS Lambda를 사용하여 응답을 처리합니다. 
B. Amazon Pinpoint 여정을 구축하십시오. 분석 및 보관을 위해 이벤트를 Amazon Kinesis 데이터 스트림으로 보내도록 Amazon Pinpoint를 구성합니다. 
C. Amazon Simple Queue Service(Amazon SQS)를 사용하여 SMS 메시지를 배포합니다. AWS Lambda를 사용하여 응답을 처리합니다. 
D. Amazon Simple Notification Service(Amazon SNS) FIFO 주제를 생성합니다. 분석 및 보관을 위해 Amazon Kinesis 데이터 스트림을 SNS 주제에 구독합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q524
회사에서 Amazon EC2 데이터 및 여러 Amazon S3 버킷에 대한 백업 전략을 구현하려고 합니다. 규정 요구 사항으로 인해 회사는 특정 기간 동안 백업 파일을 보존해야 합니다. 회사는 보 유기간 동안 파일을 변조해서는 안됩니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Backup을 사용하여 거버넌스 모드에서 볼트 잠금이 있는 백업 볼트를 생성합니다. 필요한 백업 계획을 생성합니다. 
B. Amazon Data Lifecycle Manager를 사용하여 필요한 자동 스냅샷 정책을 생성합니다. 
C. Amazon S3 파일 게이트웨이를 사용하여 백업을 생성합니다. 적절한 S3 수명 주기 관리를 구성합니다. 
D. AWS Backup을 사용하여 규정 준수 모드에서 볼트 잠금이 있는 백업 볼트를 생성합니다. 필요한 백업 계획을 생성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q525
회사는 AWS에서 2계층 전자 상거래 웹 사이트를 운영합니다. 웹 계층은 트래픽을 Amazon EC2 인스턴스로 보내는 로드 밸런서로 구성됩니다. 데이터베이스 계층은 Amazon RDS DB 인스턴스를 사용합니다. EC2 인스턴스와 RDS DB 인스턴스는 퍼블릭 인터넷에 노출되어서는 안 됩니다. EC2 인스턴스는 타사 웹 서비스를 통해 주문 결제 처리를 완료하기 위해 인터넷 액 세스가 필요합니다. 애플리케이션은 고가용성이어야 합니다. 이러한 요구 사항을 충족하는 구성 옵션 조합은 무엇입니까? (두 가지를 선택하세요.)
A. Auto Scaling 그룹을 사용하여 프라이빗 서브넷에서 EC2 인스턴스를 시작합니다. 프라이빗 서브넷에 RDS 다중 AZ DB 인스턴스를 배포합니다.
B. 2개의 가용 영역에 걸쳐 2개의 프라이빗 서브넷과 2개의 NAT 게이트웨이로 VPC를 구성합니다. 프라이빗 서브넷에 Application Load Balancer를 배포합니다.
C. Auto Scaling 그룹을 사용하여 두 가용 영역의 퍼블릭 서브넷에서 EC2 인스턴스를 시작합니다. 프라이빗 서브넷에 RDS 다중 AZ DB 인스턴스를 배포합니다.
D. 퍼블릭 서브넷 1개, 프라이빗 서브넷 1개, 2개의 가용 영역에 걸친 NAT 게이트웨이 2개로 VPC를 구성합니다. 퍼블릭 서브넷에 Application Load Balancer를 배포합니다.
E. 2개의 가용 영역에 걸친 2개의 퍼블릭 서브넷, 2개의 프라이빗 서브넷 및 2개의 NAT 게이트웨이로 VPC를 구성합니다. 퍼블릭 서브넷에 Application Load Balancer를 배포합니다.

<details>
<summary>정답 보기</summary>

**AE**
</details>

---

### Q526
한 회사가 최근 다른 AWS 리전에 재해 복구 사이트를 만들었습니다. 회사는 정기적으로 두 리전의 NFS 파일 시스템 간에 대량의 데이터를 주고 받아야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS DataSync를 사용하십시오. 
B. AWS Snowball 디바이스를 사용합니다. 
C. Amazon EC2에서 SFTP 서버를 설정합니다. 
D. AWS 데이터베이스 마이그레이션 서비스(AWS DMS)를 사용합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q527
회사에서 AWS에 웹 애플리케이션을 배포했습니다. 이 회사는 조정 요구 사항을 지원하기 위해 기본 DB 인스턴스와 5개의 읽기 전용 복제본을 사용하여 MySQL용 Amazon RDS에서 백 엔드 데이터베이스를 호스팅합니다. 읽기 전용 복제본은 기본 DB 인스턴스보다 1초 이상 뒤처져서는 안 됩니다. 데이터베이스는 정기적으로 예약된 저장 프로시저를 실행합니다. 웹 사이트의 트래픽이 증가함에 따라 복제본은 피크 로드 기간 동안 추가 지연을 경험합니다. 솔루션 설계자는 복제 지연을 최대한 줄여야 합니다. 솔루션 설계자는 애플리케이션 코드에 대한 변경을 최소화하고 지속적인 운영 오버헤드를 최소화해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 데이터베이스를 Amazon Aurora MySQL로 마이그레이션합니다. 읽기 전용 복제본을 Aurora 복제본으로 교체하고 Aurora Auto Scaling을 구성합니다. 저장 프로시저를 Aurora
MySQL 기본 함수로 바꿉니다.
B. 데이터베이스 앞에 Redis 클러스터용 Amazon ElastiCache를 배포합니다. 응용 프로그램이 데이터베이스를 쿼리하기 전에 캐시를 확인하도록 응용 프로그램을 수정하십시오. 저장
프로시저를 AWS Lambda 함수로 바꿉니다.
C. 데이터베이스를 Amazon EC2 인스턴스에서 실행되는 MySQL 데이터베이스로 마이그레이션합니다. 모든 복제본 노드에 대해 컴퓨팅에 최적화된 대규모 EC2 인스턴스를 선택합니다.
EC2 인스턴스에서 저장 프로시저를 유지합니다.
D. 데이터베이스를 Amazon DynamoDB로 마이그레이션합니다. 필요한 처리량을 지원하고 온디맨드 용량 확장을 구성하기 위해 많은 수의 RCU(읽기 용량 단위)를 프로비저닝합니다.
저장 프로시저를 DynamoDB 스트림으로 바꿉니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q528
회사에 AWS로 마이그레이션해야 하는 Windows 기반 애플리케이션이 있습니다. 이 애플리케이션은 여러 가용 영역에 배포된 여러 Amazon EC2 Windows 인스턴스에 연결된 공유 Windows 파일 시스템을 사용해야 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 볼륨 게이트웨이 모드에서 AWS Storage Gateway를 구성합니다. 각 Windows 인스턴스에 볼륨을 마운트합니다. 
B. Windows 파일 서버용 Amazon FSx를 구성합니다. Amazon FSx 파일 시스템을 각 Windows 인스턴스에 탑재합니다. 
C. Amazon Elastic File System(Amazon EFS)을 사용하여 파일 시스템을 구성합니다. EFS 파일 시스템을 각 Windows 인스턴스에 마운트합니다. 
D. 필요한 크기로 Amazon Elastic Block Store(Amazon EBS) 볼륨을 구성합니다. 각 EC2 인스턴스를 볼륨에 연결합니다. 볼륨 내의 파일 시스템을 각 Windows 인스턴스에 마운
트합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q529
한 회사가 최근 AWS 계정의 Amazon EC2 인스턴스에서 다양한 새 워크로드를 시작했습니다. 회사는 인스턴스를 원격으로 안전하게 액세스하고 관리하기 위한 전략을 수립해야 합니다. 회 사는 기본 AWS 서비스와 함께 작동하고 AWS Well-Architected 프레임워크를 따르는 반복 가능한 프로세스를 구현해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 관리를 위해 각 인스턴스의 터미널 인터페이스에 직접 액세스하려면 EC2 직렬 콘솔을 사용하십시오. 
B. 각각의 기존 인스턴스와 새 인스턴스에 적절한 IAM 역할을 연결합니다. AWS Systems Manager Session Manager를 사용하여 원격 SSH 세션을 설정합니다. 
C. 관리 SSH 키 쌍을 만듭니다. 퍼블릭 키를 각 EC2 인스턴스에 로드합니다. 퍼블릭 서브넷에 배스천 호스트를 배포하여 각 인스턴스 관리를 위한 터널을 제공합니다. 
D. AWS Site-to-Site VPN 연결을 설정합니다. 관리자에게 로컬 온프레미스 시스템을 사용하여 VPN 터널에서 SSH 키를 사용하여 인스턴스에 직접 연결하도록 지시합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q530
회사에서 Amazon S3 Standard 스토리지를 사용하여 백업 파일을 저장하고 있습니다. 1개월 동안 파일에 자주 액세스합니다. 그러나 1개월이 지나면 파일에 액세스하지 않습니다. 회사는 파일을 무기한으로 보관해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 스토리지 솔루션은 무엇입니까?
A. 개체를 자동으로 마이그레이션하도록 S3 Intelligent-Tiering을 구성합니다. 
B. 1개월 후에 객체를 S3 Standard에서 S3 Glacier Deep Archive로 전환하는 S3 수명 주기 구성을 생성합니다. 
C. 1개월 후 객체를 S3 Standard에서 S3 Standard-Infrequent Access(S3 Standard-IA)로 전환하는 S3 수명 주기 구성을 생성합니다. 
D. 1개월 후에 객체를 S3 Standard에서 S3 One Zone-Infrequent Access(S3 One Zone-IA)로 전환하는 S3 수명 주기 구성을 생성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q531
회사에는 매일 총 1TB의 상태 알림을 생성하는 수천 개의 에지 장치가 있습니다. 각 알림의 크기는 약 2KB입니다. 솔루션 설계자는 향후 분석을 위해 경고를 수집하고 저장하는 솔루션을 구 현해야 합니다. 회사는 고가용성 솔루션을 원합니다. 그러나 회사는 비용을 최소화해야 하며 추가 인프라를 관리하기를 원하지 않습니다. 또한 회사는 즉각적인 분석을 위해 14일간의 데이터를 유지하고 14일 보다 오래된 모든 데이터를 보관하기를 원합니다. 이러한 요구 사항을 충족하는 운영상 가장 효율적인 솔루션은 무엇입니까?
A. Amazon Kinesis Data Firehose 전송 스트림을 생성하여 알림을 수집합니다. Amazon S3 버킷에 알림을 전달하도록 Kinesis Data Firehose 스트림을 구성합니다. 14일 후에
데이터를 Amazon S3 Glacier로 전환하도록 S3 수명 주기 구성을 설정합니다.
B. 두 가용 영역에서 Amazon EC2 인스턴스를 시작하고 이를 Elastic Load Balancer 뒤에 배치하여 알림을 수집합니다. Amazon S3 버킷에 알림을 저장할 EC2 인스턴스에서 스크
립트를 생성합니다. 14일 후에 데이터를 Amazon S3 Glacier로 전환하도록 S3 수명 주기 구성을 설정합니다.
C. Amazon Kinesis Data Firehose 전송 스트림을 생성하여 알림을 수집합니다. Amazon OpenSearch Service(Amazon Elasticsearch Service) 클러스터에 알림을 전달하
도록 Kinesis Data Firehose 스트림을 구성합니다. 매일 수동 스냅샷을 생성하고 14일보다 오래된 클러스터에서 데이터를 삭제하도록 Amazon OpenSearch Service(Amazon Elasticsearch Service) 클러스터를 설정합니다.
D. 알림을 수집할 Amazon Simple Queue Service(Amazon SQS) 표준 대기열을 생성하고 메시지 보존 기간을 14일로 설정합니다. 소비자가 SQS 대기열을 폴링하고 메시지 수명
을 확인하고 필요에 따라 메시지 데이터를 분석하도록 구성합니다. 메시지가 14일이 지난 경우 소비자는 메시지를 Amazon S3 버킷에 복사하고 SQS 대기열에서 메시지를 삭제해야 합 니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q532
솔루션 설계자는 퍼블릭 및 프라이빗 서브넷이 있는 VPC를 설계하고 있습니다. VPC와 서브넷은 IPv4 CIDR 블록을 사용합니다. 고가용성을 위해 3개의 가용 영역(AZ) 각각에 퍼블릭 서 브넷 1개와 프라이빗 서브넷 1개가 있습니다. 인터넷 게이트웨이는 퍼블릭 서브넷에 대한 인터넷 액세스를 제공하는 데 사용됩니다. 프라이빗 서브넷은 Amazon EC2 인스턴스가 소프트웨 어 업데이트를 다운로드할 수 있도록 인터넷에 액세스해야 합니다. 사설 서브넷에 대한 인터넷 액세스를 활성화하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 각 AZ의 퍼블릭 서브넷마다 하나씩 세 개의 NAT 게이트웨이를 생성합니다. 비 VPC 트래픽을 해당 AZ의 NAT 게이트웨이로 전달하는 각 AZ에 대한 프라이빗 라우팅 테이블을 생성합
니다.
B. 각 AZ의 각 프라이빗 서브넷에 대해 하나씩 세 개의 NAT 인스턴스를 만듭니다. 비 VPC 트래픽을 해당 AZ의 NAT 인스턴스로 전달하는 각 AZ에 대한 프라이빗 라우팅 테이블을 생성
합니다.
C. 프라이빗 서브넷 중 하나에 두 번째 인터넷 게이트웨이를 만듭니다. VPC가 아닌 트래픽을 프라이빗 인터넷 게이트웨이로 전달하는 프라이빗 서브넷의 라우팅 테이블을 업데이트합니다. 
D. 퍼블릭 서브넷 중 하나에 외부 전용 인터넷 게이트웨이를 만듭니다. 비 VPC 트래픽을 외부 전용 인터넷 게이트웨이로 전달하는 프라이빗 서브넷의 라우팅 테이블을 업데이트합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q533
회사에서 Amazon ECS를 사용하여 애플리케이션을 실행합니다. 애플리케이션은 원본 이미지의 크기가 조정된 버전을 생성한 다음 Amazon S3 API를 호출하여 크기가 조정된 이미지를 Amazon S3에 저장합니다. 솔루션 설계자는 애플리케이션이 Amazon S3에 액세스할 권한이 있는지 어떻게 확인할 수 있습니까?
A. Amazon ECS에서 읽기/쓰기 액세스를 허용하도록 AWS IAM에서 S3 역할을 업데이트한 다음 컨테이너를 다시 시작합니다. 
B. S3 권한이 있는 IAM 역할을 생성한 다음 작업 정의에서 해당 역할을 taskRoleArn으로 지정합니다. 
C. Amazon ECS에서 Amazon S3로의 액세스를 허용하는 보안 그룹을 생성하고 ECS 클러스터에서 사용하는 시작 구성을 업데이트합니다. 
D. S3 권한이 있는 IAM 사용자를 만든 다음 이 계정으로 로그인한 상태에서 ECS 클러스터에 대한 Amazon EC2 인스턴스를 다시 시작합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q534
솔루션 설계자는 공용 서브넷과 데이터베이스 서브넷을 포함하는 2계층 아키텍처를 설계하고 있습니다. 퍼블릭 서브넷의 웹 서버는 포트 443에서 인터넷에 열려 있어야 합니다. 데이터베이스 서브넷의 Amazon RDS for MySQL DB 인스턴스는 포트 3306의 웹 서버에서만 액세스할 수 있어야 합니다. 솔루션 설계자가 수행해야 하는 단계의 조합은 무엇입니까? 이러한 요구 사항을 충족합니까? (두 가지를 선택하세요.)
A. 퍼블릭 서브넷에 대한 네트워크 ACL을 만듭니다. 포트 3306에서 0.0.0.0/0에 대한 아웃바운드 트래픽을 거부하는 규칙을 추가합니다.
B. DB 인스턴스에 대한 보안 그룹을 생성합니다. 포트 3306에서 퍼블릭 서브넷 CIDR 블록의 트래픽을 허용하는 규칙을 추가합니다.
C. 퍼블릭 서브넷의 웹 서버에 대한 보안 그룹을 생성합니다. 포트 443에서 0.0.0.0/0의 트래픽을 허용하는 규칙을 추가합니다.
D. DB 인스턴스에 대한 보안 그룹을 생성합니다. 포트 3306에서 웹 서버 보안 그룹의 트래픽을 허용하는 규칙을 추가합니다.
E. DB 인스턴스에 대한 보안 그룹을 생성합니다. 포트 3306에서 웹 서버 보안 그룹의 트래픽을 제외한 모든 트래픽을 거부하는 규칙을 추가합니다.

<details>
<summary>정답 보기</summary>

**CD**
</details>

---

### Q535
회사에는 수명이 다한 온프레미스 볼륨 백업 솔루션이 있습니다. 회사는 AWS를 새로운 백업 솔루션의 일부로 사용하고 AWS에 백업되는 동안 모든 데이터에 대한 로컬 액세스를 유지하려고 합니다. 회사는 AWS에 백업된 데이터가 자동으로 안전하게 전송되기를 원합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. AWS Snowball을 사용하여 온프레미스 솔루션에서 Amazon S3로 데이터를 마이그레이션합니다. 데이터에 대한 로컬 액세스를 제공하기 위해 Snowball S3 엔드포인트를 탑재하도
록 온프레미스 시스템을 구성합니다.
B. AWS Snowball Edge를 사용하여 온프레미스 솔루션에서 Amazon S3로 데이터를 마이그레이션합니다. Snowball Edge 파일 인터페이스를 사용하여 온프레미스 시스템에 데이터
에 대한 로컬 액세스를 제공합니다.
C. AWS Storage Gateway를 사용하고 캐시된 볼륨 게이트웨이를 구성합니다. 온프레미스에서 Storage Gateway 소프트웨어 어플라이언스를 실행하고 로컬로 캐시할 데이터 비율을
구성합니다. 데이터에 대한 로컬 액세스를 제공하기 위해 게이트웨이 스토리지 볼륨을 마운트합니다.
D. AWS Storage Gateway를 사용하고 저장된 볼륨 게이트웨이를 구성합니다. 온프레미스에서 Storage Gateway 소프트웨어 어플라이언스를 실행하고 게이트웨이 스토리지 볼륨을
온프레미스 스토리지에 매핑합니다. 데이터에 대한 로컬 액세스를 제공하기 위해 게이트웨이 스토리지 볼륨을 마운트합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q536
회사에서 애플리케이션을 서버리스 솔루션으로 이동하려고 합니다. 서버리스 솔루션은 SL을 사용하여 기존 및 신규 데이터를 분석해야 합니다. 회사는 데이터를 Amazon S3 버킷에 저장합 니다. 데이터는 암호화가 필요하며 다른 AWS 리전에 복제되어야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 새 S3 버킷을 생성합니다. 새 S3 버킷에 데이터를 로드합니다. S3 교차 리전 복제(CRR)를 사용하여 암호화된 객체를 다른 리전의 S3 버킷에 복제합니다. AWS KMS 다중 리전 키
(SSE-KMS)로 서버 측 암호화를 사용합니다. Amazon Athena를 사용하여 데이터를 쿼리합니다.
B. 새 S3 버킷을 생성합니다. 새 S3 버킷에 데이터를 로드합니다. S3 CRR(Cross-Region Replication)을 사용하여 암호화된 객체를 다른 리전의 S3 버킷에 복제합니다. AWS KMS
다중 리전 키(SSE-KMS)로 서버 측 암호화를 사용합니다. Amazon RDS를 사용하여 데이터를 쿼리합니다.
C. 기존 S3 버킷에 데이터를 로드합니다. S3 CRR(Cross-Region Replication)을 사용하여 암호화된 객체를 다른 리전의 S3 버킷에 복제합니다. Amazon S3 관리형 암호화 키
(SSE-S3)로 서버 측 암호화를 사용합니다. Amazon Athena를 사용하여 데이터를 쿼리합니다.
D. 기존 S3 버킷에 데이터를 로드합니다. S3 CRR(Cross-Region Replication)을 사용하여 암호화된 객체를 다른 리전의 S3 버킷에 복제합니다. Amazon S3 관리형 암호화 키
(SSE-S3)로 서버 측 암호화를 사용합니다. Amazon RDS를 사용하여 데이터를 쿼리합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q537
회사가 AWS 클라우드에서 애플리케이션을 구축하고 있습니다. 애플리케이션은 두 AWS 리전의 Amazon S3 버킷에 데이터를 저장합니다. 회사는 AWS Key Management Service (AWS KMS) 고객 관리형 키를 사용하여 S3 버킷에 저장된 모든 데이터를 암호화해야 합니다. 두 S3 버킷의 데이터는 동일한 KMS 키로 암호화 및 암호 해독되어야 합니다. 데이터와 키는 두 지역 각각에 저장되어야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 각 리전에서 S3 버킷을 생성합니다. Amazon S3 관리형 암호화 키(SSE-S3)로 서버 측 암호화를 사용하도록 S3 버킷을 구성합니다. S3 버킷 간의 복제를 구성합니다. 
B. 고객 관리 다중 리전 KMS 키를 생성합니다. 각 리전에서 S3 버킷을 생성합니다. S3 버킷 간의 복제를 구성합니다. 클라이언트 측 암호화와 함께 KMS 키를 사용하도록 애플리케이션을
구성합니다.
C. 각 리전에서 고객 관리형 KMS 키와 S3 버킷을 생성합니다. Amazon S3 관리형 암호화 키(SSE-S3)로 서버 측 암호화를 사용하도록 S3 버킷을 구성합니다. S3 버킷 간의 복제를 구
성합니다.
D. 각 리전에서 고객 관리형 KMS 키와 S3 버킷을 생성합니다. AWS KMS 키(SSE-KMS)로 서버 측 암호화를 사용하도록 S3 버킷을 구성합니다. S3 버킷 간의 복제를 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q538
회사는 단일 Amazon EC2 온디맨드 인스턴스에서 웹 사이트 분석 애플리케이션을 호스팅합니다. 분석 소프트웨어는 PHP로 작성되었으며 MySQL 데이터베이스를 사용합니다. 분석 소프 트웨어, PHP를 제공하는 웹 서버 및 데이터베이스 서버는 모두 EC2 인스턴스에서 호스팅됩니다. 애플리케이션이 사용량이 많은 시간 동안 성능 저하의 징후를 보이고 있으며 5xx 오류를 표 시하고 있습니다. 회사는 애플리케이션을 원활하게 확장해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 데이터베이스를 Amazon RDS for MySQL DB 인스턴스로 마이그레이션합니다. 웹 애플리케이션의 AMI를 생성합니다. AMI를 사용하여 두 번째 EC2 온디맨드 인스턴스를 시작합
니다. Application Load Balancer를 사용하여 각 EC2 인스턴스에 로드를 분산합니다.
B. 데이터베이스를 Amazon RDS for MySQL DB 인스턴스로 마이그레이션합니다. 웹 애플리케이션의 AMI를 생성합니다. AMI를 사용하여 두 번째 EC2 온디맨드 인스턴스를 시작합
니다. Amazon Route 53 가중 라우팅을 사용하여 2개의 EC2 인스턴스에 로드를 분산합니다.
C. 데이터베이스를 Amazon Aurora MySQL DB 인스턴스로 마이그레이션합니다. EC2 인스턴스를 중지하고 인스턴스 유형을 변경하는 AWS Lambda 함수를 생성합니다. CPU 사용
률이 75%를 초과하면 Lambda 함수를 호출하는 Amazon CloudWatch 경보를 생성합니다.
D. 데이터베이스를 Amazon Aurora MySQL DB 인스턴스로 마이그레이션합니다. 웹 애플리케이션의 AMI를 생성합니다. 시작 템플릿에 AMI를 적용합니다. 시작 템플릿으로 Auto
Scaling 그룹 생성 스팟 플릿을 사용하도록 시작 템플릿을 구성합니다. Application Load Balancer를 Auto Scaling 그룹에 연결합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q539
회사에서 여러 마이크로서비스로 구성된 애플리케이션을 구축하고 있습니다. 이 회사는 컨테이너 기술을 사용하여 AWS에 소프트웨어를 배포하기로 결정했습니다. 회사는 유지 관리 및 확장 을 위한 지속적인 노력을 최소화하는 솔루션이 필요합니다. 회사는 추가 인프라를 관리할 수 없습니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 작업 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. Amazon Elastic Container Service(Amazon ECS) 클러스터를 배포합니다. 
B. 여러 가용 영역에 걸쳐 있는 Amazon EC2 인스턴스에 Kubernetes 제어 평면을 배포합니다. 
C. Amazon EC2 시작 유형으로 Amazon Elastic Container Service(Amazon ECS) 서비스를 배포합니다. 2보다 크거나 같은 원하는 태스크 번호 레벨을 지정하십시오. 
D. Fargate 시작 유형으로 Amazon Elastic Container Service(Amazon ECS) 서비스를 배포합니다. 2보다 크거나 같은 원하는 태스크 번호 레벨을 지정하십시오. 
E. 여러 가용 영역에 걸쳐 있는 Amazon EC2 인스턴스에 Kubernetes 작업자 노드를 배포합니다. 각 마이크로 서비스에 대해 두 개 이상의 복제본을 지정하는 배포를 만듭니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q540
게임 회사는 고가용성 아키텍처를 설계하고 있습니다. 애플리케이션은 수정된 Linux 커널에서 실행되며 UDP 기반 트래픽만 지원합니다. 회사는 최상의 사용자 경험을 제공하기 위해 프런트 엔드 계층이 필요합니다. 해당 계층은 대기 시간이 짧아야 하고 트래픽을 가장 가까운 엣지 로케이션으로 라우팅하고 애플리케이션 엔드포인트에 진입하기 위한 정적 IP 주소를 제공해야 합니 다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 요청을 Application Load Balancer로 전달하도록 Amazon Route 53을 구성합니다. AWS Application Auto Scaling에서 애플리케이션에 AWS Lambda를 사용합니다. 
B. 요청을 Network Load Balancer로 전달하도록 Amazon CloudFront를 구성합니다. AWS Application Auto Scaling 그룹의 애플리케이션에 AWS Lambda를 사용합니다. 
C. 요청을 Network Load Balancer로 전달하도록 AWS Global Accelerator를 구성합니다. EC2 Auto Scaling 그룹의 애플리케이션에 Amazon EC2 인스턴스를 사용합니다. 
D. 요청을 Application Load Balancer로 전달하도록 Amazon API Gateway를 구성합니다. EC2 Auto Scaling 그룹의 애플리케이션에 Amazon EC2 인스턴스를 사용합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q541
회사에서 Amazon RDS DB 인스턴스에 데이터를 저장할 계획입니다. 회사는 미사용 데이터를 암호화해야 합니다. 솔루션 설계자는 이 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. AWS Key Management Service(AWS KMS)에서 키를 생성합니다. DB 인스턴스에 대한 암호화를 활성화합니다. 
B. 암호화 키를 생성합니다. AWS Secrets Manager에 키를 저장합니다. 키를 사용하여 DB 인스턴스를 암호화합니다. 
C. AWS Certificate Manager(ACM)에서 인증서를 생성합니다. 인증서를 사용하여 DB 인스턴스에서 SSL/TLS를 활성화합니다. 
D. AWS Identity and Access Management(IAM)에서 인증서를 생성합니다. 인증서를 사용하여 DB 인스턴스에서 SSL/TLS를 활성화합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q542
한 회사에서 Java Spring Boot 애플리케이션을 프라이빗 서브넷의 Amazon Elastic Kubernetes Service(Amazon EKS)에서 실행되는 포드로 배포했습니다. 애플리케이션은 Amazon DynamoDB 테이블에 데이터를 써야 합니다. 솔루션 설계자는 애플리케이션이 인터넷에 트래픽을 노출하지 않고 DynamoDB 테이블과 상호 작용할 수 있는지 확인해야 합니다. 이 목표를 달성하기 위해 솔루션 설계자는 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. EKS 포드에 충분한 권한이 있는 IAM 역할을 연결합니다.
B. EKS 포드에 충분한 권한이 있는 IAM 사용자를 연결합니다.
C. 프라이빗 서브넷의 네트워크 ACL을 통해 DynamoDB 테이블에 대한 아웃바운드 연결을 허용합니다.
D. DynamoDB용 VPC 엔드포인트를 생성합니다.
E. Java Spring Boot 코드에 액세스 키를 삽입합니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q543
회사의 애플리케이션에 성능 문제가 있습니다. 애플리케이션은 상태 저장이며 Amazon EC2 인스턴스에서 인 메모리 작업을 완료해야 합니다. 이 회사는 AWS CloudFormation을 사용 하여 인프라를 배포하고 M5 EC2 인스턴스 제품군을 사용했습니다. 트래픽이 증가함에 따라 애플리케이션 성능이 저하되었습니다. 사용자는 사용자가 애플리케이션에 액세스하려고 할 때 지 연을 보고합니다. 운영상 가장 효율적인 방식으로 이러한 문제를 해결하는 솔루션은 무엇입니까?
A. Auto Scaling 그룹에서 실행되는 T3 EC2 인스턴스로 EC2 인스턴스를 교체합니다. AWS Management Console을 사용하여 변경합니다. 
B. Auto Scaling 그룹에서 EC2 인스턴스를 실행하도록 CloudFormation 템플릿을 수정합니다. 증가가 필요한 경우 Auto Scaling 그룹의 원하는 용량과 최대 용량을 수동으로 늘립니
다.
C. CloudFormation 템플릿을 수정합니다. EC2 인스턴스를 R5 EC2 인스턴스로 교체합니다. Amazon CloudWatch 내장 EC2 메모리 메트릭을 사용하여 향후 용량 계획을 위해 애
플리케이션 성능을 추적합니다.
D. CloudFormation 템플릿을 수정합니다. EC2 인스턴스를 R5 EC2 인스턴스로 교체합니다. EC2 인스턴스에 Amazon CloudWatch 에이전트를 배포하여 향후 용량 계획을 위한 사
용자 지정 애플리케이션 지연 시간 메트릭을 생성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q544
회사는 AWS에서 확장 가능한 웹 애플리케이션을 호스팅하려고 합니다. 응용 프로그램은 전 세계 여러 지역의 사용자가 액세스할 수 있습니다. 애플리케이션 사용자는 최대 기가바이트 크기의 고유한 데이터를 다운로드하고 업로드할 수 있습니다. 개발 팀은 업로드 및 다운로드 대기 시간을 최소화하고 성능을 최대화할 수 있는 비용 효율적인 솔루션을 원합니다. 이를 달성하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. Transfer Acceleration과 함께 Amazon S3를 사용하여 애플리케이션을 호스팅합니다. 
B. CacheControl 헤더와 함께 Amazon S3를 사용하여 애플리케이션을 호스팅합니다. 
C. Auto Scaling 및 Amazon CloudFront와 함께 Amazon EC2를 사용하여 애플리케이션을 호스팅합니다. 
D. Auto Scaling 및 Amazon ElastiCache와 함께 Amazon EC2를 사용하여 애플리케이션을 호스팅합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q545
한 회사가 여러 대륙에 걸쳐 도시의 온도, 습도 및 기압에 대한 데이터를 수집합니다. 회사가 매일 각 사이트에서 수집하는 평균 데이터 양은 500GB입니다. 각 사이트에는 고속 인터넷 연결이 있습니다. 회사는 이러한 모든 글로벌 사이트의 데이터를 단일 Amazon S3 버킷에 가능한 한 빨리 집계하려고 합니다. 솔루션은 운영 복잡성을 최소화해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 대상 S3 버킷에서 S3 Transfer Acceleration을 켭니다. 멀티파트 업로드를 사용하여 사이트 데이터를 대상 S3 버킷에 직접 업로드합니다. 
B. 각 사이트의 데이터를 가장 가까운 리전의 S3 버킷에 업로드합니다. S3 교차 리전 복제를 사용하여 객체를 대상 S3 버킷에 복사합니다. 그런 다음 원본 S3 버킷에서 데이터를 제거합니
다.
C. AWS Snowball Edge Storage Optimized 장치 작업을 매일 예약하여 각 사이트에서 가장 가까운 리전으로 데이터를 전송합니다. S3 교차 리전 복제를 사용하여 객체를 대상 S3
버킷에 복사합니다.
D. 각 사이트에서 가장 가까운 리전의 Amazon EC2 인스턴스로 데이터를 업로드합니다. Amazon Elastic Block Store(Amazon EBS) 볼륨에 데이터를 저장합니다. 정기적으로
EBS 스냅샷을 생성하여 대상 S3 버킷이 포함된 리전에 복사합니다. 해당 리전에서 EBS 볼륨을 복원합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q546
회사는 웹 사이트에서 Amazon CloudFront를 사용하고 있습니다. 회사는 CloudFront 배포에서 로깅을 활성화했으며 로그는 회사의 Amazon S3 버킷 중 하나에 저장됩니다. 회사는 로 그에 대한 고급 분석을 수행하고 시각화를 구축해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Amazon Athena에서 표준 SQL 쿼리를 사용하여 S3 버킷의 CloudFront 로그를 분석합니다. AWS Glue로 결과를 시각화합니다. 
B. Amazon Athena에서 표준 SQL 쿼리를 사용하여 S3 버킷의 CloudFront 로그를 분석합니다. Amazon QuickSight로 결과를 시각화합니다. 
C. Amazon DynamoDB에서 표준 SQL 쿼리를 사용하여 S3 버킷의 CloudFront 로그를 분석합니다. AWS Glue로 결과를 시각화합니다. 
D. Amazon DynamoDB에서 표준 SQL 쿼리를 사용하여 S3 버킷의 CloudFront 로그를 분석합니다. Amazon QuickSight로 결과를 시각화합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q547
회사는 Amazon EC2 인스턴스 플릿에서 프로덕션 애플리케이션을 실행합니다. 애플리케이션은 Amazon SQS 대기열에서 데이터를 읽고 병렬로 메시지를 처리합니다. 메시지 볼륨은 예 측할 수 없으며 종종 트래픽이 간헐적으로 발생합니다. 이 애플리케이션은 다운타임 없이 지속적으로 메시지를 처리해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 스팟 인스턴스를 독점적으로 사용하여 필요한 최대 용량을 처리하십시오. 
B. 예약 인스턴스를 독점적으로 사용하여 필요한 최대 용량을 처리합니다. 
C. 기본 용량으로 예약 인스턴스를 사용하고 추가 용량을 처리하려면 스팟 인스턴스를 사용합니다. 
D. 기본 용량에는 예약 인스턴스를 사용하고 추가 용량을 처리하려면 온디맨드 인스턴스를 사용합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q548
회사는 웨어러블 장치를 사용하는 많은 참가자로부터 데이터를 수집합니다. 회사는 데이터를 Amazon DynamoDB 테이블에 저장하고 애플리케이션을 사용하여 데이터를 분석합니다. 데이 터 워크로드는 일정하고 예측 가능합니다. 회사는 DynamoDB에 대한 예상 예산 이하를 유지하려고 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 프로비저닝 모드와 DynamoDB Standard-Infrequent Access(DynamoDB Standard-IA)를 사용합니다. 예상 워크로드에 대한 용량을 예약합니다. 
B. 프로비저닝 모드를 사용합니다. RCU(읽기 용량 단위) 및 WCU(쓰기 용량 단위)를 지정합니다. 
C. 주문형 모드를 사용합니다. 읽기 용량 단위(RCU) 및 쓰기 용량 단위(WCU)를 워크로드의 변경 사항을 수용할 수 있을 만큼 높게 설정합니다. 
D. 주문형 모드를 사용합니다. 예약 용량이 있는 RCU(읽기 용량 단위) 및 WCU(쓰기 용량 단위)를 지정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q549
회사에는 다음 구성 요소를 포함하는 데이터 수집 워크플로가 있습니다. 새로운 데이터 전송에 대한 알림을 수신하는 Amazon Simple Notification Service(Amazon SNS) 주제 데이터를 처리하고 저장하는 AWS Lambda 함수 네트워크 연결 문제로 인해 수집 워크플로가 때때로 실패함 . 장애가 발생하면 회사에서 수동으로 작업을 다시 실행하지 않는 한 해당 데이터가 수집되지 않습니다. 모든 알림이 최종적으로 처리되도록 하려면 솔루션 설계자가 무엇을 해야 합니까?
A. 여러 가용 영역에 걸쳐 배포할 Lambda 함수를 구성합니다. 
B. Lambda 함수의 구성을 수정하여 함수에 대한 CPU 및 메모리 할당을 늘립니다. 
C. 재시도 횟수와 재시도 사이의 대기 시간을 모두 늘리도록 SNS 주제의 재시도 전략을 구성합니다. 
D. Amazon Simple Queue Service(Amazon SQS) 대기열을 장애 시 대상으로 구성합니다. 대기열의 메시지를 처리하도록 Lambda 함수를 수정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q550
솔루션 설계자는 스토리지 비용을 최적화해야 합니다. 솔루션 설계자는 더 이상 액세스하지 않거나 거의 액세스하지 않는 Amazon S3 버킷을 식별해야 합니다. 최소한의 운영 오버헤드로 이 목표를 달성할 수 있는 솔루션은 무엇입니까?
A. 고급 활동 메트릭에 대한 S3 Storage Lens 대시보드를 사용하여 버킷 액세스 패턴을 분석합니다. 
B. AWS Management Console에서 S3 대시보드를 사용하여 버킷 액세스 패턴을 분석합니다. 
C. 버킷에 대한 Amazon CloudWatch BucketSizeBytes 지표를 켭니다. Amazon Athena에서 메트릭 데이터를 사용하여 버킷 액세스 패턴을 분석합니다. 
D. S3 객체 모니터링을 위해 AWS CloudTrail을 켭니다. Amazon CloudWatch Logs와 통합된 CloudTrail 로그를 사용하여 버킷 액세스 패턴을 분석합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q551
회사는 ap-southeast-3 리전의 Amazon Aurora PostgreSQL 데이터베이스에 기밀 데이터를 저장합니다. 데이터베이스는 AWS Key Management Service(AWS KMS) 고객 관 리형 키로 암호화됩니다. 이 회사는 최근에 인수되었으며 ap-southeast-3에서 인수 회사의 AWS 계정과 데이터베이스 백업을 안전하게 공유해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 데이터베이스 스냅샷을 생성합니다. 스냅샷을 암호화되지 않은 새 스냅샷에 복사합니다. 인수 회사의 AWS 계정과 새 스냅샷을 공유합니다. 
B. 데이터베이스 스냅샷을 생성합니다. 인수 회사의 AWS 계정을 KMS 키 정책에 추가합니다. 인수 회사의 AWS 계정과 스냅샷을 공유합니다. 
C. 다른 AWS 관리형 KMS 키를 사용하는 데이터베이스 스냅샷을 생성합니다. 인수 회사의 AWS 계정을 KMS 키 별칭에 추가합니다. 인수 회사의 AWS 계정과 스냅샷을 공유합니다. 
D. 데이터베이스 스냅샷을 생성합니다. 데이터베이스 스냅샷을 다운로드합니다. Amazon S3 버킷에 데이터베이스 스냅샷을 업로드합니다. 인수 회사의 AWS 계정에서 액세스를 허용하도
록 S3 버킷 정책을 업데이트합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q552
회사는 AWS 클라우드 배포를 검토하여 Amazon S3 버킷에 무단 구성 변경이 없는지 확인해야 합니다. 이 목표를 달성하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. 적절한 규칙으로 AWS Config를 켭니다. 
B. 적절한 확인을 통해 AWS Trusted Advisor를 켭니다. 
C. 적절한 평가 템플릿으로 Amazon Inspector를 켭니다. 
D. Amazon S3 서버 액세스 로깅을 켭니다. Amazon EventBridge(Amazon Cloud Watch Events)를 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q553
회사는 웹 사이트에서 항목의 검색 가능한 저장소를 유지 관리합니다. 데이터는 1,000만 개 이상의 행을 포함하는 Amazon RDS for MySQL 데이터베이스 테이블에 저장됩니다. 데이터베 이스에는 2TB의 범용 SSD 스토리지가 있습니다. 회사 웹 사이트를 통해 매일 이 데이터에 대한 수백만 건의 업데이트가 있습니다. 회사는 일부 삽입 작업이 10초 이상 걸리는 것을 발견했습니다. 회사는 데이터베이스 스토리지 성능이 문제라고 판단했습니다. 이 성능 문제를 해결하는 솔루션은 무엇입니까?
A. 스토리지 유형을 프로비저닝된 IOPS SSD로 변경합니다. 
B. DB 인스턴스를 메모리 최적화 인스턴스 클래스로 변경합니다. 
C. DB 인스턴스를 버스트 가능한 성능 인스턴스 클래스로 변경합니다. 
D. MySQL 기본 비동기 복제로 다중 AZ RDS 읽기 복제본을 활성화합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q554
개발자에게는 AWS Lambda 함수를 사용하여 파일을 Amazon S3에 업로드하는 애플리케이션이 있으며 작업을 수행하는 데 필요한 권한이 필요합니다. 개발자에게는 이미 Amazon S3 에 필요한 유효한 IAM 자격 증명이 있는 IAM 사용자가 있습니다. 권한을 부여하려면 솔루션 설계자가 무엇을 해야 합니까?
A. Lambda 함수의 리소스 정책에 필요한 IAM 권한을 추가합니다. 
B. Lambda 함수에서 기존 IAM 자격 증명을 사용하여 서명된 요청을 생성합니다. 
C. 새 IAM 사용자를 생성하고 Lambda 함수에서 기존 IAM 자격 증명을 사용합니다. 
D. 필요한 권한이 있는 IAM 실행 역할을 생성하고 IAM 역할을 Lambda 함수에 연결합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q555
회사에는 중요한 데이터가 포함된 Amazon S3 버킷이 있습니다. 회사는 우발적인 삭제로부터 데이터를 보호해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. S3 버킷에서 버전 관리를 활성화합니다. 
B. S3 버킷에서 MFA 삭제를 활성화합니다. 
C. S3 버킷에 버킷 정책을 생성합니다. 
D. S3 버킷에서 기본 암호화를 활성화합니다. 
E. S3 버킷의 객체에 대한 수명 주기 정책을 생성합니다.

<details>
<summary>정답 보기</summary>

**AB**
</details>

---

### Q556
회사에서 UDP 연결을 사용하는 VoIP(Voice over Internet Protocol) 서비스를 제공합니다. 이 서비스는 Auto Scaling 그룹에서 실행되는 Amazon EC2 인스턴스로 구성됩니다. 이 회사는 여러 AWS 지역에 배포했습니다. 회사는 지연 시간이 가장 짧은 리전으로 사용자를 라우팅해야 합니다. 회사는 또한 리전 간에 자동화된 장애 조치가 필요합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. NLB(Network Load Balancer) 및 연결된 대상 그룹을 배포합니다. 대상 그룹을 Auto Scaling 그룹과 연결합니다. 각 리전에서 NLB를 AWS Global Accelerator 엔드포인트로
사용합니다.
B. ALB(Application Load Balancer) 및 연결된 대상 그룹을 배포합니다. 대상 그룹을 Auto Scaling 그룹과 연결합니다. 각 리전에서 ALB를 AWS Global Accelerator 엔드포인트
로 사용합니다.
C. NLB(Network Load Balancer) 및 연결된 대상 그룹을 배포합니다. 대상 그룹을 Auto Scaling 그룹과 연결합니다. 각 NLB의 별칭을 가리키는 Amazon Route 53 지연 시간 레
코드를 생성합니다. 지연 시간 레코드를 오리진으로 사용하는 Amazon CloudFront 배포를 생성합니다.
D. ALB(Application Load Balancer) 및 연결된 대상 그룹을 배포합니다. 대상 그룹을 Auto Scaling 그룹과 연결합니다. 각 ALB의 별칭을 가리키는 Amazon Route 53 가중치 레
코드를 생성합니다. 가중 레코드를 오리진으로 사용하는 Amazon CloudFront 배포를 배포합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q557
회사에는 온프레미스 Windows Server에서 실행되는 Microsoft .NET 애플리케이션이 있습니다. 애플리케이션은 Oracle Database Standard Edition 서버를 사용하여 데이터를 저 장합니다. 이 회사는 AWS로의 마이그레이션을 계획하고 있으며 애플리케이션을 이동하는 동안 개발 변경을 최소화하려고 합니다. AWS 애플리케이션 환경은 가용성이 높아야 합니다. 이러한 요구 사항을 충족하기 위해 회사는 어떤 조합의 조치를 취해야 합니까? (두 가지를 선택하세요.)
A. .NET Core를 실행하는 AWS Lambda 함수를 사용하여 애플리케이션을 서버리스로 리팩터링합니다. 
B. 다중 AZ 배포에서 .NET 플랫폼을 사용하여 AWS Elastic Beanstalk에서 애플리케이션을 다시 호스팅합니다. 
C. Amazon Linux Amazon 머신 이미지(AMI)를 사용하여 Amazon EC2에서 실행되도록 애플리케이션 플랫폼을 변경합니다. 
D. 다중 AZ 배포에서 AWS DMS(AWS Database Migration Service)를 사용하여 Oracle 데이터베이스에서 Amazon DynamoDB로 마이그레이션합니다. 
E. 다중 AZ 배포에서 AWS Database Migration Service(AWS DMS)를 사용하여 Oracle 데이터베이스에서 Amazon RDS의 Oracle로 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q558
회사는 Amazon RDS DB 인스턴스에서 실행되는 모든 데이터베이스에 대해 새로운 데이터 보존 정책을 구현하고 있습니다. 회사는 최소 2년 동안 일일 백업을 유지해야 합니다. 백업은 일 관되고 복원 가능해야 합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 어떤 솔루션을 권장해야 합니까?
A. RDS 백업을 유지하기 위해 AWS Backup에서 백업 볼트를 생성합니다. 일일 일정과 생성 후 2년의 만료 기간으로 새 백업 계획을 생성합니다. 백업 계획에 RDS DB 인스턴스를 할당
합니다.
B. 일일 스냅샷을 위해 RDS DB 인스턴스의 백업 기간을 구성합니다. 각 RDS DB 인스턴스에 2년의 스냅샷 보존 정책을 할당합니다. Amazon DLM(Amazon Data Lifecycle
Manager)을 사용하여 스냅샷 삭제를 예약합니다.
C. 만료 기간이 2년인 Amazon CloudWatch Logs에 자동으로 백업되도록 데이터베이스 트랜잭션 로그를 구성합니다. 
D. AWS Database Migration Service(AWS DMS) 복제 작업을 구성합니다. 복제 인스턴스를 배포하고 변경 데이터 캡처(CDC) 작업을 구성하여 데이터베이스 변경 사항을 대상으로
Amazon S3에 스트리(cid:1535)합니다. 2년 후 스냅샷을 삭제하도록 S3 수명 주기 정책을 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q559
애플리케이션 개발 팀은 큰 이미지를 더 작은 압축 이미지로 변환하는 마이크로서비스를 설계하고 있습니다. 사용자가 웹 인터페이스를 통해 이미지를 업로드할 때 마이크로 서비스는 이미지를 Amazon S3 버킷에 저장하고 AWS Lambda 함수로 이미지를 처리 및 압축하고 이미지를 압축된 형태로 다른 S3 버킷에 저장해야 합니다. 솔루션 설계자는 이미지를 자동으로 처리하기 위해 내구성 있고 상태 비저장 구성 요소를 사용하는 솔루션을 설계해야 합니다. 이러한 요구 사항을 충족하는 작업 조합은 무엇입니까? (두 가지를 선택하세요.)
A. Amazon Simple Queue Service(Amazon SQS) 대기열을 생성합니다. 이미지가 S3 버킷에 업로드될 때 SQS 대기열에 알림을 보내도록 S3 버킷을 구성합니다. 
B. Amazon Simple Queue Service(Amazon SQS) 대기열을 호출 소스로 사용하도록 Lambda 함수를 구성합니다. SQS 메시지가 성공적으로 처리되면 대기열에서 메시지를 삭제
합니다.
C. 새 업로드에 대해 S3 버킷을 모니터링하도록 Lambda 함수를 구성합니다. 업로드된 이미지가 감지되면 파일 이름을 메모리의 텍스트 파일에 쓰고 텍스트 파일을 사용하여 처리된 이미지
를 추적합니다.
D. Amazon EC2 인스턴스를 시작하여 Amazon Simple Queue Service(Amazon SQS) 대기열을 모니터링합니다. 대기열에 항목이 추가되면 EC2 인스턴스의 텍스트 파일에 파일
이름을 기록하고 Lambda 함수를 호출합니다.
E. S3 버킷을 모니터링하도록 Amazon EventBridge(Amazon CloudWatch Events) 이벤트를 구성합니다. 이미지가 업로드되면 추가 처리를 위해 애플리케이션 소유자의 이메일 주
소와 함께 Amazon ampl Notification Service(Amazon SNS) 주제로 알림을 보냅니다.

<details>
<summary>정답 보기</summary>

**AB**
</details>

---

### Q560
한 회사에서 us-east-1 리전의 Microsoft SQL Server 단일 AZ DB 인스턴스용 100GB Amazon RDS를 사용하여 고객 트랜잭션을 저장합니다. 회사는 DB 인스턴스에 대한 고가용 성 및 자동 복구가 필요합니다. 또한 회사는 1년에 여러 번 RDS 데이터베이스에 대한 보고서를 실행해야 합니다. 보고 프로세스로 인해 트랜잭션이 고객 계정에 게시되는 데 평소보다 오래 걸립니다. 회사는 보고 프로세스 의 성능을 향상시킬 솔루션이 필요합니다. 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 단일 AZ DB 인스턴스에서 다중 AZ 배포로 DB 인스턴스를 수정합니다. 
B. 현재 DB 인스턴스의 스냅샷을 찍습니다. 다른 가용 영역의 새 RDS 배포로 스냅샷을 복원합니다. 
C. 다른 가용 영역에서 DB 인스턴스의 읽기 전용 복제본을 생성합니다. 보고서에 대한 모든 요청은 읽기 전용 복제본을 가리킵니다. 
D. 데이터베이스를 RDS Custom으로 마이그레이션합니다. 
E. RDS Proxy를 사용하여 보고 요청을 유지 관리 기간으로 제한합니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q561
Amazon EC2 인스턴스에서 호스팅되는 애플리케이션은 Amazon S3 버킷에 액세스해야 합니다. 트래픽이 인터넷을 통과하면 안 됩니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 액세스를 어떻게 구성해야 합니까?
A. Amazon Route 53을 사용하여 프라이빗 호스팅 영역을 생성합니다. 
B. VPC에서 Amazon S3에 대한 게이트웨이 VPC 엔드포인트를 설정합니다. 
C. NAT 게이트웨이를 사용하여 S3 버킷에 액세스하도록 EC2 인스턴스를 구성합니다. 
D. VPC와 S3 버킷 간에 AWS Site-to-Site VPN 연결을 설정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q562
회사에는 Amazon EC2 인스턴스에서 실행되는 레거시 데이터 처리 애플리케이션이 있습니다. 데이터는 순차적으로 처리되지만 결과의 순서는 중요하지 않습니다. 응용 프로그램은 모놀리 식 아키텍처를 사용합니다. 회사에서 수요 증가에 맞춰 애플리케이션을 확장할 수 있는 유일한 방법은 인스턴스 크기를 늘리는 것입니다. 이 회사의 개발자는 Amazon Elastic Container Service(Amazon ECS)에서 마이크로서비스 아키텍처를 사용하도록 애플리케이션을 다시 작성하기로 결정했습니다. 솔루션 설계자는 마이크로서비스 간의 통신을 위해 무엇을 권장해야 합니까?
A. Amazon Simple Queue Service(Amazon SQS) 대기열을 생성합니다. 데이터 생산자에 코드를 추가하고 데이터를 대기열로 보냅니다. 데이터 소비자에 코드를 추가하여 대기열의
데이터를 처리합니다.
B. Amazon Simple Notification Service(Amazon SNS) 주제를 생성합니다. 데이터 생산자에 코드를 추가하고 주제에 알림을 게시합니다. 데이터 소비자에 코드를 추가하여 주제를
구독합니다.
C. 메시지를 전달할 AWS Lambda 함수를 생성합니다. 데이터 생산자에 코드를 추가하여 데이터 객체로 Lambda 함수를 호출합니다. 데이터 소비자에 코드를 추가하여 Lambda 함수에
서 전달되는 데이터 객체를 수신합니다.
D. Amazon DynamoDB 테이블을 생성합니다. DynamoDB 스트림을 활성화합니다. 데이터 생산자에 코드를 추가하여 테이블에 데이터를 삽입합니다. 데이터 소비자에 코드를 추가하여
DynamoDB Streams API를 사용하여 새 테이블 항목을 감지하고 데이터를 검색합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q563
회사에서 애플리케이션을 AWS로 마이그레이션하고 있습니다. 응용 프로그램은 다른 계정에 배포됩니다. 회사는 AWS Organizations를 사용하여 중앙에서 계정을 관리합니다. 회사의 보 안 팀은 회사의 모든 계정에 대한 SSO(Single Sign-On) 솔루션이 필요합니다. 회사는 온프레미스 자체 관리 Microsoft Active Directory에서 사용자와 그룹을 계속 관리해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS SSO 콘솔에서 AWS Single Sign-On(AWS SSO)을 활성화합니다. 단방향 포리스트 트러스트 또는 단방향 도메인 트러스트를 생성하여 Microsoft Active Directory용
AWS Directory Service를 사용하여 회사의 자체 관리형 Microsoft Active Directory를 AWS SSO와 연결합니다.
B. AWS SSO 콘솔에서 AWS Single Sign-On(AWS SSO)을 활성화합니다. Microsoft Active Directory용 AWS Directory Service를 사용하여 회사의 자체 관리형
Microsoft Active Directory를 AWS SSO와 연결하는 양방향 포리스트 트러스트를 생성합니다.
C. AWS 디렉터리 서비스를 사용합니다. 회사의 자체 관리 Microsoft Active Directory와 양방향 신뢰 관계를 만듭니다. 
D. 온프레미스에 ID 공급자(IdP)를 배포합니다. AWS SSO 콘솔에서 AWS Single Sign-On(AWS SSO)을 활성화합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q564
회사는 온프레미스에서 Oracle 데이터베이스를 실행합니다. 회사는 AWS로 마이그레이션하는 과정에서 데이터베이스를 사용 가능한 최신 버전으로 업그레이드하려고 합니다. 또한 회사는 데이터베이스에 재해 복구(DR)를 설정하려고 합니다. 회사는 정상 운영 및 DR 설정을 위한 운영 오버헤드를 최소화해야 합니다. 회사는 또한 데이터베이스의 기본 운영 체제에 대한 액세스를 유지 관리해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Oracle 데이터베이스를 Amazon EC2 인스턴스로 마이그레이션합니다. 다른 AWS 리전으로 데이터베이스 복제를 설정합니다. 
B. Oracle 데이터베이스를 Oracle용 Amazon RDS로 마이그레이션합니다. 리전 간 자동 백업을 활성화하여 스냅샷을 다른 AWS 리전에 복제합니다. 
C. Oracle 데이터베이스를 Amazon RDS Custom for Oracle로 마이그레이션합니다. 다른 AWS 리전에서 데이터베이스에 대한 읽기 전용 복제본을 생성합니다. 
D. Oracle 데이터베이스를 Oracle용 Amazon RDS로 마이그레이션합니다. 다른 가용 영역에서 대기 데이터베이스를 생성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q565
한 미디어 회사가 시스템을 AWS 클라우드로 이전할 가능성을 평가하고 있습니다. 회사는 비디오 처리를 위해 가능한 최대 I/O 성능을 갖춘 최소 10TB의 스토리지, 미디어 콘텐츠를 저장하 기 위한 300TB의 내구성이 뛰어난 스토리지, 더 이상 사용하지 않는 아카이브 미디어에 대한 요구 사항을 충족하기 위해 900TB의 스토리지가 필요합니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자가 추천해야 하는 서비스 세트는 무엇입니까?
A. 최대 성능을 위한 Amazon EBS, 내구성 있는 데이터 스토리지를 위한 Amazon S3, 아카이브 스토리지를 위한 Amazon S3 Glacier 
B. 최대 성능을 위한 Amazon EBS, 내구성 있는 데이터 스토리지를 위한 Amazon EFS, 아카이브 스토리지를 위한 Amazon S3 Glacier 
C. 최대 성능을 위한 Amazon EC2 인스턴스 스토어, 내구성 있는 데이터 스토리지를 위한 Amazon EFS, 아카이브 스토리지를 위한 Amazon S3 
D. 최대 성능을 위한 Amazon EC2 인스턴스 스토어, 내구성 있는 데이터 스토리지를 위한 Amazon S3, 아카이브 스토리지를 위한 Amazon S3 Glacier

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q566
솔루션 설계자는 Amazon S3 버킷에 업로드된 모든 객체가 암호화되도록 하려면 어떻게 해야 합니까?
A. PutObject에 s3:x-amz-acl 헤더 세트가 없는 경우 거부하도록 버킷 정책을 업데이트합니다. 
B. PutObject에 프라이빗으로 설정된 s3:x-amz-acl 헤더가 없는 경우 거부하도록 버킷 정책을 업데이트합니다. 
C. PutObject에 true로 설정된 aws:SecureTransport 헤더가 없는 경우 거부하도록 버킷 정책을 업데이트합니다. 
D. PutObject에 x-amz-server-side-encryption 헤더 세트가 없는 경우 거부하도록 버킷 정책을 업데이트합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q567
회사는 Amazon CloudWatch Logs 로그 그룹에 애플리케이션 로그를 저장합니다. 새로운 정책에 따라 회사는 거의 실시간으로 Amazon OpenSearch Service(Amazon Elasticsearch Service)에 모든 애플리케이션 로그를 저장해야 합니다. 최소한의 운영 오버헤드로 이 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 로그를 Amazon OpenSearch Service(Amazon Elasticsearch Service)로 스트리(cid:1535)하도록 CloudWatch Logs 구독을 구성합니다. 
B. AWS Lambda 함수를 생성합니다. 로그 그룹을 사용하여 함수를 호출하여 Amazon OpenSearch Service(Amazon Elasticsearch Service)에 로그를 기록합니다. 
C. Amazon Kinesis Data Firehose 전송 스트림을 생성합니다. 전송 스트림 소스로 로그 그룹을 구성합니다. Amazon OpenSearch Service(Amazon Elasticsearch Service)
를 전송 스트림의 대상으로 구성합니다.
D. 각 애플리케이션 서버에 Amazon Kinesis Agent를 설치하고 구성하여 Amazon Kinesis Data Streams에 로그를 전달합니다. Amazon OpenSearch Service(Amazon
Elasticsearch Service)에 로그를 전달하도록 Kinesis Data Streams를 구성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q568
Amazon EC2 인스턴스는 새 VPC의 프라이빗 서브넷에 있습니다. 이 서브넷에는 아웃바운드 인터넷 액세스 권한이 없지만 EC2 인스턴스에는 외부 공급업체로부터 월별 보안 업데이트를 다운로드할 수 있는 기능이 필요합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 인터넷 게이트웨이를 생성하고 VPC에 연결합니다. 인터넷 게이트웨이를 기본 경로로 사용하도록 프라이빗 서브넷 경로 테이블을 구성합니다. 
B. NAT 게이트웨이를 생성하고 퍼블릭 서브넷에 배치합니다. NAT 게이트웨이를 기본 경로로 사용하도록 프라이빗 서브넷 경로 테이블을 구성합니다. 
C. NAT 인스턴스를 생성하고 EC2 인스턴스가 있는 동일한 서브넷에 배치합니다. NAT 인스턴스를 기본 경로로 사용하도록 프라이빗 서브넷 경로 테이블을 구성합니다. 
D. 인터넷 게이트웨이를 생성하고 VPC에 연결합니다. NAT 인스턴스를 생성하고 EC2 인스턴스가 있는 동일한 서브넷에 배치합니다. 인터넷 게이트웨이를 기본 경로로 사용하도록 프라이
빗 서브넷 경로 테이블을 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q569
한 회사에서 사용자가 사진을 업로드하고 이미지에 사진 프레임을 추가할 수 있는 이미지 분석 애플리케이션을 만들었습니다. 사용자는 이미지에 추가할 사진 프레임을 나타내기 위해 이미지와 메타데이터를 업로드합니다. 애플리케이션은 단일 Amazon EC2 인스턴스와 Amazon DynamoDB를 사용하여 메타데이터를 저장합니다. 응용 프로그램이 점점 대중화되고 사용자 수가 증가하고 있습니다. 회사는 시간대와 요일에 따라 동시접속자 수가 크게 달라질 것으로 예상하고 있다. 회사는 애플리케이션이 증가하는 사용자 기반의 요구 사항을 충족하도록 확장할 수 있는지 확인해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Lambda를 사용하여 사진을 처리하십시오. 사진과 메타데이터를 DynamoDB에 저장합니다. 
B. Amazon Kinesis Data Firehose를 사용하여 사진을 처리하고 사진과 메타데이터를 저장합니다. 
C. AWS Lambda를 사용하여 사진을 처리합니다. 사진을 Amazon S3에 저장합니다. 메타데이터를 저장하기 위해 DynamoDB를 보관합니다. 
D. EC2 인스턴스 수를 3개로 늘립니다. 프로비저닝된 IOPS SSD(io2) Amazon Elastic Block Store(Amazon EBS) 볼륨을 사용하여 사진과 메타데이터를 저장합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q570
한 온라인 소매 회사는 5천만 명 이상의 활성 고객을 보유하고 있으며 매일 25,000건 이상의 주문을 받습니다. 회사는 고객의 구매 데이터를 수집하고 이 데이터를 Amazon S3에 저장합니 다. 추가 고객 데이터는 Amazon RDS에 저장됩니다. 회사는 팀이 분석을 수행할 수 있도록 다양한 팀에서 모든 데이터를 사용할 수 있도록 하려고 합니다. 솔루션은 데이터에 대한 세분화된 권한을 관리하는 기능을 제공하고 운영 오버헤드를 최소 화해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 구매 데이터를 마이그레이션하여 Amazon RDS에 직접 씁니다. RDS 액세스 제어를 사용하여 액세스를 제한하십시오. 
B. Amazon RDS에서 Amazon S3로 데이터를 주기적으로 복사하도록 AWS Lambda 함수를 예약합니다. AWS Glue 크롤러를 생성합니다. Amazon Athena를 사용하여 데이터를
쿼리합니다. S3 정책을 사용하여 액세스를 제한하십시오.
C. AWS Lake Formation을 사용하여 데이터 레이크를 생성합니다. Amazon RDS에 대한 AWS Glue JDBC 연결을 생성합니다. Lake Formation에 S3 버킷을 등록합니다.
Lake Formation 액세스 제어를 사용하여 액세스를 제한하십시오.
D. Amazon Redshift 클러스터를 생성합니다. Amazon S3 및 Amazon RDS에서 Amazon Redshift로 데이터를 주기적으로 복사하도록 AWS Lambda 함수를 예약합니다.
Amazon Redshift 액세스 제어를 사용하여 액세스를 제한하십시오.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q571
회사에서 갑자기 수요가 증가하고 있습니다. 회사는 Amazon 머신 이미지(AMI)에서 대규모 Amazon EC2 인스턴스를 프로비저닝해야 합니다. 인스턴스는 Auto Scaling 그룹에서 실행 됩니다. 회사는 요구 사항을 충족하기 위해 최소 초기화 대기 시간을 제공하는 솔루션이 필요합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. aws ec2 register-image 명령을 사용하여 스냅샷에서 AMI를 생성합니다. AWS Step Functions를 사용하여 Auto Scaling 그룹의 AMI를 교체하십시오. 
B. 스냅샷에서 Amazon Elastic Block Store(Amazon EBS) 빠른 스냅샷 복원을 활성화합니다. 스냅샷을 사용하여 AMI를 프로비저닝합니다. Auto Scaling 그룹의 AMI를 새 AMI
로 교체합니다.
C. Amazon Data Lifecycle Manager(Amazon DLM)에서 AMI 생성을 활성화하고 수명 주기 규칙을 정의합니다. Auto Scaling 그룹에서 AMI를 수정하는 AWS Lambda 함수를
생성합니다.
D. Amazon EventBridge를 사용하여 AMI를 프로비저닝하는 AWS Backup 수명 주기 정책을 호출합니다. EventBridge에서 Auto Scaling 그룹 용량 제한을 이벤트 소스로 구성합
니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q572
솔루션 설계자는 웹 사이트를 위한 고가용성 인프라를 설계해야 합니다. 이 웹 사이트는 Amazon EC2 인스턴스에서 실행되는 Windows 웹 서버로 구동됩니다. 솔루션 설계자는 수천 개의 IP 주소에서 발생하는 대규모 DDoS 공격을 완화할 수 있는 솔루션을 구현해야 합니다. 다운타임은 웹사이트에 허용되지 않습니다. 그러한 공격으로부터 웹 사이트를 보호하기 위해 솔루션 설계자는 어떤 조치를 취해야 합니까? (두 가지를 선택하세요.)
A. AWS Shield Advanced를 사용하여 DDoS 공격을 중지하십시오. 
B. 공격자를 자동으로 차단하도록 Amazon GuardDuty를 구성합니다. 
C. 정적 및 동적 콘텐츠 모두에 대해 Amazon CloudFront를 사용하도록 웹 사이트를 구성합니다. 
D. AWS Lambda 함수를 사용하여 공격자 IP 주소를 VPC 네트워크 ACL에 자동으로 추가합니다. 
E. CPU 사용률이 80%로 설정된 대상 추적 조정 정책과 함께 Auto Scaling 그룹에서 EC2 스팟 인스턴스를 사용합니다.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q573
한 회사가 최근 전체 IT 환경을 AWS 클라우드로 마이그레이션했습니다. 회사는 사용자가 적절한 변경 제어 프로세스를 사용하지 않고 과도한 크기의 Amazon EC2 인스턴스를 프로비저닝 하고 보안 그룹 규칙을 수정하고 있음을 발견했습니다. 솔루션 설계자는 이러한 인벤토리 및 구성 변경 사항을 추적하고 감사하기 위한 전략을 고안해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 어떤 조치를 취해야 합니까? (두 가지를 선택하세요.)
A. AWS CloudTrail을 활성화하고 감사에 사용하십시오. 
B. Amazon EC2 인스턴스에 대한 데이터 수명 주기 정책을 사용합니다. 
C. AWS Trusted Advisor를 활성화하고 보안 대시보드를 참조합니다. 
D. AWS Config를 활성화하고 감사 및 규정 준수를 위한 규칙을 생성합니다. 
E. AWS CloudFormation 템플릿을 사용하여 이전 리소스 구성을 복원합니다.

<details>
<summary>정답 보기</summary>

**AD**
</details>

---

### Q574
회사는 온프레미스 데이터 센터의 Kubernetes 클러스터에서 컨테이너화된 애플리케이션을 실행합니다. 회사는 데이터 저장을 위해 MongoDB 데이터베이스를 사용하고 있습니다. 회사는 이러한 환경 중 일부를 AWS로 마이그레이션하려고 하지만 현재로서는 코드 변경이나 배포 방법 변경이 불가능합니다. 회사는 운영 오버헤드를 최소화하는 솔루션이 필요합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 컴퓨팅을 위해 Amazon EC2 작업자 노드와 함께 Amazon Elastic Container Service(Amazon ECS)를 사용하고 데이터 저장을 위해 EC2의 MongoDB를 사용합니다. 
B. 컴퓨팅용 AWS Fargate 및 데이터 스토리지용 Amazon DynamoDB와 함께 Amazon Elastic Container Service(Amazon ECS) 사용 
C. Amazon Elastic Kubernetes Service(Amazon EKS)를 Amazon EC2 작업자 노드와 함께 컴퓨팅용으로 사용하고 Amazon DynamoDB를 데이터 저장용으로 사용합니다. 
D. 컴퓨팅용 AWS Fargate 및 데이터 스토리지용 Amazon DocumentDB(MongoDB 호환)와 함께 Amazon Elastic Kubernetes Service(Amazon EKS)를 사용합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q575
회사에서 데이터를 Amazon S3 버킷으로 이동할 계획입니다. 데이터는 S3 버킷에 저장될 때 암호화되어야 합니다. 또한 암호화 키는 매년 자동으로 순환되어야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 데이터를 S3 버킷으로 이동합니다. Amazon S3 관리형 암호화 키(SSE-S3)로 서버 측 암호화를 사용합니다. SSE-S3 암호화 키의 기본 제공 키 회전 동작을 사용합니다. 
B. AWS Key Management Service(AWS KMS) 고객 관리형 키를 생성합니다. 자동 키 순환을 활성화합니다. 고객 관리형 KMS 키를 사용하도록 S3 버킷의 기본 암호화 동작을 설
정합니다. 데이터를 S3 버킷으로 이동합니다.
C. AWS Key Management Service(AWS KMS) 고객 관리형 키를 생성합니다. 고객 관리형 KMS 키를 사용하도록 S3 버킷의 기본 암호화 동작을 설정합니다. 데이터를 S3 버킷으
로 이동합니다. 매년 KMS 키를 수동으로 교체합니다.
D. 데이터를 S3 버킷으로 이동하기 전에 고객 키 자료로 데이터를 암호화합니다. 키 자료 없이 AWS Key Management Service(AWS KMS) 키를 생성합니다. 고객 키 자료를 KMS
키로 가져옵니다. 자동 키 순환을 활성화합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q576
한 회사에서 UDP를 사용하는 수천 개의 지리적으로 분산된 원격 장치로부터 데이터를 수신하는 애플리케이션을 실행합니다. 애플리케이션은 데이터를 즉시 처리하고 필요한 경우 장치로 다 시 메시지를 보냅니다. 데이터가 저장되지 않습니다. 회사는 장치에서 데이터 전송에 대한 대기 시간을 최소화하는 솔루션이 필요합니다. 솔루션은 또한 다른 AWS 리전에 대한 빠른 장애 조치를 제공해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon Route 53 장애 조치 라우팅 정책을 구성합니다. 두 리전 각각에 NLB(Network Load Balancer)를 생성합니다. 데이터를 처리하기 위해 AWS Lambda 함수를 호출하도
록 NLB를 구성합니다.
B. AWS Global Accelerator를 사용합니다. 두 리전 각각에 NLB(Network Load Balancer)를 엔드포인트로 생성합니다. Fargate 시작 유형으로 Amazon Elastic Container
Service(Amazon ECS) 클러스터를 생성합니다. 클러스터에서 ECS 서비스를 생성합니다. Amazon ECS에서 데이터를 NLProcess하기 위한 대상으로 ECS 서비스를 설정합니 다.
C. AWS Global Accelerator를 사용합니다. 두 리전 각각에 Application Load Balancer(ALB)를 엔드포인트로 생성합니다. Fargate 시작 유형으로 Amazon Elastic Container
Service(Amazon ECS) 클러스터를 생성합니다. 클러스터에서 ECS 서비스를 생성합니다. ECS 서비스를 ALB의 대상으로 설정합니다. Amazon ECS에서 데이터를 처리합니다.
D. Amazon Route 53 장애 조치 라우팅 정책을 구성합니다. 두 리전 각각에 Application Load Balancer(ALB)를 생성합니다. Fargate 시작 유형으로 Amazon Elastic
Container Service(Amazon ECS) 클러스터를 생성합니다. 클러스터에서 ECS 서비스를 생성합니다. ECS 서비스를 ALB의 대상으로 설정합니다. Amazon ECS에서 데이터를 처리합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q577
한 회사에서 MySQL용 Amazon RDS에 데이터베이스를 배포했습니다. 트랜잭션 증가로 인해 데이터베이스 지원 팀은 DB 인스턴스에 대한 느린 읽기를 보고하고 있으며 읽기 전용 복제본 을 추가할 것을 권장합니다. 이 변경 사항을 구현하기 전에 솔루션 설계자가 수행해야 하는 작업 조합은 무엇입니까? (두 가지를 선택하세요.)
A. RDS 기본 노드에서 binlog 복제를 활성화합니다. 
B. 원본 DB 인스턴스의 장애 조치 우선 순위를 선택합니다. 
C. 원본 DB 인스턴스에서 장기 실행 트랜잭션이 완료되도록 허용합니다. 
D. 글로벌 테이블을 생성하고 테이블을 사용할 수 있는 AWS 리전을 지정합니다. 
E. 백업 보존 기간을 0 이외의 값으로 설정하여 원본 인스턴스에서 자동 백업을 활성화합니다.

<details>
<summary>정답 보기</summary>

**CE**
</details>

---

### Q578
한 회사에서 Auto Scaling 그룹의 클라이언트와 서버 간의 통신에 UDP를 사용하는 실시간 멀티플레이어 게임을 개발하고 있습니다. 하루 동안 수요가 급증할 것으로 예상되므로 게임 서버 플랫폼은 그에 따라 적응해야 합니다. 개발자는 개입 없이 확장되는 데이터베이스 솔루션에 게이머 점수 및 기타 비관계형 데이터를 저장하기를 원합니다. 솔루션 설계자는 어떤 솔루션을 추천해야 합니까?
A. 트래픽 분산에는 Amazon Route 53을 사용하고 데이터 저장에는 Amazon Aurora Serverless를 사용하십시오. 
B. 트래픽 분산을 위해 Network Load Balancer를 사용하고 데이터 저장을 위해 주문형 Amazon DynamoDB를 사용합니다. 
C. 트래픽 분산을 위해 Network Load Balancer를 사용하고 데이터 저장을 위해 Amazon Aurora Global Database를 사용합니다. 
D. 트래픽 분산을 위해 Application Load Balancer를 사용하고 데이터 저장을 위해 Amazon DynamoDB 전역 테이블을 사용합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q579
전자 상거래 회사에는 Amazon API Gateway 및 AWS Lambda 함수를 사용하는 주문 처리 애플리케이션이 있습니다. 애플리케이션은 Amazon Aurora PostgreSQL 데이터베이스 에 데이터를 저장합니다. 최근 판매 행사 중에 고객 주문이 갑자기 급증했습니다. 일부 고객은 시간 초과를 경험했고 애플리케이션은 해당 고객의 주문을 처리하지 않았습니다. 솔루션 설계자는 많은 수의 열린 연결로 인해 데이터베이스에서 CPU 사용률과 메모리 사용률이 높다고 판단했습니다. 솔루션 설계자는 응용 프로그램을 최소한으로 변경하면서 시간 초과 오 류를 방지해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Lambda 함수에 대해 프로비저닝된 동시성을 구성합니다. 여러 AWS 리전에서 글로벌 데이터베이스가 되도록 데이터베이스를 수정합니다. 
B. Amazon RDS 프록시를 사용하여 데이터베이스에 대한 프록시를 생성합니다. 데이터베이스 엔드포인트 대신 RDS 프록시 엔드포인트를 사용하도록 Lambda 함수를 수정합니다. 
C. 다른 AWS 리전에서 데이터베이스에 대한 읽기 전용 복제본을 생성합니다. API Gateway에서 쿼리 문자열 파라미터를 사용하여 트래픽을 읽기 전용 복제본으로 라우팅합니다. 
D. AWS Database Migration Service(AWS DMS)를 사용하여 Aurora PostgreSQL에서 Amazon DynamoDB로 데이터를 마이그레이션합니다. DynamoDB 테이블을 사용
하도록 Lambda 함수를 수정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q580
회사에 통합 결제를 사용하는 여러 AWS 계정이 있습니다. 이 회사는 90일 동안 여러 개의 활성 고성능 Amazon RDS for Oracle 온디맨드 DB 인스턴스를 실행합니다. 회사의 재무 팀은 통합 결제 계정 및 기타 모든 AWS 계정에서 AWS Trusted Advisor에 액세스할 수 있습니다. 재무 팀은 적절한 AWS 계정을 사용하여 RDS에 대한 Trusted Advisor 확인 권장 사항에 액세스해야 합니다. 재무팀은 적절한 Trusted Advisor 수표를 검토하여 RDS 비용을 줄여야 합 니다. 이러한 요구 사항을 충족하기 위해 재무 팀은 어떤 조합의 단계를 수행해야 합니까? (두 가지를 선택하세요.)
A. RDS 인스턴스가 실행 중인 계정의 Trusted Advisor 권장 사항을 사용합니다. 
B. 통합 결제 계정의 Trusted Advisor 권장 사항을 사용하여 모든 RDS 인스턴스 확인을 동시에 확인합니다. 
C. Amazon RDS 예약 인스턴스 최적화에 대한 Trusted Advisor 검사를 검토합니다. 
D. Amazon RDS 유휴 DB 인스턴스에 대한 Trusted Advisor 검사를 검토합니다. 
E. Amazon Redshift 예약 노드 최적화에 대한 Trusted Advisor 검사를 검토합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q581
의학 연구실에서 새로운 연구와 관련된 데이터를 생성합니다. 연구소는 온프레미스 파일 기반 애플리케이션을 위해 전국의 클리닉에 최소한의 대기 시간으로 데이터를 제공하고자 합니다. 데이 터 파일은 각 클리닉에 대한 읽기 전용 권한이 있는 Amazon S3 버킷에 저장됩니다. 이러한 요구 사항을 충족하기 위해 솔루션 설계자는 무엇을 권장해야 합니까?
A. 각 클리닉에서 온프레미스로 AWS Storage Gateway 파일 게이트웨이를 가상 머신(VM)으로 배포합니다. 
B. 처리를 위해 AWS DataSync를 사용하여 각 클리닉의 온프레미스 애플리케이션으로 파일을 마이그레이션합니다. 
C. 각 클리닉에서 온프레미스로 AWS Storage Gateway 볼륨 게이트웨이를 가상 머신(VM)으로 배포합니다. 
D. Amazon Elastic File System(Amazon EFS) 파일 시스템을 각 클리닉의 온프레미스 서버에 연결합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q582
회사에서 Amazon 머신 이미지(AMI)를 관리하려고 합니다. 회사는 현재 AMI가 생성된 동일한 AWS 리전에 AMI를 복사합니다. 회사는 AWS API 호출을 캡처하고 회사 계정 내에서 Amazon EC2 CreateImage API 작업이 호출될 때마다 알림을 보내는 애플리케이션을 설계해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS CloudTrail 로그를 쿼리하고 CreateImage API 호출이 감지되면 알림을 보내는 AWS Lambda 함수를 생성합니다. 
B. 업데이트된 로그가 Amazon S3로 전송될 때 발생하는 Amazon Simple Notification Service(Amazon SNS) 알림으로 AWS CloudTrail을 구성합니다. Amazon Athena를
사용하여 새 테이블을 생성하고 API 호출이 감지되면 CreateImage에서 쿼리합니다.
C. CreateImage API 호출에 대한 Amazon EventBridge(Amazon CloudWatch Events) 규칙을 생성합니다. CreateImage API 호출이 감지되면 알림을 보내도록 대상을
Amazon Simple Notification Service(Amazon SNS) 주제로 구성합니다.
D. Amazon Simple Queue Service(Amazon SQS) FIFO 대기열을 AWS CloudTrail 로그의 대상으로 구성합니다. CreateImage API 호출이 감지되면 Amazon Simple
Notification Service(Amazon SNS) 주제에 알림을 보내는 AWS Lambda 함수를 생성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q583
솔루션 설계자는 회사가 AWS에서 애플리케이션을 실행하는 비용을 최적화하도록 도와야 합니다. 애플리케이션은 아키텍처 내 컴퓨팅을 위해 Amazon EC2 인스턴스, AWS Fargate 및 AWS Lambda를 사용합니다. EC2 인스턴스는 애플리케이션의 데이터 수집 계층을 실행합니다. EC2 사용은 산발적이고 예측할 수 없습니다. EC2 인스턴스에서 실행되는 워크로드는 언제든지 중단될 수 있습니다. 애플 리케이션 프런트 엔드는 Fargate에서 실행되고 Lambda는 API 계층을 제공합니다. 프런트 엔드 사용률 및 API 레이어 사용률은 내년 동안 예측할 수 있습니다. 이 애플리케이션을 호스팅하는 데 가장 비용 효율적인 솔루션을 제공하는 구매 옵션 조합은 무엇입니까? (두 가지를 선택하세요.)
A. 데이터 수집 계층에 스팟 인스턴스를 사용합니다.
B. 데이터 수집 계층에 온디맨드 인스턴스 사용
C. 프런트엔드 및 API 계층에 대한 1년 Compute Savings Plan을 구매하세요.
D. 데이터 수집 계층을 위해 1년 전체 선결제 예약 인스턴스를 구매합니다.
E. 프런트엔드 및 API 계층에 대한 1년 EC2 인스턴스 Savings Plan을 구매하세요.

<details>
<summary>정답 보기</summary>

**AC**
</details>

---

### Q584
한 회사에서 Amazon S3 버킷을 스토리지로 사용할 파일 공유 애플리케이션을 개발하고 있습니다. 회사는 Amazon CloudFront 배포를 통해 모든 파일을 제공하려고 합니다. 회사는 S3 URL에 대한 직접 탐색을 통해 파일에 액세스할 수 있기를 원하지 않습니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. 각 S3 버킷에 대한 개별 정책을 작성하여 CloudFront 액세스에 대해서만 읽기 권한을 부여하십시오. 
B. IAM 사용자를 생성합니다. 사용자에게 S3 버킷의 객체에 대한 읽기 권한을 부여합니다. 사용자를 CloudFront에 할당합니다. 
C. CloudFront 배포 ID를 Principal로 할당하고 대상 S3 버킷을 Amazon 리소스 이름(ARN)으로 할당하는 S3 버킷 정책을 작성합니다. 
D. 원본 액세스 ID(OAI)를 만듭니다. CloudFront 배포에 OAI를 할당합니다. OAI만 읽기 권한을 갖도록 S3 버킷 권한을 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q585
회사에서 CompanyConfidential Amazon S3 버킷에 대한 액세스 권한이 없어야 하는 새로운 클라우드 엔지니어를 채용했습니다. 클라우드 엔지니어는 AdminTools라는 S3 버킷에 대 한 읽기 및 쓰기 권한이 있어야 합니다. 이러한 기준을 충족하는 IAM 정책은 무엇입니까?
A.
B.
C.
D.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q586
회사에서 응용 프로그램의 데이터를 암호화해야 하는 개발자를 지원하기 위해 확장 가능한 키 관리 인프라를 구축하려고 합니다. 솔루션 아키텍트는 운영 부담을 줄이기 위해 무엇을 해야 합니까?
A. 다단계 인증(MFA)을 사용하여 암호화 키를 보호하십시오. 
B. AWS Key Management Service(AWS KMS)를 사용하여 암호화 키를 보호합니다. 
C. AWS Certificate Manager(ACM)를 사용하여 암호화 키를 생성, 저장 및 할당합니다. 
D. IAM 정책을 사용하여 암호화 키를 보호할 수 있는 액세스 권한이 있는 사용자의 범위를 제한합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q587
회사에는 매시간 수백 개의 .csv 파일을 Amazon S3 버킷에 배치하는 애플리케이션이 있습니다. 파일 크기는 1GB입니다. 파일이 업로드될 때마다 회사는 파일을 Apache Parquet 형식 으로 변환하고 출력 파일을 S3 버킷에 배치해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. .csv 파일을 다운로드하고 파일을 Parquet 형식으로 변환하고 출력 파일을 S3 버킷에 배치하는 AWS Lambda 함수를 생성합니다. 각 S3 PUT 이벤트에 대해 Lambda 함수를 호출
합니다.
B. Apache Spark 작업을 생성하여 .csv 파일을 읽고, 파일을 Parquet 형식으로 변환하고, 출력 파일을 S3 버킷에 배치합니다. Spark 작업을 호출하기 위해 각 S3 PUT 이벤트에 대한
AWS Lambda 함수를 생성합니다.
C. 애플리케이션이 .csv 파일을 배치하는 S3 버킷에 대한 AWS Glue 테이블과 AWS Glue 크롤러를 생성합니다. Amazon Athena를 주기적으로 사용하여 AWS Glue 테이블을 쿼리
하고, 쿼리 결과를 Parquet 형식으로 변환하고, 출력 파일을 S3 버킷에 배치하도록 AWS Lambda 함수를 예약합니다.
D. AWS Glue 추출, 변환 및 로드(ETL) 작업을 생성하여 .csv 파일을 Parquet 형식으로 변환하고 출력 파일을 S3 버킷에 배치합니다. 각 S3 PUT 이벤트에 대한 AWS Lambda 함
수를 생성하여 ETL 작업을 호출합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q588
회사는 새 문서가 Amazon S3 버킷에 업로드될 때 AWS Lambda 함수를 호출하는 서버리스 애플리케이션을 배포했습니다. 애플리케이션은 Lambda 함수를 사용하여 문서를 처리합니다 . 최근 마케팅 캠페인 후 회사는 애플리케이션이 많은 문서를 처리하지 않는다는 사실을 알게 되었습니다. 솔루션 설계자는 이 애플리케이션의 아키텍처를 개선하기 위해 무엇을 해야 합니까?
A. Lambda 함수의 런타임 제한 시간 값을 15분으로 설정합니다. 
B. S3 버킷 복제 정책을 구성합니다. 나중에 처리할 수 있도록 S3 버킷에 문서를 준비합니다. 
C. 추가 Lambda 함수를 배포합니다. 두 Lambda 함수에서 문서 처리 부하를 분산합니다. 
D. Amazon Simple Queue Service(Amazon SQS) 대기열을 생성합니다. 대기열에 요청을 보냅니다. 대기열을 Lambda에 대한 이벤트 소스로 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q589
회사는 회사의 기본 웹 사이트를 사용할 수 없는 경우 사용자를 백업 정적 오류 페이지로 안내하려고 합니다. 기본 웹 사이트의 DNS 레코드는 Amazon Route 53에서 호스팅됩니다. 도메인 은 Application Load Balancer(ALB)를 가리킵니다. 회사는 변경 및 인프라 오버헤드를 최소화하는 솔루션이 필요합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 지연 시간 라우팅 정책을 사용하도록 Route 53 레코드를 업데이트합니다. 트래픽이 가장 반응이 빠른 엔드포인트로 전송되도록 Amazon S3 버킷에서 호스팅되는 정적 오류 페이지를
레코드에 추가합니다.
B. Route 53 활성-수동 장애 조치 구성을 설정합니다. Route 53 상태 확인에서 ALB 엔드포인트가 비정상이라고 판단하면 Amazon S3 버킷에서 호스팅되는 정적 오류 페이지로 트래픽
을 보냅니다.
C. 정적 오류 페이지를 엔드포인트로 호스팅하는 Amazon EC2 인스턴스와 ALB를 사용하여 Route 53 활성-활성 구성을 설정합니다. ALB에 대한 상태 확인이 실패한 경우에만 인스턴
스에 요청을 보내도록 Route 53을 구성합니다.
D. 다중값 응답 라우팅 정책을 사용하도록 Route 53 레코드를 업데이트합니다. 상태 확인을 만듭니다. 상태 확인이 통과되면 트래픽을 웹사이트로 안내합니다. 상태 확인을 통과하지 못한
경우 Amazon S3에서 호스팅되는 정적 오류 페이지로 트래픽을 보냅니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q590
회사의 웹 애플리케이션이 Application Load Balancer 뒤의 Amazon EC2 인스턴스에서 실행 중입니다. 이 회사는 최근 정책을 변경하여 이제 특정 국가에서만 애플리케이션에 액세스 하도록 요구합니다. 이 요구 사항을 충족하는 구성은 무엇입니까?
A. EC2 인스턴스에 대한 보안 그룹을 구성합니다. 
B. Application Load Balancer에서 보안 그룹을 구성합니다. 
C. VPC의 Application Load Balancer에서 AWS WAF를 구성합니다. 
D. EC2 인스턴스를 포함하는 서브넷에 대한 네트워크 ACL을 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q591
회사는 Amazon Elastic Kubernetes Service(Amazon EKS)를 사용하여 컨테이너 애플리케이션을 실행합니다. 회사의 작업량은 하루 종일 일정하지 않습니다. 회사는 Amazon EKS가 워크로드에 따라 확장 및 축소되기를 원합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (2개 선택)
A. AWS Lambda 함수를 사용하여 EKS 클러스터의 크기를 조정합니다.
B. Kubernetes Metrics Server를 사용하여 수평적 포드 자동 확장을 활성화합니다.
C. Kubernetes Cluster Autoscaler를 사용하여 클러스터의 노드 수를 관리합니다.
D. Amazon API Gateway를 사용하여 Amazon EKS에 연결합니다.
E. AWS App Mesh를 사용하여 네트워크 활동을 관찰합니다.

<details>
<summary>정답 보기</summary>

**BC**
</details>

---

### Q592
회사에는 드물게 액세스하는 패턴으로 글로벌 영업 팀에서 사용하는 온프레미스 MySQL 데이터베이스가 있습니다. 영업팀은 데이터베이스의 가동 중지 시간을 최소화해야 합니다. 데이터베 이스 관리자는 향후 더 많은 사용자를 예상하여 특정 인스턴스 유형을 선택하지 않고 이 데이터베이스를 AWS로 마이그레이션하려고 합니다. 솔루션 설계자는 어떤 서비스를 추천해야 합니까?
A. 아마존 오로라 MySQL 
B. MySQL용 Amazon Aurora 서버리스 
C. 아마존 레드시프트 스펙트럼 
D. MySQL용 Amazon RDS

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q593
회사는 Amazon API Gateway를 사용하여 동일한 VPC에서 두 개의 REST API로 프라이빗 게이트웨이를 실행합니다. BuyStock RESTful 웹 서비스는 CheckFunds RESTful 웹 서비스를 호출하여 주식을 구매하기 전에 충분한 자금을 사용할 수 있는지 확인합니다. 회사는 VPC 흐름 로그에서 BuyStock RESTful 웹 서비스가 VPC 대신 인터넷을 통해 CheckFunds RESTful 웹 서비스를 호출한다는 사실을 확인했습니다. 솔루션 설계자는 API가 VPC를 통해 통신하도록 솔루션을 구현해야 합니다. 코드를 가장 적게 변경하여 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 인증을 위해 HTTP 헤더에 X-API-Key 헤더를 추가합니다. 
B. 인터페이스 엔드포인트를 사용합니다. 
C. 게이트웨이 엔드포인트를 사용합니다. 
D. 두 REST API 사이에 Amazon Simple Queue Service(Amazon SQS) 대기열을 추가합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q594
회사에서 엔지니어 팀을 위해 개별 AWS 계정을 실험하려고 합니다. 회사는 지정된 달의 Amazon EC2 인스턴스 사용량이 각 계정의 특정 임계값을 초과하는 즉시 알림을 받기를 원합니다. 이 요구 사항을 가장 비용 효율적으로 충족하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. Cost Explorer를 사용하여 서비스별 비용에 대한 일일 보고서를 생성합니다. EC2 인스턴스별로 보고서를 필터링합니다. 임계값을 초과하면 Amazon Simple Email Service
(Amazon SES) 알림을 보내도록 Cost Explorer를 구성합니다.
B. Cost Explorer를 사용하여 서비스별 월별 비용 보고서를 생성합니다. EC2 인스턴스별로 보고서를 필터링합니다. 임계값을 초과하면 Amazon Simple Email Service(Amazon
SES) 알림을 보내도록 Cost Explorer를 구성합니다.
C. AWS 예산을 사용하여 각 계정에 대한 비용 예산을 생성합니다. 기간을 매월로 설정합니다. 범위를 EC2 인스턴스로 설정합니다. 예산에 대한 경고 임계값을 설정합니다. 임계값 초과 시
알림을 받도록 Amazon Simple Notification Service(Amazon SNS) 주제를 구성합니다.
D. AWS 비용 및 사용 보고서를 사용하여 시간 단위로 보고서를 생성합니다. 보고서 데이터를 Amazon Athena와 통합합니다. Amazon EventBridge를 사용하여 Athena 쿼리를 예약
합니다. 임계값 초과 시 알림을 받도록 Amazon Simple Notification Service(Amazon SNS) 주제를 구성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q595
예산 계획의 일환으로 경영진은 사용자별로 나열된 AWS 청구 항목에 대한 보고서를 원합니다. 데이터는 부서 예산을 만드는 데 사용됩니다. 솔루션 설계자는 이 보고서 정보를 얻는 가장 효율 적인 방법을 결정해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon Athena로 쿼리를 실행하여 보고서를 생성합니다. 
B. Cost Explorer에서 보고서를 생성하고 보고서를 다운로드합니다. 
C. 청구 대시보드에서 청구서 세부 정보에 액세스하고 청구서를 다운로드합니다. 
D. Amazon Simple Email Service(Amazon SES)로 알리도록 AWS 예산에서 비용 예산을 수정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q596
회사에는 Amazon Route 53에서 전달하는 트래픽이 있는 10개 이상의 Amazon EC2 인스턴스를 호스팅하는 웹 애플리케이션이 있습니다. 회사에서 애플리케이션을 검색하려고 할 때 때 때로 시간 초과 오류가 발생합니다. 네트워킹 팀은 일부 DNS 쿼리가 비정상 인스턴스의 IP 주소를 반환하여 시간 초과 오류가 발생했음을 발견했습니다. 이러한 시간 초과 오류를 극복하기 위해 솔루션 설계자는 무엇을 구현해야 합니까?
A. 각 EC2 인스턴스에 대해 Route 53 단순 라우팅 정책 레코드를 생성합니다. 상태 확인을 각 레코드와 연결합니다. 
B. 각 EC2 인스턴스에 대해 Route 53 장애 조치 라우팅 정책 레코드를 생성합니다. 상태 확인을 각 레코드와 연결합니다. 
C. EC2 인스턴스를 원본으로 사용하여 Amazon CloudFront 배포를 생성합니다. 상태 확인을 EC2 인스턴스와 연결합니다. 
D. EC2 인스턴스 앞에서 상태 확인을 통해 Application Load Balancer(ALB)를 생성합니다. 루트 53에서 ALB로 이동합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q597
회사는 모든 기능이 활성화된 AWS Organizations를 사용하고 ap-southeast-2 리전에서 여러 Amazon EC2 워크로드를 실행합니다. 회사에는 다른 리전에서 리소스가 생성되지 않도 록 하는 SCP(서비스 제어 정책)가 있습니다. 보안 정책에 따라 회사는 유휴 상태의 모든 데이터를 암호화해야 합니다. 감사 결과 직원이 볼륨을 암호화하지 않고 EC2 인스턴스용 Amazon Elastic Block Store(Amazon EBS) 볼륨을 생성한 것으로 확인되었습니다. 회사는 암호화된 EBS 볼륨을 사용하 기 위해 모든 IAM 사용자 또는 루트 사용자가 ap-southeast-2에서 시작하는 모든 새 EC2 인스턴스를 원합니다. 회사는 EBS 볼륨을 생성하는 직원에게 최소한의 영향을 미치는 솔루션을 원합니다. 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (두 가지를 선택하세요.)
A. Amazon EC2 콘솔에서 EBS 암호화 계정 속성을 선택하고 기본 암호화 키를 정의합니다. 
B. IAM 권한 경계를 생성합니다. 권한 경계를 루트 조직 단위(OU)에 연결합니다. ec2:Encrypted 조건이 false인 경우 ec2:CreateVolume 작업을 거부하도록 경계를 정의합니다. 
C. SCP를 생성합니다. 루트 조직 단위(OU)에 SCP를 연결합니다. ec2:Encrypted 조건이 false일 때 ec2:CreateVolume 작업을 거부하도록 SCP를 정의합니다. 
D. ec2:Encrypted 조건이 false인 경우 ec2:CreateVolume 작업을 거부하도록 각 계정에 대한 IAM 정책을 업데이트합니다. 
E. 조직 관리 계정에서 기본 EBS 볼륨 암호화 설정을 지정합니다.

<details>
<summary>정답 보기</summary>

**CE**
</details>

---

### Q598
회사는 비디오 콘텐츠를 게시하고 모든 모바일 플랫폼에서 사용할 수 있도록 트랜스코딩하는 온라인 서비스를 제공합니다. 애플리케이션 아키텍처는 Amazon Elastic File System (Amazon EFS) Standard를 사용하여 여러 Amazon EC2 Linux 인스턴스가 처리를 위해 비디오 콘텐츠에 액세스할 수 있도록 비디오를 수집하고 저장합니다. 시간이 지남에 따라 서비 스의 인기가 높아짐에 따라 스토리지 비용이 너무 비싸졌습니다. 가장 비용 효율적인 스토리지 솔루션은 무엇입니까?
A. 파일용 AWS Storage Gateway를 사용하여 동영상 콘텐츠를 저장하고 처리합니다. 
B. 볼륨에 AWS Storage Gateway를 사용하여 비디오 콘텐츠를 저장하고 처리합니다. 
C. Amazon EFS를 사용하여 비디오 콘텐츠를 저장합니다. 처리가 완료되면 파일을 Amazon Elastic Block Store(Amazon EBS)로 전송합니다. 
D. 동영상 콘텐츠 저장을 위해 Amazon S3를 사용합니다. 처리를 위해 파일을 서버에 연결된 Amazon Elastic Block Store(Amazon EBS) 볼륨으로 임시로 이동합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q599
회사는 의료 실험의 결과를 Amazon S3 리포지토리에 저장해야 합니다. 리포지토리는 소수의 과학자가 새 파일을 추가할 수 있도록 허용하고 다른 모든 사용자는 읽기 전용 액세스로 제한해 야 합니다. 어떤 사용자도 리포지토리의 파일을 수정하거나 삭제할 수 없습니다. 회사는 모든 파일을 생성일로부터 최소 1년 동안 저장소에 보관해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 법적 보존 기간이 1년인 거버넌스 모드에서 S3 객체 잠금을 사용합니다. 
B. 보존 기간이 365일인 규정 준수 모드에서 S3 객체 잠금을 사용합니다. 
C. IAM 역할을 사용하여 모든 사용자가 S3 버킷의 객체를 삭제하거나 변경하지 못하도록 제한합니다. S3 버킷 정책을 사용하여 IAM 역할만 허용하십시오. 
D. 객체가 추가될 때마다 AWS Lambda 함수를 호출하도록 S3 버킷을 구성합니다. 수정된 개체가 적절하게 표시될 수 있도록 저장된 개체의 해시를 추적하도록 기능을 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q600
솔루션 아키텍트가 다가올 음악 행사를 위해 웹사이트를 최적화하고 있습니다. 공연 영상은 실시간으로 스트리(cid:1535)되며 주문형으로 제공된다. 이 행사는 전 세계 온라인 청중을 끌어들일 것으로 예상됩니다. 실시간 및 온디맨드 스트리(cid:1535)의 성능을 모두 향상시키는 서비스는 무엇입니까?
A. 아마존 클라우드프론트 
B. AWS 글로벌 액셀러레이터 
C. 아마존 루트 53 
D. Amazon S3 Transfer Acceleration

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q601
회사는 AWS에서 애플리케이션을 호스팅합니다. 이 회사는 Amazon Cognito를 사용하여 사용자를 관리합니다. 사용자가 애플리케이션에 로그인하면 애플리케이션은 Amazon API Gateway에서 호스팅되는 REST API를 사용하여 Amazon DynamoDB에서 필요한 데이터를 가져옵니다. 이 회사는 개발 노력을 줄이기 위해 REST API에 대한 액세스를 제어하는 AWS 관리형 솔루션을 원합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 어떤 사용자가 요청했는지 확인하기 위해 API Gateway에서 권한 부여자가 되도록 AWS Lambda 함수를 구성합니다. 
B. 각 사용자에 대해 각 요청과 함께 전송되어야 하는 API 키를 생성하고 할당합니다. AWS Lambda 함수를 사용하여 키를 검증합니다. 
C. 모든 요청과 함께 헤더에 사용자의 이메일 주소를 보냅니다. 해당 이메일 주소를 가진 사용자에게 적절한 액세스 권한이 있는지 확인하려면 AWS Lambda 함수를 호출하십시오. 
D. Amazon Cognito가 각 요청을 검증할 수 있도록 API Gateway에서 Amazon Cognito 사용자 풀 권한 부여자를 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q602
회사에는 ALB(Application Load Balancer) 뒤의 단일 가용 영역에 있는 Amazon EC2 Auto Scaling 그룹에서 6개의 프런트 엔드 웹 서버를 실행하는 다중 계층 애플리케이션이 있습 니다. 솔루션 설계자는 애플리케이션을 수정하지 않고 인프라를 고가용성으로 수정해야 합니다. 고가용성을 제공하는 솔루션 설계자는 어떤 아키텍처를 선택해야 합니까?
A. 두 리전 각각에서 세 개의 인스턴스를 사용하는 Auto Scaling 그룹을 만듭니다. 
B. 2개의 가용 영역 각각에서 3개의 인스턴스를 사용하도록 Auto Scaling 그룹을 수정합니다. 
C. 다른 리전에서 더 많은 인스턴스를 빠르게 생성하는 데 사용할 수 있는 Auto Scaling 템플릿을 생성합니다. 
D. 라운드 로빈 구성에서 Amazon EC2 인스턴스 앞의 ALB를 변경하여 웹 계층에 대한 트래픽의 균형을 맞춥니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q603
금융 회사의 고객은 문자 메시지를 보내 재정 고문과의 약속을 요청합니다. Amazon EC2 인스턴스에서 실행되는 웹 애플리케이션은 약속 요청을 수락합니다. 텍스트 메시지는 웹 애플리케이 션을 통해 Amazon Simple Queue Service(Amazon SQS) 대기열에 게시됩니다. EC2 인스턴스에서 실행되는 또 다른 애플리케이션은 회의 초대장과 회의 확인 이메일 메시지를 고객 에게 보냅니다. 예약에 성공한 후 이 애플리케이션은 회의 정보를 Amazon DynamoDB 데이터베이스에 저장합니다. 회사가 확장됨에 따라 고객은 회의 초대장이 도착하는 데 시간이 더 오래 걸린다고 보고합니다. 솔루션 설계자는 이 문제를 해결하기 위해 무엇을 권장해야 합니까?
A. DynamoDB 데이터베이스 앞에 DynamoDB Accelerator(DAX) 클러스터를 추가합니다. 
B. 약속 요청을 수락하는 웹 애플리케이션 앞에 Amazon API Gateway API를 추가합니다. 
C. Amazon CloudFront 배포를 추가합니다. 오리진을 약속 요청을 수락하는 웹 애플리케이션으로 설정합니다. 
D. 회의 초대를 보내는 애플리케이션에 대한 Auto Scaling 그룹을 추가합니다. SQS 대기열의 깊이에 따라 확장되도록 Auto Scaling 그룹을 구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q604
회사는 온프레미스 데이터 센터의 여러 애플리케이션에 영향을 미치는 위반을 경험했습니다. 공격자는 서버에서 실행 중인 맞춤형 애플리케이션의 취약점을 이용했습니다. 이 회사는 현재 Amazon EC2 인스턴스에서 실행되도록 애플리케이션을 마이그레이션하고 있습니다. 이 회사는 EC2 인스턴스의 취약성을 능동적으로 스캔하고 결과를 자세히 설명하는 보고서를 보내는 솔루션을 구현하려고 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Shield를 배포하여 EC2 인스턴스의 취약점을 스캔합니다. 결과를 AWS CloudTrail에 기록하는 AWS Lambda 함수를 생성합니다. 
B. Amazon Macie 및 AWS Lambda 함수를 배포하여 EC2 인스턴스의 취약점을 스캔합니다. 결과를 AWS CloudTrail에 기록합니다. 
C. Amazon GuardDuty를 켭니다. GuardDuty 에이전트를 EC2 인스턴스에 배포합니다. 결과를 자세히 설명하는 보고서의 생성 및 배포를 자동화하도록 AWS Lambda 함수를 구성
합니다.
D. Amazon Inspector를 켭니다. Amazon Inspector 에이전트를 EC2 인스턴스에 배포합니다. 결과를 자세히 설명하는 보고서의 생성 및 배포를 자동화하도록 AWS Lambda 함수를
구성합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q605
회사는 AWS 리전에 워크로드가 있습니다. 고객은 Amazon API Gateway REST API를 사용하여 워크로드에 연결하고 액세스합니다. 이 회사는 Amazon Route 53을 DNS 공급자로 사용합니다. 회사는 모든 고객에게 개별적이고 안전한 URL을 제공하고자 합니다. 가장 높은 운영 효율성으로 이러한 요구 사항을 충족하는 단계 조합은 무엇입니까? (3개를 선택하세요.)
A. 등록기관에 필요한 도메인을 등록합니다. Route 53 호스팅 영역에서 와일드카드 사용자 지정 도메인 이름을 생성하고 API 게이트웨이 엔드포인트를 가리키는 영역에 기록합니다. 
B. 다른 리전에 있는 AWS Certificate Manager(ACM)의 도메인과 일치하는 와일드카드 인증서를 요청합니다. 
C. Route 53에서 필요에 따라 각 고객에 대한 호스팅 영역을 생성합니다. API 게이트웨이 엔드포인트를 가리키는 영역 레코드를 생성합니다. 
D. 동일한 리전의 AWS Certificate Manager(ACM)에서 사용자 지정 도메인 이름과 일치하는 와일드카드 인증서를 요청합니다. 
E. API Gateway에서 각 고객에 대해 여러 API 끝점을 만듭니다. 
F. API Gateway에서 REST API용 사용자 정의 도메인 이름을 생성합니다. AWS Certificate Manager(ACM)에서 인증서를 가져옵니다.

<details>
<summary>정답 보기</summary>

**ADF**
</details>

---

### Q606
회사는 AWS에 사용자 디바이스에서 센서 데이터를 수집하는 3계층 환경을 가지고 있습니다. 트래픽은 NLB(Network Load Balancer)를 거쳐 웹 계층용 Amazon EC2 인스턴스로 이동하고 마지막으로 데이터베이스 호출을 수행하는 애플리케이션 계층용 EC2 인스턴스로 이동합니다. 솔루션 설계자는 웹 계층으로 전송되는 데이터의 보안을 개선하기 위해 무엇을 해야 합니까?
A. TLS 수신기를 구성하고 NLB에 서버 인증서를 추가합니다.
B. AWS Shield Advanced를 구성하고 NLB에서 AWS WAF를 활성화합니다.
C. 로드 밸런서를 Application Load Balancer로 변경하고 여기에 AWS WAF를 연결합니다.
D. AWS Key Management Service(AWS KMS)를 사용하여 EC2 인스턴스에서 Amazon Elastic Block Store(Amazon EBS) 볼륨을 암호화합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q607
회사의 보안 팀이 VPC 흐름 로그에서 네트워크 트래픽을 캡처하도록 요청합니다. 로그는 90일 동안 자주 액세스한 후 간헐적으로 액세스합니다. 솔루션 설계자는 로그를 구성할 때 이러한 요구 사항을 충족하기 위해 무엇을 해야 합니까?
A. Amazon CloudWatch를 대상으로 사용하십시오. 90일 만료로 CloudWatch 로그 그룹 설정 
B. Amazon Kinesis를 대상으로 사용합니다. 항상 90일 동안 로그를 유지하도록 Kinesis 스트림을 구성합니다. 
C. AWS CloudTrail을 대상으로 사용합니다. Amazon S3 버킷에 저장하도록 CloudTrail을 구성하고 S3 Intelligent-Tiering을 활성화합니다. 
D. Amazon S3를 대상으로 사용합니다. S3 수명 주기 정책을 활성화하여 90일 후에 로그를 S3 Standard-Infrequent Access(S3 Standard-IA)로 전환합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q608
한 회사에 여러 Amazon EC2 인스턴스에서 실행되는 애플리케이션이 있습니다. 각 EC2 인스턴스에는 여러 Amazon Elastic Block Store(Amazon EBS) 데이터 볼륨이 연결되어 있 습니다. 애플리케이션의 EC2 인스턴스 구성 및 데이터는 야간에 백업해야 합니다. 또한 애플리케이션은 다른 AWS 리전에서 복구 가능해야 합니다. 운영상 가장 효율적인 방식으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 애플리케이션 EBS 볼륨의 야간 스냅샷을 예약하고 스냅샷을 다른 리전에 복사하는 AWS Lambda 함수를 작성합니다. 
B. 야간 백업을 수행하기 위해 AWS Backup을 사용하여 백업 계획을 생성합니다. 백업을 다른 리전에 복사합니다. 애플리케이션의 EC2 인스턴스를 리소스로 추가합니다. 
C. 야간 백업을 수행하기 위해 AWS Backup을 사용하여 백업 계획을 만듭니다. 백업을 다른 리전에 복사합니다. 애플리케이션의 EBS 볼륨을 리소스로 추가합니다. 
D. 애플리케이션 EBS 볼륨의 야간 스냅샷을 예약하고 스냅샷을 다른 가용 영역에 복사하는 AWS Lambda 함수를 작성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q609
회사에는 Amazon RDS의 데이터베이스에 목록을 저장하는 자동차 판매 웹 사이트가 있습니다. 자동차가 판매되면 웹사이트에서 목록을 제거하고 데이터를 여러 대상 시스템으로 전송해야 합니다. 솔루션 설계자는 어떤 디자인을 추천해야 합니까?
A. 대상이 소비할 Amazon Simple Queue Service(Amazon SQS) 대기열로 정보를 전송하도록 Amazon RDS의 데이터베이스가 업데이트될 때 트리거되는 AWS Lambda 함수
를 생성합니다.
B. 대상이 사용할 Amazon Simple Queue Service(Amazon SQS) FIFO 대기열에 정보를 전송하도록 Amazon RDS의 데이터베이스가 업데이트될 때 트리거되는 AWS
Lambda 함수를 생성합니다.
C. RDS 이벤트 알림을 구독하고 여러 Amazon Simple Notification Service(Amazon SNS) 주제로 팬 아웃된 Amazon Simple Queue Service(Amazon SQS) 대기열을 보
냅니다. AWS Lambda 함수를 사용하여 대상을 업데이트합니다.
D. RDS 이벤트 알림을 구독하고 여러 Amazon Simple Queue Service(Amazon SQS) 대기열로 팬 아웃된 Amazon Simple Notification Service(Amazon SNS) 주제를 보
냅니다. AWS Lambda 함수를 사용하여 대상을 업데이트합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q610
회사는 수집된 원시 데이터를 Amazon S3 버킷에 저장합니다. 이 데이터는 회사 고객을 대신하여 여러 유형의 분석에 사용됩니다. 요청된 분석 유형에 따라 S3 객체에 대한 액세스 패턴이 결정됩니다. 회사는 접속 패턴을 예측하거나 통제할 수 없습니다. 회사는 S3 비용을 줄이고자 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. S3 복제를 사용하여 자주 액세스하지 않는 개체를 S3 Standard-Infrequent Access(S3 Standard-IA)로 전환합니다.
B. S3 수명 주기 규칙을 사용하여 객체를 S3 Standard에서 Standard-Infrequent Access로 전환(S3 Standard-IA)
C. S3 수명 주기 규칙을 사용하여 객체를 S3 Standard에서 S3 Intelligent-Tiering으로 전환
D. S3 Inventory를 사용하여 S3 Standard에서 S3 Intelligent-Tiering으로 액세스하지 않은 객체를 식별하고 전환

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q611
회사에서 새로운 동적 주문 웹사이트를 구축하고 있습니다. 회사는 서버 유지 관리 및 패치를 최소화하려고 합니다. 웹 사이트는 가용성이 높아야 하며 사용자 요구의 변화를 충족하기 위해 가 능한 한 빨리 읽기 및 쓰기 용량을 확장해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Amazon S3에서 정적 콘텐츠를 호스팅합니다. Amazon API Gateway 및 AWS Lambda를 사용하여 동적 콘텐츠를 호스팅합니다. 데이터베이스에 대한 온디맨드 용량과 함께
Amazon DynamoDB를 사용합니다. 웹 사이트 콘텐츠를 제공하도록 Amazon CloudFront를 구성합니다.
B. Amazon S3에서 정적 콘텐츠를 호스팅합니다. Amazon API Gateway 및 AWS Lambda를 사용하여 동적 콘텐츠를 호스팅합니다. 데이터베이스에는 Aurora Auto Scaling과 함
께 Amazon Aurora를 사용하십시오. 웹 사이트 콘텐츠를 제공하도록 Amazon CloudFront를 구성합니다.
C. Amazon EC2 인스턴스에서 모든 웹 사이트 콘텐츠를 호스팅합니다. Auto Scaling 그룹을 생성하여 EC2 인스턴스를 확장합니다. Application Load Balancer를 사용하여 트래픽
을 분산합니다. 데이터베이스에 대해 프로비저닝된 쓰기 용량과 함께 Amazon DynamoDB를 사용합니다.
D. Amazon EC2 인스턴스에서 모든 웹 사이트 콘텐츠를 호스팅합니다. Auto Scaling 그룹을 생성하여 EC2 인스턴스를 확장합니다. Application Load Balancer를 사용하여 트래픽
을 분산합니다. 데이터베이스에는 Aurora Auto Scaling과 함께 Amazon Aurora를 사용하십시오.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q612
한 회사가 us-east-1 리전 내의 3개의 별도 VPC에서 여러 비즈니스 애플리케이션을 실행하고 있습니다. 애플리케이션은 VPC 간에 통신할 수 있어야 합니다. 또한 애플리케이션은 단일 온 프레미스 데이터 센터에서 실행되는 대기 시간에 민감한 애플리케이션에 매일 수백 기가바이트의 데이터를 지속적으로 전송할 수 있어야 합니다. 솔루션 설계자는 비용 효율성을 극대화하는 네트워크 연결 솔루션을 설계해야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. 데이터 센터에서 AWS로 3개의 AWS Site-to-Site VPN 연결을 구성합니다. 각 VPC에 대해 하나의 VPN 연결을 구성하여 연결을 설정합니다. 
B. 각 VPC에서 타사 가상 네트워크 어플라이언스를 시작합니다. 데이터 센터와 각 가상 어플라이언스 간에 IPsec VPN 터널을 설정합니다. 
C. 데이터 센터에서 us-east-1의 Direct Connect 게이트웨이로 3개의 AWS Direct Connect 연결을 설정합니다. Direct Connect 연결 중 하나를 사용하도록 각 VPC를 구성하여
연결을 설정합니다.
D. 데이터 센터에서 AWS로 하나의 AWS Direct Connect 연결을 설정합니다. 전송 게이트웨이를 생성하고 각 VPC를 전송 게이트웨이에 연결합니다. Direct Connect 연결과 transit
gateway 간의 연결을 설정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q613
회사에서 Amazon 머신 이미지(AMI)를 관리하려고 합니다. 회사는 현재 AMI가 생성된 동일한 AWS 리전에 AMI를 복사합니다. 회사는 AWS API 호출을 캡처하고 회사 계정 내에서 Amazon EC2 CreateImage API 작업이 호출될 때마다 알림을 보내는 애플리케이션을 설계해야 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS CloudTrail 로그를 쿼리하고 CreateImage API 호출이 감지되면 알림을 보내는 AWS Lambda 함수를 생성합니다. 
B. 업데이트된 로그가 Amazon S3로 전송될 때 발생하는 Amazon Simple Notification Service(Amazon SNS) 알림으로 AWS CloudTrail을 구성합니다. Amazon Athena를
사용하여 새 테이블을 생성하고 API 호출이 감지되면 CreateImage에서 쿼리합니다.
C. CreateImage API 호출에 대한 Amazon EventBridge(Amazon CloudWatch Events) 규칙을 생성합니다. CreateImage API 호출이 감지되면 알림을 보내도록 대상을
Amazon Simple Notification Service(Amazon SNS) 주제로 구성합니다.
D. Amazon Simple Queue Service(Amazon SQS) FIFO 대기열을 AWS CloudTrail 로그의 대상으로 구성합니다. CreateImage API 호출이 감지되면 Amazon Simple
Notification Service(Amazon SNS) 주제에 알림을 보내는 AWS Lambda 함수를 생성합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q614
미디어 회사는 AWS에서 웹 사이트를 호스팅합니다. 웹 사이트 애플리케이션의 아키텍처에는 ALB(Application Load Balancer) 뒤에 있는 Amazon EC2 인스턴스 플릿과 Amazon Aurora에서 호스팅되는 데이터베이스가 포함됩니다. 회사의 사이버 보안 팀은 애플리케이션이 SQL 주입에 취약하다고 보고합니다. 회사는 이 문제를 어떻게 해결해야 할까요?
A. ALB 앞에서 AWS WAF를 사용합니다. 적절한 웹 ACL을 AWS WAF와 연결합니다. 
B. 고정 응답으로 SQL 주입에 응답하는 ALB 수신기 규칙을 생성합니다. 
C. 모든 SQL 삽입 시도를 자동으로 차단하려면 AWS Shield Advanced에 가입하십시오. 
D. 모든 SQL 주입 시도를 자동으로 차단하도록 Amazon Inspector를 설정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q615
솔루션 설계자는 회사의 애플리케이션을 위한 새로운 마이크로서비스를 설계해야 합니다. 클라이언트는 마이크로 서비스에 도달하기 위해 HTTPS 끝점을 호출할 수 있어야 합니다. 또한 마이 크로서비스는 AWS Identity and Access Management(IAM)를 사용하여 호출을 인증해야 합니다. 솔루션 설계자는 Go 1.x로 작성된 단일 AWS Lambda 함수를 사용하여 이 마이 크로서비스에 대한 논리를 작성합니다. 어떤 솔루션이 운영상 가장 효율적인 방식으로 기능을 배포합니까?
A. Amazon API Gateway REST API를 생성합니다. Lambda 함수를 사용하도록 메서드를 구성합니다. API에서 IAM 인증을 활성화합니다. 
B. 함수에 대한 Lambda 함수 URL을 생성합니다. 인증 유형으로 AWS_IAM을 지정합니다. 
C. Amazon CloudFront 배포를 생성합니다. 함수를 Lambda@Edge에 배포합니다. IAM 인증 로직을 Lambda@Edge 함수에 통합합니다. 
D. Amazon CloudFront 배포를 생성합니다. CloudFront Functions에 함수를 배포합니다. 인증 유형으로 AWS_IAM을 지정합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q616
회사에서 새 애플리케이션을 출시하고 Amazon CloudWatch 대시보드에 애플리케이션 지표를 표시합니다. 회사의 제품 관리자는 이 대시보드에 정기적으로 액세스해야 합니다. 제품 관리 자에게 AWS 계정이 없습니다. 솔루션 설계자는 최소 권한 원칙에 따라 제품 관리자에게 액세스 권한을 제공해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. CloudWatch 콘솔에서 대시보드를 공유합니다. 제품 관리자의 이메일 주소를 입력하고 공유 단계를 완료합니다. 제품 관리자에게 대시보드에 대한 공유 가능한 링크를 제공합니다. 
B. 제품 관리자 전용 IAM 사용자를 생성합니다. CloudWatchReadOnlyAccess AWS 관리형 정책을 사용자에게 연결합니다. 새 로그인 자격 증명을 제품 관리자와 공유하십시오. 올바
른 대시보드의 브라우저 URL을 제품 관리자와 공유하십시오.
C. 회사 직원을 위한 IAM 사용자를 생성합니다. ViewOnlyAccess AWS 관리형 정책을 IAM 사용자에게 연결합니다. 새 로그인 자격 증명을 제품 관리자와 공유하십시오. 제품 관리자에
게 CloudWatch 콘솔로 이동하여 대시보드 섹션에서 이름으로 대시보드를 찾도록 요청하십시오.
D. 퍼블릭 서브넷에 배스천 서버를 배포합니다. 제품 관리자가 대시보드에 액세스해야 하는 경우 서버를 시작하고 RDP 자격 증명을 공유합니다. 배스천 서버에서 브라우저가 대시보드를 볼
수 있는 적절한 권한이 있는 캐시된 AWS 자격 증명으로 대시보드 URL을 열도록 구성되어 있는지 확인합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q617
연구소는 약 8TB의 데이터를 처리해야 합니다. 실험실에는 스토리지 하위 시스템에 대해 1밀리초 미만의 대기 시간과 최소 6GBps의 처리량이 필요합니다. Amazon Linux를 실행하는 수 백 개의 Amazon EC2 인스턴스가 데이터를 배포하고 처리합니다. 성능 요구 사항을 충족하는 솔루션은 무엇입니까?
A. NetApp ONTAP 파일 시스템용 Amazon FSx를 생성합니다. 각 볼륨의 계층화 정책을 ALL로 설정했습니다. 원시 데이터를 파일 시스템으로 가져옵니다. EC2 인스턴스에 fila 시스
템을 탑재합니다.
B. 원시 데이터를 저장할 Amazon S3 버킷을 생성합니다. 영구 SSD 스토리지를 사용하는 Amazon FSx for Lustre 파일 시스템을 생성합니다. Amazon S3에서 데이터를 가져오고
내보내는 옵션을 선택합니다. EC2 인스턴스에 파일 시스템을 탑재합니다.
C. 원시 데이터를 저장할 Amazon S3 버킷을 생성합니다. 영구 HDD 스토리지를 사용하는 Amazon FSx for Lustre 파일 시스템을 생성합니다. Amazon S3에서 데이터를 가져오고
내보내는 옵션을 선택합니다. EC2 인스턴스에 파일 시스템을 탑재합니다.
D. NetApp ONTAP 파일 시스템용 Amazon FSx를 생성합니다. 각 볼륨의 계층화 정책을 NONE으로 설정합니다. 원시 데이터를 파일 시스템으로 가져옵니다. EC2 인스턴스에 파일
시스템을 탑재합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q618
회사는 단일 가용 영역의 Amazon EC2 인스턴스에서 3계층 웹 애플리케이션을 호스팅합니다. 웹 애플리케이션은 EC2 인스턴스에서 호스팅되는 자체 관리형 MySQL 데이터베이스를 사 용하여 Amazon Elastic Block Store(Amazon EBS) 볼륨에 데이터를 저장합니다. MySQL 데이터베이스는 현재 1TB 프로비저닝된 IOPS SSD(io2) EBS 볼륨을 사용합니다. 이 회사는 피크 트래픽에서 읽기 및 쓰기 모두에 대해 1,000 IOPS의 트래픽을 예상합니다. 회사는 두 배의 IOPS 용량을 유지하면서 중단을 최소화하고 성능을 안정화하며 비용을 절감하고자 합니다. 이 회사는 데이터베이스 계층을 가용성이 높고 내결함성이 있는 완전 관리형 솔루 션으로 이동하려고 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. io2 Block Express EBS 볼륨이 있는 MySQL DB 인스턴스용 Amazon RDS의 다중 AZ 배포를 사용합니다. 
B. 범용 SSD(gp2) EBS 볼륨이 있는 MySQL DB 인스턴스용 Amazon RDS의 다중 AZ 배포를 사용합니다. 
C. Amazon S3 Intelligent-Tiering 액세스 계층을 사용합니다. 
D. 두 개의 큰 EC2 인스턴스를 사용하여 활성-수동 모드에서 데이터베이스를 호스팅합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q619
솔루션 설계자는 대용량 SaaS(Software as a Service) 플랫폼에 대한 재해 복구(DR) 계획을 만들어야 합니다. 플랫폼의 모든 데이터는 Amazon Aurora MySQL DB 클러스터에 저 장됩니다. DR 계획은 데이터를 보조 AWS 리전에 복제해야 합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 보조 리전의 Aurora 클러스터에 MySQL 바이너리 로그 복제를 사용합니다. 보조 리전에서 Aurora 클러스터용 DB 인스턴스 1개를 프로비저닝합니다. 
B. DB 클러스터에 대한 Aurora 글로벌 데이터베이스를 설정합니다. 설정이 완료되면 보조 리전에서 DB 인스턴스를 제거합니다. 
C. AWS Database Migration Service(AWS DMS)를 사용하여 데이터를 보조 리전의 Aurora 클러스터에 지속적으로 복제합니다. 보조 리전에서 DB 인스턴스를 제거합니다. 
D. DB 클러스터에 대한 Aurora 글로벌 데이터베이스를 설정합니다. 보조 리전에서 최소 하나의 DB 인스턴스를 지정합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q620
VPC-A의 Amazon EC2 인스턴스에서 실행 중인 애플리케이션은 VPC-B의 다른 EC2 인스턴스에 있는 파일에 액세스해야 합니다. 두 VPC 모두 별도의 AWS 계정에 있습니다. 네트워 크 관리자는 VPC-A에서 VPC-B의 EC2 인스턴스에 대한 보안 액세스를 구성하는 솔루션을 설계해야 합니다. 연결에는 단일 장애 지점이나 대역폭 문제가 없어야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. VPC-A와 VPC-B 간에 VPC 피어링 연결을 설정합니다. 
B. VPC-B에서 실행되는 EC2 인스턴스에 대한 VPC 게이트웨이 엔드포인트를 설정합니다. 
C. 가상 프라이빗 게이트웨이를 VPC-B에 연결하고 VPC-A에서 라우팅을 설정합니다. 
D. VPC-B에서 실행 중인 EC2 인스턴스에 대한 프라이빗 가상 인터페이스(VIF)를 생성하고 VPC-A에서 적절한 경로를 추가합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q621
회사에서 최근 마케팅 캠페인의 효과를 측정하려고 합니다. 회사는 판매 데이터의 .csv 파일에 대해 일괄 처리를 수행하고 그 결과를 매시간 Amazon S3 버킷에 저장합니다. S3 버킷에는 페 타바이트 규모의 객체가 포함되어 있습니다. 이 회사는 Amazon Athena에서 일회성 쿼리를 실행하여 특정 지역에서 특정 날짜에 가장 인기 있는 제품을 확인합니다. 쿼리가 실행을 완료하는 데 예상보다 오래 걸리거나 실패하는 경우가 있습니다. 솔루션 설계자는 쿼리 성능과 안정성을 개선하기 위해 어떤 조치를 취해야 합니까? (두 가지를 선택하세요.)
A. S3 객체 크기를 128MB 미만으로 줄입니다. 
B. Amazon S3에서 데이터를 날짜 및 지역별로 분할합니다. 
C. 파일을 Amazon S3에 큰 단일 객체로 저장합니다. 
D. Amazon Kinesis Data Analytics를 사용하여 일괄 처리 작업의 일부로 쿼리를 실행합니다. 
E. AWS Glue 추출, 변환 및 로드(ETL) 프로세스를 사용하여 .csv 파일을 Apache Parquet 형식으로 변환합니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q622
회사는 AWS 클라우드에 수백 개의 Amazon EC2 Linux 기반 인스턴스를 보유하고 있습니다. 시스템 관리자는 공유 SSH 키를 사용하여 인스턴스를 관리했습니다. 최근 감사 후 회사의 보안 팀은 모든 공유 키를 제거하도록 지시하고 있습니다. 솔루션 설계자는 EC2 인스턴스에 대한 보안 액세스를 제공하는 솔루션을 설계해야 합니다. 최소한의 관리 오버헤드로 이 요구 사항을 충족하는 솔루션은 무엇입니까?
A. AWS Systems Manager Session Manager를 사용하여 EC2 인스턴스에 연결합니다. 
B. AWS Security Token Service(AWS STS)를 사용하여 온디맨드 방식으로 일회성 SSH 키를 생성합니다. 
C. 배스천 인스턴스 집합에 대한 공유 SSH 액세스를 허용합니다. 배스천 인스턴스에서 SSH 액세스만 허용하도록 다른 모든 인스턴스를 구성합니다. 
D. Amazon Cognito 사용자 지정 권한 부여자를 사용하여 사용자를 인증합니다. AWS Lambda 함수를 호출하여 임시 SSH 키를 생성합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q623
한 병원에서 환자의 증상을 수집하는 새로운 애플리케이션을 설계하고 있습니다. 병원은 아키텍처에서 Amazon Simple Queue Service(Amazon SQS)와 Amazon Simple Notification Service(Amazon SNS)를 사용하기로 결정했습니다. 솔루션 설계자가 인프라 디자인을 검토하고 있습니다. 저장 및 전송 중에 데이터를 암호화해야 합니다. 병원의 승인된 직원만 데이터에 액세스할 수 있어야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. SQS 구성 요소에서 서버 측 암호화를 켭니다. 기본 키 정책을 업데이트하여 인증된 보안 주체 집합으로 키 사용을 제한합니다. 
B. AWS Key Management Service(AWS KMS) 고객 관리 키를 사용하여 SNS 구성 요소에서 서버 측 암호화를 켭니다. 키 정책을 적용하여 인증된 보안 주체 집합으로 키 사용을 제
한합니다.
C. SNS 구성 요소에서 암호화를 켭니다. 기본 키 정책을 업데이트하여 인증된 보안 주체 집합으로 키 사용을 제한합니다. TLS를 통한 암호화된 연결만 허용하도록 주제 정책에서 조건을 설
정합니다.
D. AWS Key Management Service(AWS KMS) 고객 관리 키를 사용하여 SQS 구성 요소에서 서버 측 암호화를 켭니다. 키 정책을 적용하여 인증된 보안 주체 집합으로 키 사용을
제한합니다. TLS를 통한 암호화된 연결만 허용하도록 대기열 정책에서 조건을 설정합니다.
E. AWS Key Management Service(AWS KMS) 고객 관리 키를 사용하여 SQS 구성 요소에서 서버 측 암호화를 켭니다. IAM 정책을 적용하여 인증된 보안 주체 집합으로 키 사용을
제한합니다. TLS를 통한 암호화된 연결만 허용하도록 대기열 정책에서 조건을 설정합니다.

<details>
<summary>정답 보기</summary>

**BD**
</details>

---

### Q624
회사는 3계층 상태 비저장 웹 애플리케이션을 위한 백업 전략이 필요합니다. 웹 애플리케이션은 조정 이벤트에 응답하도록 구성된 동적 조정 정책이 있는 Auto Scaling 그룹의 Amazon EC2 인스턴스에서 실행됩니다. 데이터베이스 계층은 PostgreSQL용 Amazon RDS에서 실행됩니다. 웹 애플리케이션은 EC2 인스턴스에 임시 로컬 스토리지가 필요하지 않습니다. 회사 의 복구 지점 목표(RPO)는 2시간입니다. 백업 전략은 확장성을 최대화하고 이 환경에 대한 리소스 활용을 최적화해야 합니다. 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. RPO를 충족하기 위해 2시간마다 EC2 인스턴스 및 데이터베이스의 Amazon Elastic Block Store(Amazon EBS) 볼륨의 스냅샷을 생성합니다. 
B. Amazon Elastic Block Store(Amazon EBS) 스냅샷을 생성하도록 스냅샷 수명 주기 정책을 구성합니다. RPO를 충족하기 위해 Amazon RDS에서 자동 백업을 활성화합니다. 
C. 웹 및 애플리케이션 계층의 최신 Amazon 머신 이미지(AMI)를 유지합니다. Amazon RDS에서 자동 백업을 활성화하고 지정 시간 복구를 사용하여 RPO를 충족합니다. 
D. 2시간마다 EC2 인스턴스의 Amazon Elastic Block Store(Amazon EBS) 볼륨의 스냅샷을 생성합니다. Amazon RDS에서 자동 백업을 활성화하고 지정 시간 복구를 사용하여
RPO를 충족합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q625
회사는 하드웨어 용량 제약으로 인해 온프레미스 데이터 센터에서 AWS 클라우드로 레거시 애플리케이션을 마이그레이션해야 합니다. 응용 프로그램은 하루 24시간, 주 7일 실행됩니다. 애 플리케이션의 데이터베이스 저장소는 시간이 지남에 따라 계속 증가합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. 애플리케이션 계층을 Amazon EC2 스팟 인스턴스로 마이그레이션합니다. 데이터 스토리지 계층을 Amazon S3로 마이그레이션합니다. 
B. 애플리케이션 계층을 Amazon EC2 예약 인스턴스로 마이그레이션합니다. 데이터 스토리지 계층을 Amazon RDS 온디맨드 인스턴스로 마이그레이션합니다. 
C. 애플리케이션 계층을 Amazon EC2 예약 인스턴스로 마이그레이션합니다. 데이터 스토리지 계층을 Amazon Aurora 예약 인스턴스로 마이그레이션합니다. 
D. 애플리케이션 계층을 Amazon EC2 온디맨드 인스턴스로 마이그레이션합니다. 데이터 스토리지 계층을 Amazon RDS 예약 인스턴스로 마이그레이션합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q626
한 회사가 AWS 클라우드에서 3계층 전자상거래 애플리케이션을 호스팅하고 있습니다. 회사는 Amazon S3에서 웹사이트를 호스팅하고 웹사이트를 판매 요청을 처리하는 API와 통합합니 다. 이 회사는 ALB(Application Load Balancer) 뒤에 있는 3개의 Amazon EC2 인스턴스에서 API를 호스팅합니다. API는 판매 요청을 비동기식으로 처리하는 백엔드 작업자와 함께 정적 및 동적 프런트 엔드 콘텐츠로 구성됩니다. 회사는 신제품 출시 이벤트 기간 동안 판매 요청 건수가 급격하게 급증할 것으로 예상하고 있다. 모든 요청이 성공적으로 처리되도록 하려면 솔루션 설계자가 무엇을 권장해야 합니까?
A. 동적 콘텐츠에 대한 Amazon CloudFront 배포를 추가합니다. 트래픽 증가를 처리하기 위해 EC2 인스턴스 수를 늘립니다. 
B. 정적 콘텐츠에 대한 Amazon CloudFront 배포를 추가합니다. Auto Scaling 그룹에 EC2 인스턴스를 배치하여 네트워크 트래픽을 기반으로 새 인스턴스를 시작합니다. 
C. 동적 콘텐츠에 대한 Amazon CloudFront 배포를 추가합니다. ALB 앞에 Amazon ElastiCache 인스턴스를 추가하여 API가 처리할 트래픽을 줄입니다. 
D. 정적 콘텐츠에 대한 Amazon CloudFront 배포를 추가합니다. Amazon Simple Queue Service(Amazon SQS) 대기열을 추가하여 나중에 EC2 인스턴스에서 처리할 수 있도록
웹 사이트에서 요청을 수신합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q627
회사는 AWS에서 고성능 컴퓨팅(HPC) 워크로드를 실행합니다. 워크로드에는 대기 시간이 짧은 네트워크 성능과 긴밀하게 연결된 노드 간 통신을 통한 높은 네트워크 처리량이 필요했습니다 . Amazon EC2 인스턴스는 컴퓨팅 및 스토리지 용량에 맞게 적절한 크기로 지정되며 기본 옵션을 사용하여 시작됩니다. 워크로드의 성능을 개선하기 위해 솔루션 설계자는 무엇을 제안해야 합니까?
A. Amazon EC2 인스턴스를 시작하는 동안 클러스터 배치 그룹을 선택하십시오. 
B. Amazon EC2 인스턴스를 시작하는 동안 전용 인스턴스 테넌시를 선택합니다. 
C. Amazon EC2 인스턴스를 시작하는 동안 Elastic Inference 액셀러레이터를 선택합니다. 
D. Amazon EC2 인스턴스를 시작하는 동안 필요한 용량 예약을 선택합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q628
회사는 온프레미스 NAS(Network-Attached Storage) 시스템에서 AWS 클라우드로 600TB의 데이터를 전송해야 합니다. 데이터 전송은 2주 이내에 완료되어야 합니다. 데이터는 민감 하며 전송 중에 암호화되어야 합니다. 회사의 인터넷 연결은 100Mbps의 업로드 속도를 지원할 수 있습니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. Amazon S3 멀티파트 업로드 기능을 사용하여 HTTPS를 통해 파일을 전송합니다. 
B. 온프레미스 NAS 시스템과 가장 가까운 AWS 리전 간에 VPN 연결을 생성합니다. VPN 연결을 통해 데이터를 전송합니다. 
C. AWS Snow Family 콘솔을 사용하여 여러 AWS Snowball Edge Storage Optimized 디바이스를 주문합니다. 디바이스를 사용하여 데이터를 Amazon S3로 전송합니다. 
D. 회사 위치와 가장 가까운 AWS 리전 간에 10Gbps AWS Direct Connect 연결을 설정합니다. VPN 연결을 통해 데이터를 리전으로 전송하여 Amazon S3에 데이터를 저장합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q629
한 병원에서 대규모 기록 기록 수집을 위한 디지털 사본을 만들고자 합니다. 병원은 매일 수백 개의 새로운 문서를 계속 추가할 것입니다. 병원의 데이터 팀이 문서를 스캔하고 문서를 AWS 클 라우드에 업로드합니다. 솔루션 설계자는 애플리케이션이 데이터에 대해 SQL 쿼리를 실행할 수 있도록 문서를 분석하고, 의료 정보를 추출하고, 문서를 저장하는 솔루션을 구현해야 합니다. 솔루션은 확장성과 운영 효율성을 극대화해야 합니다. 솔루션 설계자는 이러한 요구 사항을 충족하기 위해 어떤 단계 조합을 수행해야 합니까? (두 가지를 선택하세요.)
A. MySQL 데이터베이스를 실행하는 Amazon EC2 인스턴스에 문서 정보를 씁니다. 
B. 문서 정보를 Amazon S3 버킷에 씁니다. Amazon Athena를 사용하여 데이터를 쿼리합니다. 
C. Amazon EC2 인스턴스의 Auto Scaling 그룹을 생성하여 스캔한 파일을 처리하고 의료 정보를 추출하는 사용자 지정 애플리케이션을 실행합니다. 
D. 새 문서가 업로드될 때 실행되는 AWS Lambda 함수를 생성합니다. Amazon Rekognition을 사용하여 문서를 원시 텍스트로 변환합니다. Amazon Transcribe Medical을 사용하
여 텍스트에서 관련 의료 정보를 감지하고 추출합니다.
E. 새 문서가 업로드될 때 실행되는 AWS Lambda 함수를 생성합니다. Amazon Textract를 사용하여 문서를 원시 텍스트로 변환합니다. Amazon Comprehend Medical을 사용하
여 텍스트에서 관련 의료 정보를 감지하고 추출합니다.

<details>
<summary>정답 보기</summary>

**BE**
</details>

---

### Q630
회사의 보고 시스템은 매일 수백 개의 .csv 파일을 Amazon S3 버킷에 전달합니다. 회사는 이러한 파일을 Apache Parquet 형식으로 변환하고 변환된 데이터 버킷에 파일을 저장해야 합 니다. 최소한의 개발 노력으로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. Apache Spark가 설치된 Amazon EMR 클러스터를 생성합니다. 데이터를 변환하는 Spark 애플리케이션을 작성합니다. EMRFS(EMR 파일 시스템)를 사용하여 변환된 데이터 버
킷에 파일을 씁니다.
B. AWS Glue 크롤러를 생성하여 데이터를 검색합니다. AWS Glue 추출, 변환 및 로드(ETL) 작업을 생성하여 데이터를 변환합니다. 출력 단계에서 변환된 데이터 버킷을 지정합니다. 
C. AWS Batch를 사용하여 Bash 구문으로 작업 정의를 생성하여 데이터를 변환하고 데이터를 변환된 데이터 버킷으로 출력합니다. 작업 정의를 사용하여 작업을 제출합니다. 어레이 작업
을 작업 유형으로 지정합니다.
D. 데이터를 변환하고 변환된 데이터 버킷으로 데이터를 출력하는 AWS Lambda 함수를 생성합니다. S3 버킷에 대한 이벤트 알림을 구성합니다. 이벤트 알림의 대상으로 Lambda 함수
를 지정합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q631
회사는 AWS Organizations를 사용하여 여러 부서의 여러 AWS 계정을 관리합니다. 마스터 계정에는 프로젝트 보고서가 포함된 Amazon S3 버킷이 있습니다. 회사는 이 S3 버킷에 대 한 액세스를 AWS Organizations의 조직 내 계정 사용자로만 제한하려고 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. 조직 ID에 대한 참조와 함께 aws PrincipalOrgID 전역 조건 키를 S3 버킷 정책에 추가합니다. 
B. 각 부서에 대한 조직 단위(OU)를 만듭니다. aws:PrincipalOrgPaths 전역 조건 키를 S3 버킷 정책에 추가합니다. 
C. AWS CloudTrail을 사용하여 CreateAccount, InviteAccountToOrganization, LeaveOrganization 및 RemoveAccountFromOrganization 이벤트를 모니터링합니다.
그에 따라 S3 버킷 정책을 업데이트합니다.
D. S3 버킷에 액세스해야 하는 각 사용자에게 태그를 지정합니다. aws:PrincipalTag 전역 조건 키를 S3 버킷 정책에 추가합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q632
회사의 애플리케이션은 데이터 수집을 위해 여러 SaaS(Software-as-a-Service) 소스와 통합됩니다. 회사는 Amazon EC2 인스턴스를 실행하여 데이터를 수신하고 분석을 위해 데이터 를 Amazon S3 버킷에 업로드합니다. 데이터를 수신하고 업로드하는 동일한 EC2 인스턴스도 업로드가 완료되면 사용자에게 알림을 보냅니다. 회사는 느린 응용 프로그램 성능을 발견했으 며 성능을 최대한 개선하고자 합니다. 최소한의 운영 오버헤드로 이러한 요구 사항을 충족하는 솔루션은 무엇입니까?
A. EC2 인스턴스가 확장될 수 있도록 Auto Scaling 그룹을 생성합니다. S3 버킷에 대한 업로드가 완료되면 Amazon Simple Notification Service(Amazon SNS) 주제로 이벤트
를 보내도록 S3 이벤트 알림을 구성합니다.
B. 각 SaaS 소스와 S3 버킷 간에 데이터를 전송하는 Amazon AppFlow 흐름을 생성합니다. S3 버킷에 대한 업로드가 완료되면 Amazon Simple Notification Service(Amazon
SNS) 주제로 이벤트를 보내도록 S3 이벤트 알림을 구성합니다.
C. 각 SaaS 소스에 대한 Amazon EventBridge(Amazon CloudWatch Events) 규칙을 생성하여 출력 데이터를 보냅니다. S3 버킷을 규칙의 대상으로 구성합니다. S3 버킷에 대한
업로드가 완료되면 이벤트를 전송하는 두 번째 EventBridge(Cloud Watch Events) 규칙을 생성합니다. Amazon Simple Notification Service(Amazon SNS) 주제를 두 번째 규칙의 대상으로 구성합니다.
D. EC2 인스턴스 대신 사용할 Docker 컨테이너를 생성합니다. Amazon Elastic Container Service(Amazon ECS)에서 컨테이너화된 애플리케이션을 호스팅합니다. S3 버킷에 대
한 업로드가 완료되면 Amazon Simple Notification Service(Amazon SNS) 주제로 이벤트를 보내도록 Amazon CloudWatch Container Insights를 구성합니다.

<details>
<summary>정답 보기</summary>

**B**
</details>

---

### Q633
솔루션 설계자는 고객 사례 파일을 저장할 시스템을 설계해야 합니다. 파일은 핵심 회사 자산이며 중요합니다. 파일 수는 시간이 지남에 따라 증가합니다. 파일은 Amazon EC2 인스턴스에서 실행되는 여러 애플리케이션 서버에서 동시에 액세스할 수 있어야 합니다. 솔루션에는 중복성이 내장되어 있어야 합니다. 어떤 솔루션이 이러한 요구 사항을 충족합니까?
A. Amazon Elastic File System(Amazon EFS) 
B. Amazon Elastic Block Store(Amazon EBS) 
C. Amazon S3 Glacier Deep 아카이브 
D. AWS 백업

<details>
<summary>정답 보기</summary>

**A**
</details>

---

### Q634
회사에서는 SSL/TLS 인증서를 사용하도록 Amazon CloudFront 배포를 구성하려고 합니다. 회사는 배포에 기본 도메인 이름을 사용하기를 원하지 않습니다. 대신 회사는 배포에 다른 도 메인 이름을 사용하기를 원합니다. 추가 비용 없이 인증서를 배포할 수 있는 솔루션은 무엇입니까?
A. us-east-1 지역의 AWS Certificate Manager(ACM)에서 Amazon 발급 사설 인증서를 요청합니다. 
B. us-west-1 지역의 AWS Certificate Manager(ACM)에서 Amazon 발급 개인 인증서를 요청합니다. 
C. us-east-1 지역의 AWS Certificate Manager(ACM)에서 Amazon 발급 공인 인증서를 요청합니다. 
D. us-west-1 지역의 AWS Certificate Manager(ACM)에서 Amazon 발급 공인 인증서를 요청합니다.

<details>
<summary>정답 보기</summary>

**C**
</details>

---

### Q635
회사의 애플리케이션이 AWS에서 실행됩니다. 애플리케이션은 S3 Standard-infrequent Access(S3 Standerd-IA) 스토리지 클래스를 사용하는 Amazon S3 버킷에 대용량 문서를 저장합니다. 회사는 데이터 저장 비용을 계속 지불하지만 총 S3 비용을 절감하고자 합니다. 회사는 승인된 외부 사용자가 밀리초 단위로 문서에 액세스할 수 있기를 원합니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 솔루션은 무엇입니까?
A. 요청자 지불 버킷이 되도록 S3 버킷을 구성합니다.
B. 모든 기존 객체와 향후 객체에 대해 스토리지 계층을 S3 Standard로 변경합니다.
C. S3 Docket에서 S3 Transfer Acceleration을 켭니다.
D. Amazon CloudFront를 사용하여 S3 버킷에 대한 모든 요청을 처리합니다.

<details>
<summary>정답 보기</summary>

**D**
</details>

---

### Q636
회사에는 Amazon EC2 인스턴스에서 실행되고 Amazon Aurora 데이터베이스를 사용하는 애플리케이션이 있습니다. EC2 인스턴스는 파일에 로컬로 저장된 사용자 이름과 암호를 사용 하여 데이터베이스에 연결합니다. 회사는 자격 증명 관리의 운영 오버헤드를 최소화하려고 합니다. 이 목표를 달성하기 위해 솔루션 설계자는 무엇을 해야 합니까?
A. AWS Secrets Manager를 사용하십시오. 자동 회전을 켭니다. 
B. AWS Systems Manager Parameter Store를 사용합니다. 자동 회전을 켭니다. 
C. AWS Key Management Service(AWS KMS) 암호화 키로 암호화된 객체를 저장할 Amazon S3 버킷을 생성합니다. 자격 증명 파일을 S3 버킷으로 마이그레이션합니다. 애플리
케이션이 S3 버킷을 가리키도록 합니다.
D. 각 EC2 인스턴스에 대해 암호화된 Amazon Elastic Block Store(Amazon EBS) 볼륨을 생성합니다. 새 EBS 볼륨을 각 EC2 인스턴스에 연결합니다. 자격 증명 파일을 새 EBS
볼륨으로 마이그레이션합니다. 애플리케이션이 새 EBS 볼륨을 가리키도록 합니다.

<details>
<summary>정답 보기</summary>

**A**
</details>

---
