nest new vocabulary-list-Sever --skip-git
--skip-git: 프로젝트 생성 시 Git 초기화를 생략합니다.

.eslintrc.js

용도: 코드 스타일 검사 및 규칙 정의 파일입니다.
필요 여부: ESLint를 사용하지 않을 경우 삭제 가능합니다.
.prettierrc

용도: 코드 포맷팅 규칙을 정의하는 파일입니다.
필요 여부: Prettier를 사용하지 않을 경우 삭제 가능합니다.
nest-cli.json

용도: NestJS CLI 설정 파일로, 컴파일과 빌드 관련 설정을 포함합니다.
필요 여부: 필수 파일입니다. 삭제하면 NestJS CLI가 정상 동작하지 않습니다.
package-lock.json

용도: 프로젝트 의존성을 정확히 기록하는 파일입니다.
필요 여부: 필수 파일입니다. 삭제하면 의존성 관리에 문제가 생길 수 있습니다.
package.json

용도: 프로젝트 의존성 및 스크립트를 관리하는 파일입니다.
필요 여부: 필수 파일입니다. 삭제 불가.
README.md

용도: 프로젝트 설명을 포함하는 파일입니다.
필요 여부: 설명 문서를 필요로 하지 않는 경우 삭제 가능합니다.
tsconfig.build.json

용도: 빌드 시 TypeScript 설정을 정의합니다.
필요 여부: 필수 파일입니다. 삭제 불가.
tsconfig.json

용도: 프로젝트 전역 TypeScript 설정 파일입니다.
필요 여부: 필수 파일입니다. 삭제 불가.

최근 가장 많이 사용되는 방식
TypeORM: 여전히 가장 널리 사용되며 안정적.
Prisma: 최신 프로젝트에서 채택률이 급증.
MikroORM: 경량 프로젝트 및 성능 중심 애플리케이션에 적합.


1. TypeORM의 특징
객체-테이블 매핑:
    클래스(엔터티)를 데이터베이스 테이블과 매핑하여 SQL 쿼리를 생성하고 실행.
Active Record 및 Data Mapper 패턴 지원:
    Active Record: 엔터티 클래스 자체에서 데이터 조작(삽입, 조회 등)을 처리.
    Data Mapper: Repository를 사용하여 데이터 조작을 분리.
다양한 데이터베이스 지원:
    MySQL, PostgreSQL, MariaDB, SQLite, Microsoft SQL Server 등 대부분의 SQL 데이터베이스를 지원.
타입스크립트 친화적:
    TypeScript로 작성되어 타입 안전성을 보장.
데코레이터 기반:
    데코레이터(@Entity, @Column)를 사용해 직관적으로 엔터티와 필드를 정의.

2. 왜 PostgreSQL인가?
장점
    1.오픈 소스: 무료로 사용 가능하며, 커뮤니티 지원이 활발.
    2.JSON 지원: JSON 데이터를 저장하고 쿼리할 수 있어 NoSQL처럼 활용 가능.
    3.트랜잭션: 복잡한 트랜잭션 처리가 가능.
    4.강력한 성능:
        복잡한 데이터 분석과 대규모 데이터를 처리하는 데 적합.
        파티셔닝, 인덱스 등 고급 기능 제공.
    5.확장성:
        PostGIS 확장으로 공간 데이터 지원(GIS 애플리케이션에 유용).
단점
    설정이 MySQL에 비해 조금 더 복잡할 수 있음.
    초보자에게는 학습 곡선이 있을 수 있음.