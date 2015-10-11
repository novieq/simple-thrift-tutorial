1. Create a .thrift file
2. thrift --gen java multiplication.thrift
3. thrift --gen py multiplication.thrift
4. mvn idea:idea 
5. Create a service handler, server and client in src folder. Copy the generated service code to the src folder. Compile the code using : mvn package : This will create a jar file in target
6. Run the client : java -cp ".:/Users/meramac/workspace/thrift-0.9.2/lib/java/build/libthrift-0.9.2.jar:/Users/meramac/Downloads/slf4j-1.7.12/slf4j-api-1.7.12.jar:target/multiplicationService-0.0.1-SNAPSHOT.jar" MultiplicationClient
7. Run the server : java -cp ".:/Users/meramac/workspace/thrift-0.9.2/lib/java/build/libthrift-0.9.2.jar:/Users/meramac/Downloads/slf4j-1.7.12/slf4j-api-1.7.12.jar:target/multiplicationService-0.0.1-SNAPSHOT.jar" MultiplicationServer
