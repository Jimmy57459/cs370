# Test Plan

**Author**: Team4

## 1. Testing Strategy

### 1.1 Overall strategy

Following strategies shall be followed for testing.

- Unit Testing
- Integration Testing (Manually): Android Activities for the functionality of the UI components and they displays the correct information to the UI.
- Regression Testing: Most of the test cases which are related to the change.
- System Testing

QA / Application tester(s) shall perform system and regression testing. However, Software Engineer / programmer shall write Unit tests at application level.

### 1.2 Test Selection

Black-box testing shall be used to test the test cases. However the test cases shall be tested based on condition testing.

### 1.3 Adequacy Criterion

Tests shall be performed on functional requirements. It shall be based on test pass/fail status.

### 1.4 Bug Tracking

Team shall use GIT Issue Tracker for bug tracking.

### 1.5 Technology

Manual testing shall be performed for UI/App testing. Unit test(s) shall be written to test core functionality of an application at application level. Mockito framework was used to mock some objects to use in JUnit tests.

## 2. Test Cases

Following is a list of initial test cases which can be performed to test the core functionality of a product (GroceryListManager - GML).

| TC-01           | Add List                                                                        |
| --------------- | ------------------------------------------------------------------------------- |
| Description     | User should be able to create a list.                                           |
| Pre-Condition   | User at initial interface                                                       |
| Steps           | 1.The user press the floating action button. 2.Enter the name and press confirm |
| Expected Result | One empty list is created.                                                      |
| Test Status     | Pass                                                                            |

| TC-02           | Select List                                                                         |
| --------------- | ----------------------------------------------------------------------------------- |
| Description     | User should be able to select a list.                                               |
| Pre-Condition   | At least one list exists.                                                           |
| Steps           | 1.The user opens the grocery list application. 2.The user selects an existing list. |
| Expected Result | A list is selected.                                                                 |
| Test Status     | Pass                                                                                |

| TC-03           | Rename List                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Description     | User should be able to rename the list.                                                                                   |
| Pre-Condition   | At least one list exists.                                                                                                 |
| Steps           | 1.The user selects an existing list. 2.Open the more options menu. 3. Select rename and type in a new name for this list. |
| Expected Result | Selected list is renamed.                                                                                                 |
| Test Status     | Pass                                                                                                                      |

| TC-04           | Remove List                                                                                                                                                                                                                                                                                                    |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Description     | User should be able to remove the list.                                                                                                                                                                                                                                                                        |
| Pre-Condition   | At least one list exists.                                                                                                                                                                                                                                                                                      |
| Steps           | 1. Press the kebab menu button(three vertical dots icon) on the upper right corner. 2. Select edit button to enter edit mode. 3. When the small trash can icon appears, click the icon corresponding to the list you want to delete. 4. Select yes. 5. Press the menu button and select done to exit edit mode |
| Expected Result | Selected list is removed.                                                                                                                                                                                                                                                                                      |
| Test Status     | Pass                                                                                                                                                                                                                                                                                                           |

| TC-05           | Add Item                                                                                                                                                                                                                                                     |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Description     | User should be able to add item to the list                                                                                                                                                                                                                  |
| Pre-Condition   | A list must be selected.                                                                                                                                                                                                                                     |
| Steps           | 1. The user selects an existing list. 2. Press the floating action button in the lower right corner. 3. Search item, select it, set up the quantity you need, and press confirm. 4. Return to the previous interface. You'll find the item is already there. |
| Expected Result | Item is added to this list.                                                                                                                                                                                                                                  |
| Test Status     | Pass.                                                                                                                                                                                                                                                        |

| TC-06           | Search Item                                                                                                                                                                                                              |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Description     | User should be able to search item in a product database                                                                                                                                                                 |
| Pre-Condition   | The user want to search new item in local database                                                                                                                                                                       |
| Steps           | 1. The user selects an existing list. 2. Press the floating action button in the lower right corner. 3. Type in the keyword in the search bar and press search. 4. The user can search the item by Itemname or Itemtype. |
| Expected Result | Show searching result.                                                                                                                                                                                                   |
| Test Status     | Pass.                                                                                                                                                                                                                    |

| TC-07           | Create Item                                                                             |
| --------------- | --------------------------------------------------------------------------------------- |
| Description     | User should be able to add a new item to local database.                                |
| Pre-Condition   | After searching item in database, no match can be found.                                |
| Steps           | 1.The user searchs item in database. 2. Match is not found, add a new item to Database. |
| Expected Result | New item is added to database.                                                          |
| Test Status     | Pass.                                                                                   |

| TC-08           | Check Item                                                                     |
| --------------- | ------------------------------------------------------------------------------ |
| Description     | User should be able to check/uncheck item(s) in a list without deleting them.  |
| Pre-Condition   | A list must be selected.                                                       |
| Steps           | 1.The user selects one list. 2.The user clicks the check button. 3.Select item |
| Expected Result | Selected items are marked as checked.                                          |
| Test Status     | Pass                                                                           |

| TC-09           | Set Item Quantity                                                                                              |
| --------------- | -------------------------------------------------------------------------------------------------------------- |
| Description     | User should be able to set quantity for item(s) in a selected list.                                            |
| Pre-Condition   | A list must be selected. An item must be selected.                                                             |
| Steps           | 1.The user selects a list. 2. Press the item that need to be modified. 3. Enter the quantity and press confirm |
| Expected Result | Quantity is set to a selected item.                                                                            |
| Test Status     | Pass                                                                                                           |

| TC-10           | Delete Item                                                                                |
| --------------- | ------------------------------------------------------------------------------------------ |
| Description     | User should be able to delete item in a selected list.                                     |
| Pre-Condition   | A list must be selected. One item must be selected.                                        |
| Steps           | 1.The user selects a list. 2. Long press the item and select yes in the pop-up dialog box. |
| Expected Result | The user deleted a selected item.                                                          |
| Test Status     | Pass                                                                                       |
