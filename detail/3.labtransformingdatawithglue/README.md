# 3.Lab: Transforming data with Glue

### Introduction

이 Lab에서는 분석, 머신 러닝(ML) 및 애플리케이션 개발을 위해 여러 소스의 데이터를 더 쉽게 검색, 준비, 이동 및 통합할 수 있는 서버리스 데이터 통합 서비스인 AWS Glue에 대해 알아봅니다. 크롤러를 사용하여 AWS 글루 데이터 카탈로그를 테이블로 채울 수 있습니다. 이는 대부분의 AWS 글루 사용자가 주로 사용하는 방법입니다. 크롤러는 한 번의 실행으로 여러 데이터 저장소를 크롤링할 수 있습니다.\
완료되면 크롤러가 데이터 카탈로그에서 하나 이상의 테이블을 만들거나 업데이트합니다.\
AWS 글루에서 정의하는 ETL(추출, 변환 및 로드) 작업은 이러한 데이터 카탈로그 테이블을 원본 및 대상으로 사용합니다. ETL 작업은 원본 및 대상 데이터 카탈로그 테이블에 지정된 데이터 저장소를 읽고 씁니다.\
이 Lab에서는 완벽하게 관리되는 데이터 카탈로그 및 ETL 서비스인 [AWS Glue](https://aws.amazon.com/ko/glue/?whats-new-cards.sort-by=item.additionalFields.postDateTime\&whats-new-cards.sort-order=desc)에 대해 설명합니다.

#### 이 Lab의 주요 **Architecture는** 다음과 같습니다.

![3-1](https://user-images.githubusercontent.com/105655711/191423889-82cbe5df-3c4e-4e90-b42f-cd728b1da5f3.png)

***

**사전 준비 사항**\
`앞선 [2.Lab: Ingestion with DMS]()을 선행해야 하는 Lab입니다.`

이 실습은 앞서 DMS를 통해 원본데이터를 S3로 가져온 다음 Lab4에서 Amazon Athena 및 Visualize with Amazon Quicksight를 사용하여 테이블을 쿼리할 수 있도록 Glue를 통해서 데이터를 변환을 수행합니다.

아래를 클릭하시어, Glue를 위한 실습가이드로 이동합니다.\
[3-1.Data Validation and ETL - Create Glue Crawler for initial full load data](3-1.creategluecrawlerforinitialfullloaddata.md)\
[3-2.Data Validation and ETL - Data Validation Exercise](3-2.datavalidationexercise.md)\
[3-3.Data Validation and ETL - Data ETL Exercise](3-3.dataetlexercise.md)\
[3-4.Data Validation and ETL - Create Glue Crawler for Parquet Files](3-4.creategluecrawlerforparquetfiles.md)
