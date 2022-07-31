// Design a banking system like EasyPaisa

// 1. Components we require (Functionalities)
// 2. Communication/connection among components


1. Users 
    Sign In / Sign Up
    Account Verification
    
2. Accounts
     Add / Remove Accounts
     Account TopUp
   
3. Bills
    Add Bills
    Remove Bills
    
     
4. Beneficiaries
    Add / Remove Beneficiary + Verification for adding
    
5. Transactions
    Bill Payment
    Pay to anyone
    Mobile top-ups

6. Verifications
    Handle verification like Sign-Up, Adding Beneficiary, Sending payments
    
7. Notifications
     Notification for Different Events like (Bill Payment, Pay to anyone, and Mobile Topups)
   1 option is to keep text templates in database - admin can edit too
   2nd option preferred is to keep a file (server location)
   3rd store as a string in a class

   Notification interface
     separate classes for sms, email, etc
   could do via queues system or scheduled using databases (or hybrid)

Transaction
Type - Bill Payment, Mobile Topup, etc.

**Database:**

Use relational database for the system (preferred)

**Scalability:**
- use async programming where possible
  - e.g.? populate list of banks, etc
- auto scale on server 