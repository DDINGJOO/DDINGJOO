# Backend & Platform Engineer

I build and operate backend systems and the platform under them:
infrastructure as code, observability, cost, and security.

## What I've been working on
- **Infrastructure as Code** — brought an existing, console-built AWS environment under Terraform
  by importing live resources, with guardrails against destroy and drift
- **Observability** — monitors and dashboards as code, SLO-based alerting, and finding what
  monitoring silently misses
- **Cloud cost** — measuring where the bill comes from and cutting it without losing safety margins
- **Security** — default-deny authorization in Spring Security, column-level encryption of
  personal data (AES-256-GCM via JPA converters), secrets out of config files

## Open Source Contributions

### Merged
| Project | Contribution | Pull Request |
|--------|-------------|-------------|
| Spring Security | Applied the javadoc-warnings-error policy to the `spring-security-aspects` module, aligning it with the rest of the build | [#18855](https://github.com/spring-projects/spring-security/pull/18855) |
| Micrometer | Documented Jakarta Mail instrumentation and registered it in the Observation instrumented-projects reference | [#7256](https://github.com/micrometer-metrics/micrometer/pull/7256) |

### In Review
| Project | Contribution | Pull Request |
|--------|-------------|-------------|
| Spinnaker (Orca) | Fixed a race where a duplicate `StartExecution` delivery could move a completed pipeline back to `RUNNING`, using a conditional status update (`SELECT ... FOR UPDATE`) | [#8174](https://github.com/spinnaker/spinnaker/pull/8174) |
| Spring Batch | Truncated the execution context `SHORT_CONTEXT` by UTF-8 length so multibyte contexts no longer fail on Oracle (reproduced on Oracle 23) | [#5582](https://github.com/spring-projects/spring-batch/pull/5582) |
| Spring Cloud Config | Expired the Git refresh rate when `/monitor` receives a webhook, so refreshed applications get the new commit | [#3342](https://github.com/spring-cloud/spring-cloud-config/pull/3342) |
| Spring Boot | Made Docker Compose support fail fast on unsupported `*_FILE` credential variables instead of silently falling back to defaults | [#52120](https://github.com/spring-projects/spring-boot/pull/52120) |
| Spring AI | Added unit tests for `ErrorLoggingObservationHandler` | [#7125](https://github.com/spring-projects/spring-ai/pull/7125) |

## Certifications
![AWS Developer Associate](https://img.shields.io/badge/AWS_Certified_Developer-Associate-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Engineer Information Processing](https://img.shields.io/badge/Engineer_Information_Processing-정보처리기사-0066CC?style=for-the-badge&logoColor=white)
![SQLD](https://img.shields.io/badge/SQL_Developer-SQLD-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

## Contact
[![Blog](https://img.shields.io/badge/Blog-FF5722?style=for-the-badge&logo=blogger&logoColor=white)](https://dding-shark.tistory.com/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/DDINGJOO)

## Career
**Backend & Platform Engineer** · 2026-06 – present

**TeamBind Inc.** · Backend Engineer/CTO
2025-07-01 – 2026-06-22

- Designed and built microservices-based systems as the sole backend engineer, owning the full stack from infrastructure to application
- Operated a self-managed (on-premises) Kubernetes cluster, including incident response and troubleshooting
- Designed database schemas and data models for core services
- Developed both web and app-facing backend services end to end
