# HisaabUi

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.1.0.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

# Hisaab-UI


## Features
##### 1. Sign up.(future: sign up by gmail,fb)
##### 2. Login.
##### 3. Add Friend. (by email, phone number)
##### 4. Add Transaction/update/delete/undelete. (split by %, equally, parts|paid by)
##### 5. Dashboard (owed/owe).
##### 6. Settle up.
##### 7. Notification email/text - (Settle up,add a friend, each transaction notification(opt in/opt out), Monthly statement) - future scope:Browser notification. (Future scope : standard unsubscribe from future email option within email)
##### 8. Add/update/delete/undelete Comments for trasction.
##### ----------------------------------------------------------------------------------------------------------------------------------

## Tables: Add table constraints, normalize
##### 1. User Profile table. - user name(PK), pass/auth token
##### 2. Transaction Table. - Column timestamp, tid(PK), amount, split type, settled flag.
##### 3. User table - user name(PK), first name, last name, email, phone
##### 4. Transaction-User reltaion table - (many to many)- rid(PK), transaction id, user id, group id.
##### 5. Owe table - hisaab_id(PK),Payee id, payer id, amount. (negative amount is allowed which denotes altered roles)
##### 6. Group table - group id(PK), group name, description.
##### 7. Group membership table - mid(PK),group id, user id.
##### 8. comments table- comment id(PK), text, person making the comment, transaction id(FK).



