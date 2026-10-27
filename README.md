# Platform Engineer & DevOps

I build and operate the platform that backend services run on:
infrastructure as code, deployment, observability, cost, and security.
I come from backend engineering, so I work on both sides of that line.

## Certifications
![AWS Developer Associate](https://img.shields.io/badge/AWS_Certified_Developer-Associate-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Engineer Information Processing](https://img.shields.io/badge/Engineer_Information_Processing-정보처리기사-0066CC?style=for-the-badge&logoColor=white)
![SQLD](https://img.shields.io/badge/SQL_Developer-SQLD-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

## Career
**Platform Engineer & DevOps** · 2026-06 – present
- **Infrastructure platform** — brought a console-built AWS environment under Terraform with OIDC-based workflows
- **Observability** — monitoring managed as code, alerting moved to SLOs
- **Deploy & cost** — improved the internal deployment pipeline (blue-green); traced where the cloud bill comes from and cut it
- **Security** — default-deny authorization, column-level encryption of personal data, ISO 27001 / ISMS-P preparation

**TeamBind** · Backend Engineer / CTO · 2025-07 – 2026-06<br>
<sub>A space-booking and community platform for musicians</sub>
- Designed and built a microservices architecture as the sole backend engineer
- Built and operated a self-managed (on-premises) Kubernetes cluster, including incident response
- Designed database schemas and data models for core services
- Developed web and app backends end to end

## Stack
<table>
  <tr><td><b>Primary</b></td><td><img alt="Spring" src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> <img alt="AWS" src="assets/aws.svg"> <img alt="Terraform" src="https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white"> <img alt="Kubernetes" src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"></td></tr>
  <tr><td><b>Comfortable</b></td><td><img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"> <img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"> <img alt="MySQL" src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"> <img alt="Redis" src="https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white"> <img alt="Kafka" src="https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white"></td></tr>
</table>

## Open Source Contributions

### Merged
| Project | Contributions |
|--------|---------------|
| **OpenTelemetry**<br><sub>Java instrumentation</sub> | • [#20845](https://github.com/open-telemetry/opentelemetry-java-instrumentation/pull/20845) Fixed the agent no longer propagating context through Reactor operators after the application calls `Hooks.resetOnEachOperator()`, which broke the context of externally driven `Flux.create` subscribers<br>• [#20659](https://github.com/open-telemetry/opentelemetry-java-instrumentation/pull/20659) Fixed `@WithSpan` on a `Flux` requesting 32 elements from the source regardless of downstream demand, which dropped queued work on cancel<br>• [#20658](https://github.com/open-telemetry/opentelemetry-java-instrumentation/pull/20658) Fixed Spring Kafka listeners with async acks or async return types emitting a duplicate Kafka client process span per record (a 2.32.0 regression)<br>• [#20660](https://github.com/open-telemetry/opentelemetry-java-instrumentation/pull/20660) Fixed MySQL/MariaDB `address=(host=..)(port=..)` JDBC URLs without a subprotocol losing `server.address`/`server.port`<br>• [#20661](https://github.com/open-telemetry/opentelemetry-java-instrumentation/pull/20661) Fixed the Lettuce library reporting the command name (e.g. `BLPOP.`) as `error.type` on client-side timeouts |
| **Spinnaker**<br><sub>Orca</sub> | [#8174](https://github.com/spinnaker/spinnaker/pull/8174) Fixed a race where a duplicate `StartExecution` delivery could move a completed pipeline back to `RUNNING`, using a conditional status update (`SELECT ... FOR UPDATE`) |
| **Debezium** | [#8220](https://github.com/debezium/debezium/pull/8220) Fixed a regression in the generated MySQL DDL grammar where `ALTER DATABASE` without a database name failed to parse and stopped the connector |
| **ANTLR grammars-v4** | • [#5037](https://github.com/antlr/grammars-v4/pull/5037) Made the schema name optional in the MySQL `alterDatabase` rule, the upstream source of the Debezium grammar fixed in #8220<br>• [#5039](https://github.com/antlr/grammars-v4/pull/5039) Fixed the MariaDB grammar taking `DEFAULT` as the database name in `ALTER DATABASE DEFAULT CHARSET ...`, upstream of one of the two grammars fixed in #8225 (the other, Positive-Technologies, is deprecated upstream and not accepting fixes) |
| **Keycloak** | [#53990](https://github.com/keycloak/keycloak/pull/53990) Fixed `AccessTokenContext` validating `grantType` twice instead of `rawTokenId`, so a null token id reached the encoded token id as the literal `null` rather than failing at construction |
| **Lettuce**<br><sub>Redis Java client</sub> | • [#3952](https://github.com/redis/lettuce/pull/3952) Fixed `DefaultEndpoint` validating `clientOptions` twice so a null `clientResources` bypassed the null check and surfaced later as an NPE away from the construction site<br>• [#3955](https://github.com/redis/lettuce/pull/3955) Fixed assertion messages that named the wrong argument: a misspelled `ReauthenticateBehavior` in a public builder, and `CompressionCodec` reporting a `null` output stream as the input<br>• [#3954](https://github.com/redis/lettuce/pull/3954) Fixed typos in the Javadoc of the stream `XACK` and `XLEN` commands across every API flavor, plus other comment typos |
| **Spring Cloud Config** | [#3342](https://github.com/spring-cloud/spring-cloud-config/pull/3342) Expired the Git refresh rate when `/monitor` receives a webhook, so refreshed applications get the new commit |
| **Spring Security** | [#18855](https://github.com/spring-projects/spring-security/pull/18855) Applied the javadoc-warnings-error policy to the `spring-security-aspects` module, aligning it with the rest of the build |
| **Micrometer** | [#7256](https://github.com/micrometer-metrics/micrometer/pull/7256) Documented Jakarta Mail instrumentation and registered it in the Observation instrumented-projects reference |

### In Review
| Project | Contributions |
|--------|---------------|
| **Spinnaker**<br><sub>Orca</sub> | • [#8208](https://github.com/spinnaker/spinnaker/pull/8208) Made `StartExecution`'s rollback after a failed `StartStage` push conditional, so a cancel made in that window is no longer overwritten and the redelivered message doesn't start the canceled pipeline (reproduced against MySQL)<br>• [#8209](https://github.com/spinnaker/spinnaker/pull/8209) Added a test that depends on the row lock in `updateStatusIfExpected`; it fails if `SELECT ... FOR UPDATE` is removed |
| **Debezium** | [#8225](https://github.com/debezium/debezium/pull/8225) Fixed the MariaDB and legacy MySQL grammars taking `DEFAULT` as a database name in `ALTER DATABASE DEFAULT CHARSET ...`, which silently skipped the charset change (follow-up requested by the maintainer) |
| **Spring Batch** | [#5582](https://github.com/spring-projects/spring-batch/pull/5582) Truncated the execution context `SHORT_CONTEXT` by UTF-8 length so multibyte contexts no longer fail on Oracle (reproduced on Oracle 23) |
| **Spring Boot** | [#52120](https://github.com/spring-projects/spring-boot/pull/52120) Made Docker Compose support fail fast on unsupported `*_FILE` credential variables instead of silently falling back to defaults |
| **Spring AI** | [#7125](https://github.com/spring-projects/spring-ai/pull/7125) Added unit tests for `ErrorLoggingObservationHandler` |

## Writing
I write up what I learn on [my blog](https://dding-shark.tistory.com/): SRE and observability, IaC work logs, incident response and more (180+ posts).

## Contact
[![Blog](https://img.shields.io/badge/Blog-FF5722?style=for-the-badge&logo=blogger&logoColor=white)](https://dding-shark.tistory.com/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/DDINGJOO)
