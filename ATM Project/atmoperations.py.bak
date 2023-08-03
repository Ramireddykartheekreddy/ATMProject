#atmoperations.py
from atmexcept import DepositError,WithdrawError,InSuffFundError
bal=500.00
def  deposit():
	damt=float(input("Enter ur Depoist amount:"))
	if(damt<=0):
		raise DepositError
	else:
		global bal
		bal=bal+damt
		print("\nUr account xxxxxx123 credited with INR {}".format(damt))
		print("Ur Current Account Balanace after deposit INR:{}".format(bal))

def withdraw():
	global bal
	wamt=float(input("Enter the withdraw amount:"))
	if(wamt<=0):
		raise WithdrawError
	elif((wamt+500)>bal):
		raise InSuffFundError 
	else:
		bal=bal-wamt
		print("\nUr account xxxxxx123 debited with INR {}".format(wamt))
		print("Ur Current Account Balanace after withdraw INR:{}".format(bal))

def balEnq():
	print("Ur Current Account Balanace  INR:{}".format(bal))