# Abdalrahman Ehab - 500 Days of Software

## Day 1

- Learned Spring Security filter chain internals (DelegatingFilterProxy, CsrfFilter, stateless vs stateful sessions)
[lecture -1](https://www.youtube.com/watch?v=XosclYEA6GI&list=PLchS000MeasykSXFB0Knu8-dMpnVBcWkq).

## Day 2

- finshed last hour of the lecture and learned the full archticture of authorization filter

## Day 3

- finshed JWT and Oauth2.0 archticture and Internal Configuration

## Day 4 (21/11)
- finshed second lecture and learned OIDC and the SSL flow 
- Implemented JWT config, JwtService, CustomUserDetailsService, and JwtAuthenticationFilter - [Link](https://github.com/abdalrahmanehab/spring-commerce/compare/main...feat/security-jwt)

## Day 5 (22/11)
- Finished the JWT security [PR](https://github.com/abdalrahmanehab/spring-commerce/pull/8): added login, user endpoints, role-based rules, and IDOR checks, tested in Postman, and merged into main

## Day 6 (23/11)
- Revised Spring Security and JWT in depth, focusing on interview topics
- Planned the next steps for spring-commerce: pagination, N+1 fix, testing, concurrency and Docker

## Day 7 (24/11)
- Added DTO validation to spring-commerce (cart quantity and price limits)
- Added optimistic locking (@Version) to Product and Order
- Moved ProductRepository to Spring Data JPA and updated the Liquibase migrations

## Day 8 (25/11)
- Started contributing to Apache Fineract (FINERACT-3254)
- Studied how QueryDSL is used in the codebase

## Day 9 (26/11)
- Moved retrieveAllActiveAdHocQuery from native SQL to QueryDSL (SQLQueryFactory)
- Added PostgreSQL and MySQL unit tests and ran Spotless
- Opened the FINERACT-3254 pull request