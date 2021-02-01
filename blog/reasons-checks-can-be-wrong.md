Reasons, that automated checks can be wrong[wip]

**All checks**
2. Checks that enforces / checks wrong expected behavior
3. Checks that doesn't indicate reasonable information
	1. e.g. Something that will almost always work or if breaks, then everything will break and the same behavior could be covered by different type of check

**Failed checks**
1. Wrong check's logic
2. Problem in environment
	1. Environment variables
	2. Environment setup
	3. Execution's environment (all necessary requirements had changed or hadn't been met)

**More precisely**
1. Problem in preconditions
	1. Not all test data prepared?
	2. Not all the services set up and running?
2. Problem in action
3. Problem in assertions
	1. metric that check use is flaky or wrong(by business logic or implementation)
