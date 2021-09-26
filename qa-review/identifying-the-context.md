### Questions to identify context of the project

 > ⚠️ chapter under work. For comments, refer to that [issue](https://github.com/mikementor/mikementor/issues/8)

 > 🚧 Add 'Why' section near the questions...

 > 🚧 re-order questions by priority...

 > 🚧 understand wholeness of the questions: is it enough for creating a test strategy? Are there redundant questions?

 > 🚧 identify relations with existing TPI next / TMMI / ISO 29119 / ISQTB / Context-driven testing / etc..

### Context

1. Tech stack
    1. What is tech stack?(Languages,DB,etc)
2. Infrastructure
    1. What  3rd parties are in use? 
        1. AWS services, etc
    2. What tools, serving developement, are in use?
        1. CI/CD tools (kubernetes/jenkins/code deploy etc)
        2. VCS (github/bitbucket)
        3. Task management (JIRA...)
3. Release cycles
    1. What are the delivery commitments?
        1. Scope
        2. Urgency
        3. Frequency
        4. Rollout/Rollback policies
    2. How everyone understands:
        1. What new features/fixes/known issues are being released?
        2. Current release is ready?
    3. What an actual delivery item?
        1. updated website? zip?
    4. How success/failure of the release is judged?
5. Team
    1. How manhy people work on the project? Who(devs/devops/qa/analysts/etc) works on it? At which ratio?(is there a lot of qa on devs?,etc)
6. Product-related unique context
    1. Does the product use big data/ai/ml?
    2. Does the product work with sensitive data?
    3. Does the product related to any law/government-controlled areas?
    4. Does the product need to comply with any standards?
7. Customer-related context
    1. Lots of customers?
    2. Types of customers?(for ourselves,for government/etc)
    3. What are the points of interactions with customers? 
        1. via API
        2. via UI
            1.lots of browsers/mobile browsers support? 
        3. via desktop app
        4. via mobiles
8. Is there anything we missed?

### Current status

1. What are the current quality gates? for
    1. Requirement management
        1. Are requirements fixed in written form?
        2. How does the process of maintaining them works?
            1. Writing
            2. Actualizing
        3. Who is responsible for the requirements?
        4. Do we have the way to trace requirements to developers/testers work?
        5. Do we have any automation to help ensuring some quality level of requirements?
        6. What are the functional risks of the requirements?
            1. Frequent changes?
            2. Hard to test?
            3. Incomplete/ often not enough, when it's time to implement?
    2. Testing
        1. Test environment
            1. What environments are used for testing?
            2. How do we make sure that testing on those is valid? (what are our assumptions?)
        2. Test data
            1. Are all the neccessary test data identified?
            2. Are all the neccessary test data accessible?
            3. How does it maintain itself?
            4. Are mocks in use? Why/Why not?
        3. Test state
            1. How easy it is to attain any specific state of the product to test?
        4. Automation
            1. Hierarchy
                1. What types of automation are in place?
                    1. Unit / component /integration / e2e / etc
                    2. API
                        1. Is there any specification for the API? (swagger/...)
                        2. How frequently api changes? Are breaking changes a common thing?
                    3. UI
                        1. What parts of the UI are in check? (screenshots/ e2e flow /component function/ rendering / etc)
                2. Who writes/will write automated checks?
                3. Is there an explicit policy/documentation/guideline on what check and when to write?
                4. Is there an explicit guideline on how to write an automation check?
            2. How fast/easy is to execute automated checks?
            3. How fast/easy is to write automated checks?
            4. What is/isn't being covered by automation? (Explicit assumptions)
        5. Coverage & Traceability
            1. Is there a way to understand, what requirements are covered by testing/automation?
        6. How results/progress of testing is delivered?
        7. Is the decision-making process guided by results of testing?
        8. Is  there an explicit guideline for testing?
    3. Development
        1. Is there an explicit guideline for development?
        2. Is there any metrics in use? (Code coverage)
        3. Is there any automation in place? (unit checks before push / code styles / static checks / etc)
    4. Deployment
        1. Is there an explicit guideline for deployment?
        2. Is there any automation in place to prevent broken implementation to reach enviroment?
    5. Documentation
        1. Entrypoint
            1. Is there a single entry point for newcomers? With links to all relevant data
    6. Task management
        1. How scope of work is identified?
        2. How scope of work is divided into smaller chunks?
        3. How scope of work is prioritized?
        4. Is there Definition of Ready in place?
        6. Is there Definition of Done in place?
        6. Are there quality gates in place?
    7. Feedback gathering
        1. Observability 
            1. What and how feedback is gathered from environments(dev/prod)?
            2. What tools are used to trace back errors to their root causes?
                1. Logging?
                2. Exception tracking?
                3. Tracing/distributed tracing?
2. What is relevancy context?
    1. What is important/not so?
3. What are the known/should be more priotitized risks?
    1. For example, from HTSM (look below)

### HTSM  (Heuristic test strategy model)

1. Capability. Can it perform the required functions?
2. Reliability. Will it work well and resist failure in all required situations?
    1. Robustness: the product continues to function over time without degradation, under reasonable conditions.
    2. Error handling: the product resists failure in the case of errors, is graceful when it fails, and recovers readily.
    3. Data Integrity: the data in the system is protected from loss or corruption.
    4. Safety: the product will not fail in such a way as to harm life or property.
3. Usability. How easy is it for a real user to use the product?
    1. Learnability: the operation of the product can be rapidly mastered by the intended user.
    2. Operability: the product can be operated with minimum effort and fuss.
    3. Accessibility: the product meets relevant accessibility standards and works with O/S accessibility features.
4. Charisma. How appealing is the product?
    1. Aesthetics: the product appeals to the senses.
    2. Uniqueness: the product is new or special in some way.
    3. Necessity: the product possesses the capabilities that users expect from it.
    4. Usefulness: the product solves a problem that matters, and solves it well.
    5. Entrancement: users get hooked, have fun, are fully engaged when using the product.
    6. Image: the product projects the desired impression of quality.
5. Security. How well is the product protected against unauthorized use or intrusion?
    1. Authentication: the ways in which the system verifies that a user is who he says he is.
    2. Authorization: the rights that are granted to authenticated users at varying privilege levels.
    3. Privacy: the ways in which customer or employee data is protected from unauthorized people.
    4. Security holes: the ways in which the system cannot enforce security (e.g. social engineering vulnerabilities)
6. Scalability. How well does the deployment of the product scale up or down?
7. Compatibility. How well does it work with external components & configurations?
    1. Application Compatibility: the product works in conjunction with other software products.
    2. Operating System Compatibility: the product works with a particular operating system.
    3. Hardware Compatibility: the product works with particular hardware components and configurations.
    4. Backward Compatibility: the products works with earlier versions of itself.
    5. Resource Usage: the product doesn’t unnecessarily hog memory, storage, or other system resources.
8. Performance. How speedy and responsive is it?
9. Installability. How easily can it be installed onto its target platform(s)?
    1. System requirements: Does the product recognize if some necessary component is missing or insufficient?
    2. Configuration: What parts of the system are affected by installation? Where are files and resources stored?
    3. Uninstallation: When the product is uninstalled, is it removed cleanly?
    4. Upgrades/patches: Can new modules or versions be added easily? Do they respect the existing configuration?
    5. Administration: Is installation a process that is handled by special personnel, or on a special schedule?
10. Development. How well can we create, test, and modify it?
    1. Supportability: How economical will it be to provide support to users of the product?
    2. Testability: How effectively can the product be tested?
    3. Maintainability: How economical is it to build, fix or enhance the product?
    4. Portability: How economical will it be to port or reuse the technology elsewhere?
    5. Localizability: How economical will it be to adapt the product for other places?

### Future scope-related questions

1. What are the areas you want to improve?
2. What are the areas you want to improve first?


### Resources


1. [Heuristic test strategy model](https://www.developsense.com/resources/htsm.pdf)
