Quick Gradle Enterprise & `frontend-maven-plugin` Example
=========================================================

This example project caches the output from the `frontend-maven-plugin`. 
The npm build creates files in `target/npm-build`, you can verify built results are cached by inspecting the `target/npm-build/result.txt` file

To run this example:

1. Update the server URL in `.mvn/gradle-enterprise.xml`
2. Run: `./mvnw clean verify` to populate the local cache
3. Run: `./mvnw clean verify` again and verify cache hits.
