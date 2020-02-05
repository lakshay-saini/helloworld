mvn clean org.jacoco:jacoco-maven-plugin:prepare-agent test --fail-at-end -DskipTests=false -am;

mvn sonar:sonar --batch-mode --errors " +
"-pl ${context.env.TEST_MODULES} -am " +
"-Dsonar.projectKey=${Constants.SONARCLOUD_PROJECT_KEY} " +
"-Dsonar.organization=${Constants.SONARCLOUD_ORGANISATION} " +
"-Dsonar.verbose=true " +
"-Dsonar.host.url=${Constants.SONARCLOUD_URL} " +
"-Dsonar.login=${context.env.SONARCLOUD_TOKEN} " +
"-Dsonar.pullrequest.branch=${context.env.BRANCH_NAME} " +
"-Dsonar.pullrequest.base=${Constants.RELEASES_BRANCH} " +
"-Dsonar.pullrequest.key=${context.env.CHANGE_ID}
