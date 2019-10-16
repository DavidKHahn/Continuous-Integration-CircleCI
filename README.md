## Continuous-Integration

<p align="center">
<img width="700" alt="continuous-integration-flow" src="https://user-images.githubusercontent.com/34965292/66897079-160e6900-efab-11e9-840b-7bb7f4379208.png">
</p>

**CI Guidelines:**

- CI should be implemented at the beginning of a project and then expand to continuous delivery or continous deployment.
- Code PRs should be run daily, as well as merging to master decreasing exposure to conflicts and bugs.  
- Builds, steps, test steps, linting and other checks can run more successfully leading to code reviews and merging new features.
- Testers can test software and manually deploy to production for actual usage in the real world or automated without testers as well.



- **Helpful Tools:** Tests, Typescript Linting, Circle CI, Travis CI, Jenkins (similar to CircleCI but with flexibility to manage server), Bamboo, Codeship, Prettier.

**Prettier:**
 - https://prettier.io/docs/en/precommit.html (Precommit Hook setup)
 - Setting precommit hook in package.json helps detects any formatting of code which needs to be "prettified"
 - ``npm install --save-dev --save-exact prettier`` or globally ``npm install --global prettier``
 - ``yarn add pretty-quick husky --dev`` install pretty-quick package to ensure entire file formatting on your changed/staged files.
 - ``"pre-commit": "pretty-quick --staged"`` add this inside package.json under 'scripts'


 

**Useful Links:**

- https://circleci.com/docs/2.0/getting-started/#section=getting-started (Circle CI 2.0 Documentation + Setup config.yml)
- https://www.npmjs.com/package/webpack-bundle-analyzer (Visualize size of webpack output files with an interactive zoomable treemap.)
