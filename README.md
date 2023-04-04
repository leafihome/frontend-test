# Leafi Home Front end programming test

Choose your favorite frontend frontend framework (React, Vue.js, Angular etc) to build multiple pages website contains the following Functionalities. All the APIs are pre-built and availble in the API test server.

- a page to create a new company `/companies/create`
- A page to show a list of companies `/companies`
- A page to show the details/full record of an existing company `/companies/{id}`
- A page to create a new employee, associating them to an existing company `/employees/create`
- a page to show a list of people who work at a given company `/companies/{id}`

## Bonus Functionality
- Edit an existing company's record `/companies/{id}`
- Be able to delete an employee record
- Using State Management Libraries like Redux

## API test server

### Available Scripts
We have two utility methods to create some test data for you, accessible via HTTP GET: 
- [Create test companies](http://localhost:3001/swagger/index.html#!/Companies/get_importCompanies)
- [Import people for a given company](http://localhost:3001/swagger/#!/People/get_importPeopleForCompany_companyId)


### Environment Setup
node 14 & MongoDB Community Server 5.0.

#### Using NVM to install node 14 https://github.com/nvm-sh/nvm

#### How to install MongoDB Community Server 5.0. On macOS
```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor #fix all issues
brew update
brew tap mongodb/brew
brew install mongodb-community@5.0
brew services start mongodb/brew/mongodb-community@5.0
echo 'export PATH="/usr/local/opt/mongodb-community@5.0/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

#### On Windows

- Download [node version 14](https://nodejs.org/en/blog/release/v14.17.3/) 
- Download MongoDB download [link](https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.13-rc0-signed.msi)
- Follow this instruction [Install MongoDB Community Edition on Windows](https://www.mongodb.com/docs/v5.0/tutorial/install-mongodb-on-windows/)

#### Create a MongoDb data directory if folder doesn't exist

```
mkdir -p ./data/db
```

#### To install all dependencies
`npm install`

#### Runs the server

Make sure mongoDB@5.0 is running before start the server

`npm run server`

### API Doc
http://localhost:3001/swagger


