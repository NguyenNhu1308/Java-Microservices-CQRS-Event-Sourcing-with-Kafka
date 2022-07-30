# Java-Microservices-CQRS-Event-Sourcing-with-Kafka

# Open Bank Account

```sh
curl --location --request POST 'http://localhost:5001/api/v1/openBankAccount' \
--header 'Content-Type: application/json' \
--data-raw '{
    "accountHolder": "john Doe",
    "accountType": "SAVINGS",
    "openingBalance": 50.0
}'
```

Response:

```
{
    "message": "Bank account creation request completed successfully!",
    "id": "0266c886-8267-4e9c-96ed-3dfb66aac4c4"
}
```

<img width="897" alt="Screenshot 2022-07-30 at 2 41 30 PM" src="https://user-images.githubusercontent.com/54174687/181903734-e96573db-9583-42ac-9aad-f2df0cea11ec.png">
<img width="1045" alt="Screenshot 2022-07-30 at 2 41 40 PM" src="https://user-images.githubusercontent.com/54174687/181903748-f37bd3f7-c0f8-4710-a8a0-57ad6beb68ee.png">
<img width="832" alt="Screenshot 2022-07-30 at 2 41 52 PM" src="https://user-images.githubusercontent.com/54174687/181903755-2b129749-da4f-4281-a349-623efbf0e36d.png">
<img width="1196" alt="Screenshot 2022-07-30 at 2 44 42 PM" src="https://user-images.githubusercontent.com/54174687/181903850-a830de51-fbfe-45b7-a55b-e6574c552ff0.png">

-----

# Depost Funds

```sh
curl --location --request PUT 'http://localhost:5001/api/v1/depositFunds/0266c886-8267-4e9c-96ed-3dfb66aac4c4' \
--header 'Content-Type: application/json' \
--data-raw '{
    "amount": 150.0
}'
```

Response:

```json
{
    "message": "Deposit funds request completed successfully!"
}
```
<img width="1031" alt="Screenshot 2022-07-30 at 2 47 43 PM" src="https://user-images.githubusercontent.com/54174687/181904049-776f72f8-1773-46b8-a4ef-b19f6aafb84a.png">
<img width="829" alt="Screenshot 2022-07-30 at 2 47 54 PM" src="https://user-images.githubusercontent.com/54174687/181904054-73de81fc-e958-44ad-a32d-faa8dd121403.png">
<img width="1189" alt="Screenshot 2022-07-30 at 2 49 04 PM" src="https://user-images.githubusercontent.com/54174687/181904055-554f2756-14e8-4ea7-9bdd-3078e13cf400.png">

<img width="903" alt="Screenshot 2022-07-30 at 2 47 25 PM" src="https://user-images.githubusercontent.com/54174687/181904044-e152a4b6-f3c3-4631-8f3a-f883cc276769.png">

