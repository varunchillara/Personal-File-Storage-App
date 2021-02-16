__clean:
	./mvnw clean -f pom.xml

package: __clean
	./mvnw package -f pom.xml

#Requires chrome to run selenium integration tests
run-selenium-tests:
	./mvnw test -f pom.xml

run-local:
	./mvnw spring-boot:run