# BitcoinPriceService

#### To build BitcoinPriceService type:

```
mvn clean package|install
```
#### To run BitcoinPriceService server type (from target directory):
```
java -jar bitcoin-price-service-0.0.1-SNAPSHOT.jar
```
or
```
mvn spring-boot:run
```

#### Integration testing

To run service in test mode type:
```
java -Dspring.profiles.active=test -jar bitcoin-price-service-0.0.1-SNAPSHOT.jar
```
In test mode, internet connection is not needed for server to get current prices and notify users. Server use hardcoded price value that is used to send notifications to clients.


##### ``BitcoinServiceClient``
Project contain ``BitcoinServiceClient`` class which is the simple CLI implementation of the server client. It enables the user to set any number of price alerts for different currency pairs, as well as remove them. Instruction with examples are printed after client start.
