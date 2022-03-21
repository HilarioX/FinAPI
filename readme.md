# FinAPI - My first step on NodeJS :grin:

This folder contains all the necessary files and instructions to launch and use a basic NodeJS API, that works with endpoints.

## Try it out

**How to download?**

So, we have 2 ways of downloading this repo.

- By cloning this GitHub repository by GitBash:

  ```gitbash 
  git clone git@github.com:HilarioX/FinAPI.git
  ```

- Downloading the file by clicking code, then Download zip

**Install the packages**

Download and install the API dependencies by the following commands:

```terminal
yarn install 
yarn add express
yarn add nodemon -D
```

**Running the project**

If you wanna run the project for development, so make sure you runnig this command:

```terminal
yarn dev
```

To run normaly you can use just the ``` yarn start``` comand



## Using the endpoints

### Postman or Insomnia:

- #### Creating account (post)

  /account

  - ##### Header

    - Content -type : application/json

  - ##### Body

    - ``` json 
      {
          "cpf": "insert your cpf here", 
          "name" : "insert your name here"
      }
      ```

- #### Statement (get)

  /statement

  - ##### Header

    - cpf : the value of you put in the `Creating Accont (post)`

- #### Deposit (post)

  /deposit

  - ##### Header

    - Content -type : application/json
    - cpf : the value of you put in the `Creating Accont (post)`

  - ##### Body

    - ``` json 
      {
      	"description": "some description",
      	"amount": some value here
      }
      ```

- #### Withdraw (post)

  /withdraw

  - ##### Header

    - Content -type : application/json
    - cpf : the value of you put in the `Creating Accont (post)`

  - ##### Body

    - ``` json 
      {
      	"amount": some value here
      }
      ```

- #### Statement by date (get)

  /statement/

  - ##### Header

    - cpf : the value of you put in the `Creating Accont (post)`

  - ##### Query

    - date : yyyy-mm-dd

- #### Update account (put)

  /account

  - ##### Header

    - Content -type : application/json
    - cpf : the value of you put in the `Creating Accont (post)`

  - ##### Body

    - ``` json 
      {
      	"name": "insert here the new name"
      }
      ```

- #### Account (get)

  /account

  - ##### Header

    - cpf : the value of you put in the `Creating Accont (post)`

- #### Delete user (delete)

  /account

  - ##### Header

    - cpf : the value of you put in the `Creating Accont (post)`

- #### Balance (get)

  /balance

  - ##### Header

    - cpf : the value of you put in the `Creating Accont (post)`