# dattaram_shinde
class BankAccount:
    def __init__(self,accNo,custName,dateOfOpening,balance):
        self.account_number=accNo
        self.customer_name=custName
        self.date_of_opening=dateOfOpening
        self.balance=balance
    def deposite(self,depositAmount):
        self:balance =depositAmount
        print("successfully deposited",depositAmount,"\n")
    def withdraw(self,withdrawAmount):
        if self.balance<withdrawAmount:
            print("insufficient balance\n")
        else:
            self.balance-=withdrawAmount
            print("successfully withdraw",withdrawAmount,"\n")
    def check_balance(self):
        print("a/c No=",self.account_number)
        print("customer no=",self.customer_name)

        print("date of opening=",self.date_of_opening)

        print("balance=",self.balance)
        print("================================================")
a1=BankAccount(654123987,"datta","12-06-2023",50000)
a1.check_balance()
a1.deposite(5000)
print("after deposit\n")
a1.check_balance()
a1.withdraw(10000)
print("after withdraw\n")
a1.check_balance()




