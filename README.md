# Leafihome Front end programming test

## Expected functionality:
- A page to show a list of companies `/companies`
- A page to show the details/full record of an existing company `/companies/id`
- a page to create a new company `/companies/create`
- a page to show a list of people who work at a given company `/companies/id/people`
- A page to show the details for a specific person `/people/id`
- A page to create a new person, associating them to an existing company `/people/create`

## Bonus functionality
- Edit an existing company's record `/companies/id`
- Edit a person's record `/people/id`
- Delete a person record `/people/id`
- Make the site responsive
- Using State Management Libraries like Redux

## API test server

### Available Scripts
We have two utility methods to create some test data for you, accessible via HTTP GET: 
- [Create test companies](http://localhost:3001/swagger/index.html#!/Companies/get_importCompanies)
- [Import people for a given company](http://localhost:3001/swagger/#!/People/get_importPeopleForCompany_companyId)

#### To install all dependencies
`npm install`

#### Runs the server
`npm start`

### API Doc
http://localhost:3001/swagger

### Pre server reqs
Install brew, node, npm & mongo. On OSX the commands below should work.

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor #fix all issues
brew update
brew install node
brew tap mongodb/brew
brew install mongodb-community
```

Setup MongoDb data directory if folder doesn't exist
```
mkdir -p data/db
```

#### Windows users run these two commands
```
npm run mongo
npm run server
```
