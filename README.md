# Bank

This challenge helps you practice your OO design skills.

You'll work alone, and you'll also review your own code so you can practice reflecting on and improving your own work.

## Specification

### Requirements

* You should be able to interact with your code via a JavaScript REPL - Node REPL or browser console  (You don't need to implement a command line interface that takes input from STDIN.)
* Deposits, withdrawal.
* Account statement (date, credit or debit amount, balance) printing.
* Data can be kept in memory (it doesn't need to be stored to a database or anything).

### Acceptance criteria

**Given** a client makes a deposit of 1000 on 10-01-2012  
**And** a deposit of 2000 on 13-01-2012  
**And** a withdrawal of 500 on 14-01-2012  
**When** she prints her bank statement  
**Then** she would see

```
date       || credit  || debit  || balance
14/01/2012 ||         || 500.00 || 2500.00
13/01/2012 || 2000.00 ||        || 3000.00
10/01/2012 || 1000.00 ||        || 1000.00
```


#### Standard
- [v ] Meets the spec
- [v ] Developed test-first (commit your tests before your source code to provide evidence of this)
- [v ] Passes tests
- [v ] Encapsulates adding and storing Transactions in a class
- [v ] Encapsulates Statement formatting in a class
- [v ] Encapsulates Transaction data in a class

#### Extensions
- [ ] Generate ordered bank statements between 2 dates
- [v ] Disable withdraws if the withdraw amount exceeds the available funds. Available funds must be calculated based on a complete transaction history, not a variable that gets updated
- [v ] Allow adding a 500 overdraft to the account
- [v ] Different account types (Savings, Investment, Checking). Savings & Investment accounts cant have overdrafts, Checking accounts can. Investment accounts accumulate 2% interest every month.
- [v ] Deposit limits of 20,000 per year on Savings accounts
- [ ] A front-end online banking app
- [ ] Generate PDFs of bank statements
