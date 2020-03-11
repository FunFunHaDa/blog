# [오류] Intellij, Gradle, Spring Boot 관련 오류 모음

```
FAILURE: Build failed with an exception.
* What went wrong:
Execution failed for task ':test'.
> No tests found for given includes: [......](filter.includeTestsMatching)
```
### test 대상 코드 경로를 못 찾아서 발생하는 오류다, [......]부분이 경로가 맞는지 확인해야 한다.