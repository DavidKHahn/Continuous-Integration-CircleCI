## Continuous-Integration Guidelines

**CI Guidelines:**

- Should be implemented at the beginning of a project and then expand to continuous delivery and continous deployment.
- Important to make pull requests daily and merges to master daily otherwise expose to having too many conflicts and easier to debug.

- **Helpful Tools:** Tests, Typescript Linting, Circle CI, Travis CI, Jenkins (similar to CircleCI but with flexibility to manage server), Bamboo, Codeship, Prettier

**Prettier:**
 - https://prettier.io/docs/en/precommit.html (Precommit Hook setup)
 - Setting precommit hook in package.json helps detects any formatting of code which needs to be "prettified"
 - ``npm install --save-dev --save-exact prettier`` or globally ``npm install --global prettier``
 - ``yarn add pretty-quick husky --dev`` install pretty-quick package to ensure entire file formatting on your changed/staged files.
 - ``"pre-commit": "pretty-quick --staged"`` add this inside package.json under 'scripts'


 

**Useful Links:**

- https://circleci.com/docs/2.0/getting-started/#section=getting-started (Circle CI 2.0 Documentation + Setup config.yml)
