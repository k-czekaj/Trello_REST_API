# COLT 01/2023 project: Trello REST API testing with Postman

## About project

COLT is charitable 4-week collaborative testing project organised by [Cherry IT](http://cherry-it.pl/podsumowanie-colt-1-2023/). The result of the project is a collection of Trello REST API tests. Tests were performed in the Postman tool.

## Test scope based on [Trello API documentation](https://developer.atlassian.com/cloud/trello/rest/api-group-actions/)

- Board
  - Create a Board
  - Get a Board
  - Update a Board
- List
  - Create a List on a Board
  - Get Lists on Board
  - Update a List
  - Archieve all Cards in List
- Card
  - Create a new Card
  - Get a Card on a Board
  - Update a Card
- Checklist
  - Create Checklist on a Board
  - Get Checklists on a Board
  - Create Checkitem on Checklist
- Delete
  - Delete a Checklist on a Card
  - Delete a Card 
  - Delete a Board

## Getting started

### List of steps needed to run collection and tests

1️⃣ Postman installation

:two: Creating a Trello account

:three: Trello authentication

:four: Importing a file into Postman

:five: Creating environment variables in Postman

:six: Run collection and testing

#### Postman installation

1. Go to the [Postman website](https://www.postman.com/downloads/) and click the orange button with name of your operating system.
2. Download the installation file, then run the installer and follow the instructions that appear.
3. Postman is ready to use.
    
#### Creating a Trello account

1. Go to the [Trello website](https://trello.com/) and click the blue button with text "Get Trello for free".
2. Create a Trello account by following the instructions that apper.
3. Your Trello account is ready to use.

#### Trello authentication

1. Log in to your Trello account.
2. Go to the [Trello developer API key generation page](https://trello.com/app-key).
3. Click on the "Go to the Power-Up Admin Portal", then click "Create New Key" button and enter the required details.
4. Your API key will be displayed on the page. Copy and save it for later to use in Postman.
5. Next, click on the Token link that under the key you just generated.
6. Allow application to access your Trello account.
7. Your token will be displayed on the page. Copy and save it for later to use in Postman.

#### Importing a file into Postman

1. Go to [my Postman collection file](https://github.com/k-czekaj/Trello_REST_API/blob/main/Trello%20-%20REST%20API.postman_collection.json).
2. Click on the three dots icon in the top right corner and click Download.
3. Run Postman and click on "Import" button in the top left corner.
4. Drag and drop the downloaded file from the Download folder into the "Import" window.
5. The collection will appear in Postman, ready for use.   

#### Creating environment variables in Postman

1. Click on the "Environment" dropdown in the top left corner in Postman.
2. Click on the "New" button to create a new environment and choose "Environment" icon.
3. Give your environment a name.
4. Create a "key", "token" and "baseURL" variable. You should enter the value "https://api.trello.com/1/" into the "baseURL" variable and the value of your key and token in the "key" and "token" variable. **For collections from this repository, the API key variable is named {{key}}, the token variable is named {{token}} and the URL variable is named {{baseURL}}**.
5. Click "Save" button to save the environment.
6. Click on the "Environment" dropdown in the top left corner and select the environment you just created.

#### Run collection and testing

1. Click on the "Collections" icon in Postman.
2. From the list of collections, select the one named "Trello - REST API" and click on the icon with three dots that appears when you hover over the collection name.
3. Select "Run collection" from the list.
4. Click one the orange button "Run Trello - REST API".

If the view in your Postman looks like the one on the screenshot below, then you have successfully completed all the steps and launched my collection. Congratulations!

![2023-05-21_17h00_40](https://github.com/k-czekaj/Trello_REST_API/assets/122294284/b99d7fa1-1199-4846-a95e-a2473926df8d)


