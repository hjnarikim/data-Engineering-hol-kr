# 2.Lab:Ingestion with DMS

## 2.Lab: Ingestion with DMS

#### 안내

AWS Database Migration Service (AWS DMS) 를 사용하면 데이터베이스를 AWS로 빠르고 안전하게 마이그레이션할 수 있습니다. 소스 데이터베이스는 마이그레이션 중에도 완벽하게 작동하므로 데이터베이스를 사용하는 애플리케이션의 다운타임을 최소화할 수 있습니다. AWS DMS 는 널리 사용되는 상용 및 오픈소스 데이터베이스를 소스 또는 타겟으로 삼아 데이터를 마이그레이션할 수 있습니다.

AWS DMS는 Oracle to Oracle 같은 동종 마이그레이션 뿐만 아니라 Oracle/MS SQL to Amazon Aurora 같은 이종 데이터베이스 플랫폼 간의 마이그레이션도 지원합니다. 또한 AWS DMS를 사용하면 지원하는 모든 소스 및 타겟에 대해 데이터를 지속적으로 복제할 수 있습니다. 예를 들어 여러 소스에서 Amazon S3 로 복제하여 가용성과 확장성이 뛰어난 데이터 레이크를 구축하거나, 데이터를 Amazon Redshift로 스트리밍하여 데이터베이스를 페타바이트 규모의 데이터 웨어하우스로 통합할 수 있습니다.

이 실습은 데이터 분석을 위한 사전작업으로, AWS DMS 를 활용하여 이미 만들어진 Amazon Relational Database Service (Amazon RDS) Postgres 관계형 데이터베이스로부터 Amazon Simple Storage Service (Amazon S3) 버킷으로 데이터를 마이그레이션하게 됩니다.

***

## DMS Migration Lab

이번 실습동안 아래와 같은 작업을 수행하게 됩니다:

1. DMS Lab VPC 에 subnet group 생성
2. DMS replication instance 생성
3. DMS source endpoint 생성
4. DMS target endpoint 생성
5. Initial full copy 수행을 위한 Task 생성

(옵션) 추가적으로 소스 데이터 변경분을 지속적으로 복제하는 CDC 기능에 대한 실습도 가능합니다:

1. CDC 파일을 위한 별도의 Target endpoint 생성
2. CDC 수행을 위한 Task 생성

![image](https://user-images.githubusercontent.com/87927874/197393792-80535478-6f1f-4f39-bf13-f933233f49ae.png)

아래를 클릭하시어, DMS 를 위한 실습가이드로 이동합니다.

* [2-1. DMS Preparation](2-1.dmspreparation.md)
* [2-2. DMS Full Load](2-2.dmsfullload.md)
* [2-3. (Optional) DMS Ongoing Replication](2-3.dmscdc.md)
