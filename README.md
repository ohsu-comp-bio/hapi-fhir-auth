# hapi-fhir-auth
HAPI FHIR authorization hook for the ACED data commons

- Tracking issue: [ACED-IDP/data_model](https://github.com/ACED-IDP/data_model) — [Add authentication hook for HAPI FHIR service.](https://github.com/ACED-IDP/data_model/issues/34)
- [Reference](https://hapifhir.io/hapi-fhir/docs/security/authorization_interceptor.html)
- [AuthorizationInterceptor JavaDoc](https://hapifhir.io/hapi-fhir/apidocs/hapi-fhir-server/ca/uhn/fhir/rest/server/interceptor/auth/AuthorizationInterceptor.html)
- [AuthorizationInterceptor Source](https://github.com/hapifhir/hapi-fhir/blob/master/hapi-fhir-server/src/main/java/ca/uhn/fhir/rest/server/interceptor/auth/AuthorizationInterceptor.java)

## Development

This project uses [Maven](https://maven.apache.org/) as the build system. To install Maven on macOS run:

```sh
brew install mvn
```

To compile, build, and test the project run:

```
mvn verify
```

### Maven Phases

Each of the following Maven commands would be run as `mvn <PHASE>` (e.g. `mvn validate`, from *[Introduction to the Build Lifecycle](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html)*):

- `validate` - validate the project is correct and all necessary information is available
- `compile` - compile the source code of the project
- `test` - test the compiled source code using a suitable unit testing framework. These tests should not require the code be packaged or deployed
- `package` - take the compiled code and package it in its distributable format, such as a JAR.
- `verify` - run any checks on results of integration tests to ensure quality criteria are met
- `install` - install the package into the local repository, for use as a dependency in other projects locally
- `deploy` - done in the build environment, copies the final package to the remote repository for sharing with other developers and projects.
