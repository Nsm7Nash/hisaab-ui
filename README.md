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


