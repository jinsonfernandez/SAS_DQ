# SAS_DQ
data kotak_1;
infile "C:\Users\jinsonf\Desktop\Kotak_bank_12_new.txt" 
dlm='09'x missover truncover DSD firstobs=2;

informat "EnquiryControlNumber" $100.;
informat MemberReference $100.;
informat Loan_account_Number $100.;
informat EnquiryMemberShortname $100.;
informat DateProcessed $100.;
informat TimeProcessed $100.;
informat name $100.;
informat DateofBirth $100.;
informat gender $100.;
informat IncomeTaxIDNumber$100.;
informat PassportNumber	 $100.;
informat VoterIDNumber	 $100.;
informat Telephone	 $100.;
informat address	 $100.;
informat StateCode	 $100.;
informat PINCode	 $100.;
informat DateReported_address $100.;


format EnquiryControlNumber $100.;
format MemberReference $100.;
format EnquiryMemberCode $100.;
format EnquiryMemberShortname $100.;
format DateProcessed $100.;
format TimeProcessed $100.;
format name $100.;
format DateofBirth $100.;
format gender $100.;
format IncomeTaxIDNumber $100.;
format PassportNumber $100.;
format VoterIDNumber $100.;
format Telephone $100.;
format address $100.;
format StateCode $100.;
format PINCode $100.;
format DateReported_address $100.;


input

EnquiryControlNumber $
MemberReference $
EnquiryMemberCode $
EnquiryMemberShortname$
DateProcessed $
TimeProcessed $
name $
DateofBirth $
gender $
IncomeTaxIDNumber $
PassportNumber $
VoterIDNumber $
Telephone $
address $
StateCode $
PINCode $
DateReported_address $;
run;



proc compare
base = cap_1 compare  = kotak_1  NOVALUES LISTBASEVAR;
title 'Base Varaible:CAPITAL FIRST COMPARISON';
run;

_____________________________________________________________________________________________________________________________________________________________________________
informat EnquiryControlNumber $100.;
informat MemberReference $100.;
informat Loan_account_Number $100.;
informat Loan_Status	 $100.;
informat Loan_Type	 $100.;
informat Loan_Classification	 $100.;
informat Sanction_Amount	 $100.;
informat High_Credit_Amount	 $100.;
informat Out_standing_Balance	 $100.;
informat EMI	$100.;
informat CREDITLIMIT		 $100.;
informat CASH_LIMIT		 $100.;
informat actual_paymt_amt		 $100.;
informat Interest_Rates		 $100.;
informat tenor		 $100.;
informat Income		 $100.;
informat monthly_annual_indicator	 $100.;
informat net_gross_indicator		 $100.;
informat occupation_code		 $100.;
informat COLLATERALTYPE		 $100.;
informat COLLATERALVALUE		 $100.;
informat DATE_OPENED		 $100.;
informat DATE_CLOSED		 $100.;
informat DateReported_trades		 $100.;
informat Last_payment_date		 $100.;
informat Pay_Hist_Start_Date		 $100.;
informat Pay_Hist_END_Date		 $100.;
informat Ownership_type		 $100.;
informat Over_due_amount		 $100.;
informat Tenor_Frequency		 $100.;
informat suit_filed_status		 $100.;
informat writeoff_status		 $100.;
informat writeoff_amt_tot		 $100.;
informat writeoff_amt_prin		 $100.;
informat settlement_amt		 $100.;
informat Dpd_string		 $100.;
informat PL_Propensity_Score		 $100.;
informat NTC_Score		 $100.;
informat TU_Score		 $100.;
informat ExclusionCode1		 $100.;
informat ExclusionCode2		 $100.;
informat ExclusionCode3		 $100.;
informat ExclusionCode4		 $100.;
informat ExclusionCode5		 $100.;
informat ExclusionCode6		 $100.;
informat ExclusionCode7		 $100.;
informat ReasonCode1		 $100.;
informat ReasonCode2		 $100.;
informat ReasonCode3		 $100.;
informat ReasonCode4		 $100.;
informat ReasonCode5		 $100.;
informat ErrorCode		 $100.;
informat Sector		 $100.;

format EnquiryControlNumber $100.;
format MemberReference $100.;
format Loan_account_Number $100.;
format Loan_Status $100.;
format Loan_Type $100.;
format Loan_Classification $100.;
format Sanction_Amount $100.;
format High_Credit_Amount $100.;
format Out_standing_Balance $100.;
format EMI $100.;
format CREDITLIMIT $100.;
format CASH_LIMIT $100.;
format actual_paymt_amt $100.;
format Interest_Rates $100.;
format tenor $100.;
format Income $100.;
format monthly_annual_indicator $100.;
format net_gross_indicator $100.;
format occupation_code $100.;
format COLLATERALTYPE $100.;
format COLLATERALVALUE $100.;
format DATE_OPENED $100.;
format DATE_CLOSED $100.;
format DateReported_trades $100.;
format Last_payment_date $100.;
format Pay_Hist_END_Date $100.;
format Ownership_type $100.;
format Over_due_amount $100.;
format Tenor_Frequency $100.;
format suit_filed_status $100.;
format writeoff_status $100.;
format writeoff_amt_tot $100.;
format writeoff_amt_prin $100.;
format settlement_amt $100.;
format Dpd_string $100.;
format PL_Propensity_Score $100.;
format NTC_Score $100.;
format TU_Score $100.;
format ExclusionCode1 $100.;
format ExclusionCode2 $100.;
format ExclusionCode3 $100.;
format ExclusionCode4 $100.;
format ExclusionCode5 $100.;
format ExclusionCode6 $100.;
format ExclusionCode7 $100.;
format ReasonCode1 $100.;
format ReasonCode2 $100.;
format ReasonCode3 $100.;
format ReasonCode4 $100.;
format ReasonCode5 $100.;
format ErrorCode $100.;
format Sector $100.;

input

EnquiryControlNumber $
MemberReference $
Loan_account_Number $
Loan_Status$
Loan_Type $
Loan_Classification $
Sanction_Amount $
High_Credit_Amount $
Out_standing_Balance $
EMI $
CREDITLIMIT $
CASH_LIMIT $
actual_paymt_amt $
Interest_Rates $
tenor $
Income $
monthly_annual_indicator $
net_gross_indicator $
occupation_code $
COLLATERALTYPE $
COLLATERALVALUE $
DATE_OPENED $
DATE_CLOSED $
DateReported_trades $
Last_payment_date $
Pay_Hist_END_Date $
Ownership_type $
Over_due_amount $
Tenor_Frequency $
suit_filed_status $
writeoff_status $
writeoff_amt_tot $
writeoff_amt_prin $
settlement_amt $
Dpd_string $
PL_Propensity_Score $
NTC_Score $
TU_Score $
ExclusionCode1 $
ExclusionCode2 $
ExclusionCode3 $
ExclusionCode4 $
ExclusionCode5 $
ExclusionCode6 $
ExclusionCode7 $
ReasonCode1 $
ReasonCode2 $
ReasonCode3 $
ReasonCode4 $
ReasonCode5 $
ReasonCode6 $
ErrorCode $
Sector $ ;
run;

_______________________________________________________________________________________________________________________________________________________________________________

proc import
datafile  = " C:\Users\jinsonf\Desktop\priome_tl.csv"
out = prime_data
dbms = dlm
replace;
getnames = yes;
Delimeter = ',';
run;
_______________________________________________________________________________________________________________________________________________________________________________
count of unique
proc sql;
create table a as
select MemberReference,count(*) as ct from prime_data 
group by MemberReference order by 2 desc;
quit;
_____________________________________________________________________________________________________________________________
        



