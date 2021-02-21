 > ⚠️ chapter under work. For comments, refer to that [issue](https://github.com/mikementor/mikementor/issues/7)

1. Context
2. Risks
3. Approaches

----
*Context*

1. Resources
    1. Team
    2. Delivery dates
    3. Amount of work already done ()
    4. Amount of digested/prepared/unprepared domain knowledge
2. Constraints
    1. ....
3. Something else

-----
*Risks*

1. Functional risks
    1. Don't work as intended
    2. We don't know, when it fails   ( --> monitoring and notification systems )
    3. Intentions(requirements) are incomplete or horribly incorrect
2. Infrastructure risks
3. 3rd party risks
4. Security risks
5. Legal risks (legislations come in the way, also standards like PCI DSS (Payment Card Industry Data Security Standard) )
6. Market risks ( we don't do thing, people want/need/will buy)
    1. Demand risks
    2. ...
7. Inflexible design (prevents/makes it harder and slower to change the system)
8. Resource risks
9. Performance risks
10. Unexpected risks
    1. Bug makes it to the production
        1. Approach - fast hotfix delivery
        2. Approach - fast rollback
            1. Data backups
                1. Requires backups training
11. Uncovered risks (Did we miss something?)
    1. Approach - risk-based modeling (STAMP,STPA)
12. Testing misses cases
    1. Approach - quality criteria to the requirements
    2. Approach - quality criteria to testing
    3. Approach - test case design techniques usage
13. Developed test strategy degradation with time
    1. Approach - scheduled reviews
14. Hard debuggability in microservices environment
    1. Approach - observability(distributed tracing,log aggregation) [links](https://microservices.io/patterns/observability/distributed-tracing.html)
15. Code coverage, but checks doesn't really assert anything
    1. Approach - mutation testing [PIT for Java](https://pitest.org/)
16. Something else


----
*Approaches*

1. Automation
    1. Hierarchy of automation
        1. Static checks (code quality -tools, eslint, prettier, sonar, ... )
2. Monitoring & notifications
    1. Health checks
    1. ELK / Prometheus /  Grafana / Jenkins monitors
    2. Any alerts (ElastAlerts...)
3. Testable design
    1. ...
    2. Standardazing response/error messages
        1. ...
4. Feature flagging
5. Testing
6. Quality gates
    1. For requirements
    2. For implementation
        1. For repo
            1. Readme standards
            2. Delivery standards (Dockerfile/docker-compose/health-check routes etc)
            3. Automated checks
        2. Workflow guides             
    3. For delivery
        1. Failing build on failing checks
7. CI / CD
    1. ...
8. Coverage
    1. Code coverage
        1. Different types of coverages
        2. Thresholds and quality gates
    2. Test coverage(including RTM)
    3. ...
9. Automation execution optimizations
    1. Parallelization
    2. Grouping and running in order
        1. smokes/recent/fastest/longest/riskiest/feature-component related first
    3. CI triggers
    4. Nightly builds/check run
10. Automation developing optimizations
    1. Entrypoint with guides for faster onboarding
    2. Splitting responsibility between types of automations
    3. Unifying body of checks (abstracting preparations(arrangements), actions, assertions, test data-access)
    4. Test data / state of the app preparation
        1. DB dumps / SQL scripts
        2. Data generation
        3. ...
    5. Reducing scope of what to automate (details? [⚠️])
    6. Rewriting flaky checks on different levels(e2e-> units)
    7. Removing flaky checks completely 
    8. [small tip] Using Intellij Idea Live Templates for quick checks add
    9. Ability to develop checks before implementation without  failing the CI
11. Automation reporting optimizations   
12. Static checks
    1. Code styles/code smells
    2. Specification diff checks (swagger-diff..)
13. Backward-compatible development
14. Environment setup
    1. Ability to perform all reasonable checks on local instance of the app
    2. Single availiable test environment
    3. Test environment that can be  spinned up on demand
15. Insights optimizations
    1. History of check results ( e.g. allure jenkins plugin)
    2. Traceability of check results up to components/features/requirements
    3. Having a single entrypoint for all check results/metrics
16. Completeness optimizations
    1. Test case design techniques
        1. Boundary Value Analysis
        2. Error guessing
        3. State Transition Techniques
        4. Decision Table Techniques
        5. Equivalence partitioning 
        6. ...
    2. Testing heuristics
        1. ...
    3. Modeling 
        1. ...
17. Reducing amount of checks 
18. System design
    1. Microservices [patterns](https://microservices.io/patterns/index.html)
19. Something else