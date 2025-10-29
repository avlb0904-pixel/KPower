KPower - Build-ready project with GitHub Actions
================================================

This repository is prepared to be built by GitHub Actions on push to 'main' or by manual workflow dispatch.
It will generate the Gradle wrapper on the runner (so you do not need to include gradle-wrapper.jar here).

How to use:
1. Create a new GitHub repository and push the contents of this project to it (main branch).
2. The workflow at .github/workflows/build.yml will run on push and build the mod.
3. After the workflow completes, download the artifact (kpower-jar) from the workflow run, or create a release to attach the artifact automatically.
4. Alternatively, build locally by running:
   - Install JDK 17
   - Run: gradle wrapper --gradle-version 8.4
   - Then: ./gradlew build

Mod details:
- mod id: kpower
- version: 1.0.0
- target Minecraft: 1.21.1
