# RULES

## PROMPT LIBRARY

We have various prompts that can be used for workflows.  The prompts are grouped into function and stored in separate files in the .ai/PROMPTS/ directory.

### Prompt Library Rules

1. If you are asked to do a task that relates to prompts in the list, you can ask for those prompts to be added to the context.  Example: "I want to test this model" means you should load in the unit testing prompts.
2. After the prompts are loaded, if there are multiple possible prompts to use suggest one that makes sense.

### Prompt Library List

* .ai/PROMPTS/PLAN.yml - our comprehensive feature planning workflow that includes PRD generation, task decomposition, architecture decisions, risk assessment, and testing strategy. Use this for systematic planning of any feature.
* .ai/PROMPTS/UNIT_TESTING_FULL.yml - Full version of "Think First" test generation work flow.
* .ai/PROMPTS/UNIT_TESTING_QUICK.yml - Quick version of "Think First" test generation work flow.

## Coding

Follow these rules when writing code in this project:

* Use 4 spaces for indentation
* Use camel case for variable and method names
* Use snake case for file names
* Use comments to explain your code
* Do not use the `any` type in typescript code
* Alphabetize imports and object members
* Before writing any code list out any optimizations that can be done

## Tests

### Adding Tests

Adding tests in this project should be worked on using the Think First workflow.  Prompts for that are in the prompt library.  If they aren't added to the context please add them.

### Testing Conventions

* This is a React project using typescript and jest for testing.
* Test files are located in a “****tests****” folder next to the code being tested.  Example.  Tests for “MyExampleComponent.tsx” would have tests located in a file at “****tests****/MyExampleComponent.test.tsx”.
* Tests should follow the Arrange, Act, Assert pattern.
* Tests should be grouped into `describe` sections for common functionality.
