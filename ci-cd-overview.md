CI/CD Overview
==============

**Why**

**Continuous Integration (CI)**

-   The idea is to integrate code with the rest of your team as often as possible.
-   Reduces merge conflicts/deployment risk.
-   The scope of changes must be small so conflicts are easier to fix.

**Continuous Delivery (CD)**

-   Encourages the M.V.P discipline, releasing small focused features often.
-   Test your new ideas in production with real customers.
-   Ensures you build features people want.

**Overview**

Continuous Delivery is the practice of creating a repeatable, reliable process for releasing software.

CD is a key enabler for delivering real business value as quickly and efficiently as possible.

-   New ideas can be turned into new features and quickly delivered to end users.
-   Promotes fast feed-back across the development lifecycle (dev -> business ops -> end users).
-   Promotes the warranty of your application -- bugs are quickly discovered, fixed and deployed (it's pointless if your site keeps crashing or your software is buggy).

**How**

**Automation**

-   Workflow automation encourages CD.
-   We need a set of tools to enable this automation.
-   Allows you to move fast with repeatable and consistent results.
-   Should aim to have a "one-click" deployability for any software change.

**People**

-   Must decide on a git strategy for integrating code.
-   Must decide on code review strategies.

**Test**

-   Quantitatively "measurement" of each release.
-   The goal is production-ready releases asap.

**Local Flow**

CI is not a "silver bullet". The team must be on board for this to be successful.

The team must adopt a strategy for integrating code. This usually involves

-   Pulling latest code from master.
-   Create code and tests, run locally.
-   Get the latest code from the master, merge, resolve a conflict.
-   Run the test suite, ensure passes locally.
-   Push to the remote branch (feature) and do Pull Request.
-   Discuss concerns any team members may have. Incorporate feedback.
-   Integrate with upstream master again.
-   Once merged, an automated build will be kicked off (hurray!).

**Technologies**

-   Jenkins/Circle CI
    -   The build server.
-   Github
    -   Webhook that triggers the build on the build server.
-   Docker
    -   Speed (quick to build new images/run tests).
    -   Portable (code and environment are packaged together meaning the environmental dependencies are always satisfied).
    -   Simplifies your production infrastructure (all you need installed is Docker!).
    -   Automation (automatically build images from Dockerfiles).

**Workflow Stages**

**Test**

-   Unit and Integration tests.
-   Wrap test runners in docker to use pre-defined environment for tests ensuring portability/consistency/repeatability.

**Build**

-   Build application artifacts that are a true representation of a successful application.
-   Create deployable artifacts such as Jars/war, pre-compiled assets.

**Release**

-   Create a deployable release artifact as a docker release image.
-   Includes minimal runtime environment.
-   Installs application artifacts from the Build stage.
-   Tag and Publish image to a registry such as a docker hub.

**Deploy**

-   Deploy image to an environment: Production, QA, Staging.
-   Aim to continuously deploy to at least one environment so you're continuously verifying you can successfully deploy your releases.
