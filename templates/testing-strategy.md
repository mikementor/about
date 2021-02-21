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
7. Resource risks
8. Performance risks
9. Unexpected risks
10. Something else


----
*Approaches*

1. Automation
    1. Hierarchy of automation
        1. Static checks (code quality -tools, eslint, prettier, sonar, ... )
2. Monitoring & notifications
    1. Health checks
    1. ELK / Prometheus / 
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
            2. Delivery standards (Dockerfile/docker-compose/etc)
            3. Automated checks
        2. Workflow gGuides             
    3. For delivery
        1. Failing build on failing checks
7. CI / CD
    1. ...
8. Something else