# First Part: Test Design
#### - List of bullet points with prioritization
1. User can download & install application successfully -> Critical
2. Application is opened successfully without any error msgs -> Critical
3. Application UI is correct [Header, Application logo] --> High
4. User can Add/Edit/Delete an account -> High
5. User can Add/Edit/Delete an income -> High
6. User can Add/Edit/Delete an expense -> High
7. User can't add new category for income/expense unless he subscribe to Pro -> High
8. User can Add an expense by tapping on any category -> High
9. User can change app language -> Medium
10. User can change currency -> Medium
11. User can search using text or value and results are displayed -> Medium
12. User can't leave value empty or enter negative values in adding income/expense -> Medium
13. User swipe up to see list of incomes & expenses -> Medium
14. User is able to make transfers between different accounts & others -> Medium
15. Right side menu should display Categories, Accounts, Currencies, Settings -> Medium
16. Long tap on any category icon should display its name in circle center -> Medium
17. User should be able to merge accounts -> Medium
18. Left side menu should display dropdown list with accounts, time to view actions in, Choose date button -> Medium
19. Pro features screen should appear everytime user tries to use any pro feature -> Medium
20. All Application text should be with correct spelling -> Low


#### - Example of Detailed Test Cases
1.
- Summary: User can Add an account
- Steps: 
  1. Open Monefy app
  2. Tap on 3 dots on top right
  3. Tap on Accounts
  4. Tap + button beside Add
  5. Type Name of your account
  6. Enter initial account balance
  7. Fill other information according to your preferences
  8. Tap ADD button on top right
- Expected: Account is added successfully and user can view account by navigating to accounts section
- Actual:
- Priority: High

2.
- Summary: User can change Application language
- Steps:
  1. Open Monefy app
  2. Tap on 3 dots on top right
  3. Tap on Settings
  4. Under General Settings section -> Tap on Language
  5. Choose other language than default
  6. Tap OK button
- Expected: Application language should be changed to the chosen language
- Actual:
- Priority: Medium


--------------------------------------------------------------------------------------------------
# Second Part: Bug Reporting


#### Bug 1
|    Title    |    Reproducible Steps    | Attachments | Affected Devices | Network | Severity | Priority | Impact |
| ----------- | ------------------------ | ----------- | -----------------| ------- | -------- | -------- | ------ |
| Application language is not changed correctly | 1. Open Monefy app | https://drive.google.com/file/d/1wSkqbZFs_qorl25ny6Fqcp8SPzILG7bs/view | Samsung Galaxy A71و Android 11 | Wi-Fi | Low | Medium | User will be expecting all text in application to be translated to his selected language |
|  | 2. Tap on 3 dots on top right |
|  | 3. Tap on Settings |
|  | 4. Under General Settings section -> Tap on Language |
|  | 5. Choose other language than default |
|  | 6. Tap OK button |
|  | 7. Check language of categories & menus | 

#### Bug 2
| Title | Reproducible Steps | Attachments | Affected Devices | Network | Severity | Priority | Impact |
| ----- | ------------------ | ----------- | -----------------| ------- | -------- | -------- | ------ |
| User can't change currency from account but can change from settings | 1. Open Monefy app | https://drive.google.com/file/d/1wVVLLsDw23vhMLIRx0aPDV7HalpmjBcW/view | Samsung Galaxy A71و Android 11 | Wi-Fi | Low | Medium | If it is a premium feature so users are enjoying it for free |
|  | 2. Tap on 3 dots on top right |
|  | 3. Tap on Settings | 
|  | 4. Under General Settings section -> Tap on Currency |
|  | 5. Choose other currency than default |
|  | 6. Tap on 3 dots on top right |
|  | 7. Tap on Currencies |
|  | 8. Check behavior |

#### Bug 3
| Title | Reproducible Steps | Attachments | Affected Devices | Network | Severity | Priority | Impact |
| ----- | ------------------ | ----------- | -----------------| ------- | -------- | -------- | ------ |
| Categories on chart get mixed and lines cross out | 1. Open Monefy app | https://drive.google.com/file/d/1wlO51uaYf1zbBxe4lzPyC0z7AmTZ6O-F/view | Samsung Galaxy A71و Android 11 | Wi-Fi | Medium | Medium | Chart look is not good and lines are crossed together |
|  | 2. Tap on income and add $5000 in Salary |
|  | 3. Add $100 in all categories |
|  | 4. Add extra $200 in one category (Ex: Car) |
|  | 5. Check chart behavior |

#### Bug 4
| Title | Reproducible Steps | Attachments | Affected Devices | Network | Severity | Priority | Impact |
| ----- | ------------------ | ----------- | -----------------| ------- | -------- | -------- | ------ |
| One category gets un-attached from the chart | 1. Open Monefy app | https://drive.google.com/file/d/1wzoz25ZoKLoOKn_tStXkIltyad2mfDbj/view | Samsung Galaxy A71و Android 11 | Wi-Fi | Medium | Medium | Chart look is not good and one category gets un attached from chart for no reason |
|  | 2. Tap on income and add $5000 in Salary |
|  | 3. Add $100 in all categories |
|  | 4. Add extra $200 in one category (Ex: Car) |
|  | 5. Add extra $200 in another category (Ex: Home) |
|  | 6. Check chart behavior |

#### Bug 5
| Title | Reproducible Steps | Attachments | Affected Devices | Network | Severity | Priority | Impact |
| ----- | ------------------ | ----------- | -----------------| ------- | -------- | -------- | ------ |
| User can add expense to a category while it is disabled | 1. Open Monefy app | https://drive.google.com/file/d/1x51A52LMYssRhehW_DGgh8Nr4jKA7LDP/view | Samsung Galaxy A71و Android 11 | Wi-Fi | Medium | High | User can add to a disabled category which will affect satisfaction of user
|  | 2. Tap on income and add $1000 in Salary |
|  | 3. Tap on any category and add $100 as an expense |
|  | 4. Tap on 3 dots on top right to open side menu |
|  | 5. Tap on categories |
|  | 6. Tap on the category you added in $100 | 
|  | 7. Tap 3 dots on top right |
|  | 8. Uncheck Enabled checkbox |
|  | 9. Go back to chart |
|  | 10. Tap on sports icon on chart and add $100 |

#### Bug 6
| Title | Reproducible Steps | Attachments | Affected Devices | Network | Severity | Priority | Impact |
| ----- | ------------------ | ----------- | -----------------| ------- | -------- | -------- | ------ |
| Chart fails when user add expenses in all 15 categories | 1. Open Monefy app | https://drive.google.com/file/d/1xBOloUf1IcrOHfJwJAuoQVK1zOI1OOoD/view?usp=sharing | Samsung Galaxy A71و Android 11 | Wi-Fi | Medium | High | Two categories gets un attached from the chart |
| | 2. Tap on income and add $5000 in salary | | | | | |Categories lines gets crossed together |
| | 3. Add $100 in all 15 categories as expenses | | | | | |New category is added named Others and user can't access to see what's inside |
| | 4. Check chart |


# Third Part: Test Automation

Project Link: https://github.com/amroekamel96/Amr-Ehab1
