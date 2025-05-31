# Stock-Exchange-Project


#include<stdio.h>

struct user
{
	char username[20];
	char password[20];
	char firstname[20];
	char lastname[20];
	char pan[20];
	double aadhar;
	char IFSC[50];
	int mobile;
};
struct payment
{
	int card_no;
	int expiry;
	int cvv;
	char name[30];
	int otp;
	char upi[30];
	int tran_id;
};
main()
{
	struct user u;
	int x,i,ch,t;
	struct payment k;
	char c,l,y,fg,o;
	float h,s_qua;
	printf("\n\t\t\t\t\t\t\tSTOCK MARKET EXCHANGE SYSTEM");
	printf("\n\t\t\t\t\t\t\t\t 1-->LOGIN");
	printf("\n\t\t\t\t\t\t\t\t 2-->SIGN UP");
	printf("\n\n\t\t\t\t\t CHOOSE YOUR CHOICE : ");
	scanf("%d",&x);
	switch(x)
	{
		case 1:
		printf("\n ENTER USERNAME: ");
		scanf("%s",u.username);
		printf("\n ENTER PASSWORD: ");
		scanf("%s",u.password);
		if(strcmp(u.username,"ARAVIND")==0)
		{
			if(strcmp(u.password,"AYYAPPA")==0)
			{
				printf("\n\t\t\t\t LOGIN SUCESSFULL");
					printf("\n a-->BUY THE SHARES");
	printf("\n b-->SELL THE SHARES");
	printf("\n PLEASE SELECT THE CHOICE: ");
	scanf(" %c",&c);
		int available[1000]={1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,
		1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,
		1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000};
	char pro_loss[][1000]={
"Profit","Loss","Profit","Loss","Profit","Loss","Profit","loss","Profit",
"Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss",
"Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit",
"Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss",
"Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit",
"Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss",
"Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss"};
	float share_price[1000]={3230.8,926.95,2441.30,
428.85,1625.35,576.36,2705.95,377.9,2501.00,560.10,1259.05,864.95,6289.90,970.45,1928.35,370.90,
2377.75,160.23,1055.15,176.72,8097.13,733.90,2734.95,240.45,3597.8,477.25,7095.5,937.25,2209,684.20,1927.78,237.89,
1359.99,108.65,1212.45,388.85,4488,3568.7,82.77,4569.36,598.63,2422.56,999.36,1173.35,
421.90,4439.89};
	char companies[][1000]={"TATA CONSULTANCY SERVICES LTD.","ICICI BANK LTD             ",
	"RELIANCE INDUSTRIES LTD.   ",	"ITC LTD.                 ","HDFC Bank Ltd             ",
"STATE BANK OF INDIA     ","HOUSING DEVELOPMENTFINANCE.LTD",
"BHARTI AIRTEL LTD.       ","HINDUSTAN UNILEVER LTD.  ","Life Insurance Corp INDIA.LTD",
"INFOSYS LTD.               ","AXIS BANK LTD.          ","Bajaj Finance Limited       ",
"SUN PHARMACEUTICAL INDU LTD.","KOTAK MAHINDRA BANK LTD. ","WIPRO LTD.                ",
"LARSEN & TOUBRO LTD.     ","Oil and Natural Gas Corp Ltd","HCL TECHNOLOGIES LTD.   ",
 "NTPC LTD.	              ","MARUTI SUZUKI INDIA LTD.  ","JSW STEEL LTD.	         " ,
 "Titan Company Limited     ","POWER GRID CORP oF INDIA","Avenue Supermarts Ltd    ",
 "TATA MOTORS LTD.        ","ULTRATECH CEMENT LTD.	 ","Adani Green Energy Ltd  ","NESTLE INDIA LTD.	  ",
 "ADANI PORTS AND SPECIAL.LTD","ADANI ENTERPRISES LTD.         ","COAL INDIA LTD.   	      ",
 "BAJAJ FINSERV LTD.	     ","TATA STEEL LTD.	        ","MAHINDRA & MAHINDRA LTD. ",
"HINDUSTAN ZINC LTD.	  ","LTIMindtree Ltd	        ","SIEMENS LTD.	         ",
"INDIAN OIL CORPORATION LTD. ", "BAJAJ AUTO LTD.     	    ","HDFC Life Insurance Company Ltd",
"PIDILITE INDUSTRIES LTD.","Adani Transmission Ltd	  ","SBI Life Insurance Ltd	",
"DLF LTD.	        ","DR.REDDY'S LABORATOR LTD."
};
		switch(c)
		{
			case 'a':
			printf("\n\n1-->Companies With Share Price Above RS:1000/- with profit");
			printf("\n\n2-->Companies With Share Price Below RS:1000/- with loss");
			printf("\n\n3-->All Companies");
			printf("\n\nPLEASE SELECT A CHOICE : ");
			scanf("%d",&ch);
			if(ch==1)
			{
				printf("\n\nCompanies With Share Price Above RS:1000/-");
			  printf("\n\nChoice\t\tCompany\t\t\t\t\t\t\t\t\t\t\tPrice\t\t\t\t Profit/Loss\t\t\tAVAILABLE");
			  printf("\n**\n");
				for(i=0;i<46;i++)
				{
					if(i%2==0)
					printf("\n%d\t\t%s\t\t\t\t\t\t\t\t%0.2f\t\t\t\t%s\t\t\t\t%d",i,companies[i],share_price[i],pro_loss[i],available[i]);

				}
			}
			if(ch==2)
			{
				printf("\n\nCompanies With Share Price Below RS:1000/-");
			  printf("\n\nChoice\t\tCompany\t\t\t\t\t\t\t\t\t\t\tPrice\t\t\t\t Profit/Loss\t\t\tAVAILABLE");
			  printf("\n*\n");
				for(i=0;i<46;i++)
				{
					if(i%2!=0)
                    printf("\n%d\t\t%s\t\t\t\t\t\t\t\t%0.2f\t\t\t\t%s\t\t\t\t%d",i,companies[i],share_price[i],pro_loss[i],available[i]);

				}
		    }
		    if(ch==3)
			{
				printf("\n\nAll Companies Are");
			  printf("\n\nChoice\t\tCompany\t\t\t\t\t\t\t\t\t\t\tPrice\t\t\t\t Profit/Loss\t\t\tAVAILABLE");
			  printf("\n**\n");
				for(i=0;i<46;i++)
				{
					printf("\n%d\t\t%s\t\t\t\t\t\t\t\t%0.2f\t\t\t\t%s\t\t\t\t%d",i,companies[i],share_price[i],pro_loss[i],available[i]);
				}
		    }
		    printf("\n\nSelect the Choice number of the Company you Wish to Invest : ");
		    scanf("%d",&i);
		    printf("\n Please Enter the Amount You Wish To Invest : ");
		    	scanf("%f",&h);
		    	s_qua=(h/share_price[i]);
		    	printf("\nThe Shares you get for %d : %0.1f ",u,s_qua);    
	    	printf("\n\nIf you wish to continue to payment press 'p'");
		    	scanf(" %c",&l);
		    	if(l=='p')
				{
		    	printf("\n d-->Debit/Credit Cards");
		    	printf("\n u-->UPI");
		    	printf("\n\nSelect your Payment Method");
		    	scanf(" %c",&y);
		    	if(y=='d')
		    	{
		    		printf("\nEnter Following Details");
		    		printf("\n\nCard Number : ");
		    		scanf("%d",&k.card_no);
		    		printf("\n\nExpiry Month/Year:");
		    		scanf("%d",&k.expiry);
		    		printf("\n\nCVV");
		    		scanf("%d",&k.cvv);
		    		printf("Card Holder Name");
		    		scanf("%s",k.name);
		    		printf("Press c to confirm you purchase");
		    		scanf(" %c",&fg);
		    	
		    		if(fg=='c')
		    		{
		    			printf("\n\nYour Purchase is in Process......");
		    			printf("\n\nEnter 6 Digit OTP Sent To your Mobile Number");
		    		    scanf("%d",&k.otp);
		    		    printf("\n\nYour Purchase has been Confirmed");
		    	        printf("\n\n----------------------------------------------------------------Purchase Details-------------------------------------------------------------------------------------------------------------------");
		    		    printf("\n\n\t\t\t\t\tChoice : %d\n\t\t\t\t\tCompany : %s\n\t\t\t\t\tAmount Invested : %f\n\t\t\t\t\tShares Got : %0.1f",i,companies[i],h,s_qua);
					}
				}
				else if(y=='u')
				{
					printf("\n\nEnter Your UPI ID : ");
					scanf("%s",k.upi);
					printf("\n Payment Request Has Been Sent....");
					printf("\nContinue You Transanction On your UPI App.......");
					printf("Please Enter Transaction Id Of your Purchase : ");
					scanf("%d",&k.tran_id);
					printf("\n\nYour Purchase has been Confirmed");
		    	        printf("\n\n----------------------------------------------------------------Purchase Details-------------------------------------------------------------------------------------------------------------------");
		    		    printf("\n\n\t\t\t\t\tChoice : %d\n\t\t\t\t\tCompany : %s\n\t\t\t\t\tAmount Invested : %f\n\t\t\t\t\tShares Got : %0.1f",i,companies[i],h,s_qua);	
				}
			
				break;
		}
		    
		    case'b':
		    		printf("\n\nAll Companies Are");
		    		printf("\n\nChoice\t\tCompany\t\t\t\t\t\t\t\t\t\t\tPrice\t\t\t\t Profit/Loss\t\t\tAVAILABLE");
		    		printf("\n**\n");

					for(i=0;i<46;i++)
				{
					printf("\n%d\t\t%s\t\t\t\t\t\t\t\t%0.2f\t\t\t\t%s\t\t\t\t%d",i,companies[i],share_price[i],pro_loss[i],available[i]);
				}
			 printf("\n\nSelect the Choice number of the Company you Wish to sell : ");
		    scanf("%d",&i);
		    printf("\n Please Enter the Number of Shares You Wish To Sell : ");
		    	scanf("%f",&h);
		    	s_qua=(h*share_price[i]);
		    	printf("\nThe Shares you get for %f : %0.1f ",h,s_qua); 
		    	printf("\n\nIf you wish to Continue 'p'");
		    	scanf(" %c",&o);
		    	if(o=='p'){
		    	printf("\n d-->Debit/Credit Cards");
		    	printf("\n u-->UPI");
		    	printf("\n\nSelect your Method Through which your amount will be credited");
		    	scanf(" %c",&y);
		    	if(y=='d')
		    	{
		    		printf("\nEnter Following Details");
		    		printf("\n\nCard Number : ");
		    		scanf("%d",&k.card_no);
		    		printf("\n\nExpiry Month/Year");
		    		scanf("%d",&k.expiry);
		    		printf("\n\nCVV");
		    		scanf("%d",&k.cvv);
		    		printf("Card Holder Name");
		    		scanf("%s",k.name);
		    		printf("Press c to confirm you purchase");
		    		scanf(" %c",&fg);
		    	
		    		if(fg=='c')
		    		{
		    			printf("\n\nYour Transaction is in Process......");
		    			printf("\n\nEnter 6 Digit OTP Sent To your Mobile Number");
		    		    scanf("%d",&k.otp);
		    		    printf("\n\nYour Transaction has been Confirmed");
		    	       printf("\n\n--------------------------------------------------------------------------Details----------------------------------------------------------------------------------------------------------");
		    		    printf("\n\n\t\t\t\t\tChoice : %d\n\t\t\t\t\tCompany : %s\n\t\t\t\t\tShares sold : %f\n\t\t\t\t\tAmount Credited : %0.2f",i,companies[i],h,s_qua);	
				}
				}
				else if(y=='u')
				{
					printf("\n\nEnter Your UPI ID : ");
					scanf("%s",k.upi);
					printf("\n Payment Request Has Been Sent....");
					printf("\n Your Transaction is in Process.......");
					printf("\n\nYour Transaction has been Confirmed");
		    	       printf("\n\n--------------------------------------------------------------------------Details----------------------------------------------------------------------------------------------------------");
		    		    printf("\n\n\t\t\t\t\tChoice : %d\n\t\t\t\t\tCompany : %s\n\t\t\t\t\tShares sold : %f\n\t\t\t\t\tAmount Credited : %0.2f",i,companies[i],h,s_qua);	
				}
				}
				break;
			}
        }

			}

		else
		{
			printf("\n wrong username and password");
			printf("\n this user does not exist");
		}
		break;
		case 2:
		printf("\nENTER FIRSTNAME: ");
		scanf("%s",u.firstname);
		printf("\nENTER LASTNAME: ");
		scanf("%s",u.lastname);
		printf("\nENTER USERNAME: ");
		scanf("%s",u.username);
		printf("\nENTER PASSWORD: ");
		scanf("%s",u.password);
		printf("\nENTER TO CONFIRM PASSWORD: ");
		scanf("%s",u.password);	
		printf("\nENTER YOUR PAN NUMBER : ");
        scanf("%s",u.pan);
        printf("\nENTER YOUR AADHAR NUMBER : ");
        scanf("%lf",&u.aadhar);
        printf("\nENTER YOUR BANK IFSC CODE : ");
        scanf("%s",u.IFSC);
        printf("\nENTER YOUR PHONE NUMBER : ");
        scanf("%d",&u.mobile);
        printf("\n\t\t\t\tYOU SIGNED UP");
			printf("\n a-->BUY THE SHARES");
	printf("\n b-->SELL THE SHARES");
	printf("\n PLEASE SELECT THE CHOICE: ");
	scanf(" %c",&c);
		int available[1000]={1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,
		1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,
		1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000,1000};
	char pro_loss[][1000]={
"Profit","Loss","Profit","Loss","Profit","Loss","Profit","loss","Profit",
"Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss",
"Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit",
"Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss",
"Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit",
"Loss","Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss",
"Profit","Loss","Profit","Loss","Profit","Loss","Profit","Loss"};
	float share_price[1000]={3230.8,926.95,2441.30,
428.85,1625.35,576.36,2705.95,377.9,2501.00,560.10,1259.05,864.95,6289.90,970.45,1928.35,370.90,
2377.75,160.23,1055.15,176.72,8097.13,733.90,2734.95,240.45,3597.8,477.25,7095.5,937.25,2209,684.20,1927.78,237.89,
1359.99,108.65,1212.45,388.85,4488,3568.7,82.77,4569.36,598.63,2422.56,999.36,1173.35,
421.90,4439.89};
	char companies[][1000]={"TATA CONSULTANCY SERVICES LTD.","ICICI BANK LTD             ",
	"RELIANCE INDUSTRIES LTD.   ",	"ITC LTD.                 ","HDFC Bank Ltd             ",
"STATE BANK OF INDIA     ","HOUSING DEVELOPMENTFINANCE.LTD",
"BHARTI AIRTEL LTD.       ","HINDUSTAN UNILEVER LTD.  ","Life Insurance Corp INDIA.LTD",
"INFOSYS LTD.               ","AXIS BANK LTD.          ","Bajaj Finance Limited       ",
"SUN PHARMACEUTICAL INDU LTD.","KOTAK MAHINDRA BANK LTD. ","WIPRO LTD.                ",
"LARSEN & TOUBRO LTD.     ","Oil and Natural Gas Corp Ltd","HCL TECHNOLOGIES LTD.   ",
 "NTPC LTD.	              ","MARUTI SUZUKI INDIA LTD.  ","JSW STEEL LTD.	         " ,
 "Titan Company Limited     ","POWER GRID CORP oF INDIA","Avenue Supermarts Ltd    ",
 "TATA MOTORS LTD.        ","ULTRATECH CEMENT LTD.	 ","Adani Green Energy Ltd  ","NESTLE INDIA LTD.	  ",
 "ADANI PORTS AND SPECIAL.LTD","ADANI ENTERPRISES LTD.         ","COAL INDIA LTD.   	      ",
 "BAJAJ FINSERV LTD.	     ","TATA STEEL LTD.	        ","MAHINDRA & MAHINDRA LTD. ",
"HINDUSTAN ZINC LTD.	  ","LTIMindtree Ltd	        ","SIEMENS LTD.	         ",
"INDIAN OIL CORPORATION LTD. ", "BAJAJ AUTO LTD.     	    ","HDFC Life Insurance Company Ltd",
"PIDILITE INDUSTRIES LTD.","Adani Transmission Ltd	  ","SBI Life Insurance Ltd	",
"DLF LTD.	        ","DR.REDDY'S LABORATOR LTD."
};
		switch(c)
		{
			case 'a':
			printf("\n\n1-->Companies With Share Price Above RS:1000/- with profit");
			printf("\n\n2-->Companies With Share Price Below RS:1000/- with loss");
			printf("\n\n3-->All Companies");
			printf("\n\nPLEASE SELECT A CHOICE : ");
			scanf("%d",&ch);
			if(ch==1)
			{
				printf("\n\nCompanies With Share Price Above RS:1000/-");
			  printf("\n\nChoice\t\tCompany\t\t\t\t\t\t\t\t\t\t\tPrice\t\t\t\t Profit/Loss\t\t\tAVAILABLE");
			  printf("\n**\n");
				for(i=0;i<46;i++)
				{
					if(i%2==0)
					printf("\n%d\t\t%s\t\t\t\t\t\t\t\t%0.2f\t\t\t\t%s\t\t\t\t%d",i,companies[i],share_price[i],pro_loss[i],available[i]);

				}
			}
			if(ch==2)
			{
				printf("\n\nCompanies With Share Price Below RS:1000/-");
			  printf("\n\nChoice\t\tCompany\t\t\t\t\t\t\t\t\t\t\tPrice\t\t\t\t Profit/Loss\t\t\tAVAILABLE");
			  printf("\n*\n");
				for(i=0;i<46;i++)
				{
					if(i%2!=0)
                    printf("\n%d\t\t%s\t\t\t\t\t\t\t\t%0.2f\t\t\t\t%s\t\t\t\t%d",i,companies[i],share_price[i],pro_loss[i],available[i]);

				}
		    }
		    if(ch==3)
			{
				printf("\n\nAll Companies Are");
			  printf("\n\nChoice\t\tCompany\t\t\t\t\t\t\t\t\t\t\tPrice\t\t\t\t Profit/Loss\t\t\tAVAILABLE");
			  printf("\n**\n");
				for(i=0;i<46;i++)
				{
					printf("\n%d\t\t%s\t\t\t\t\t\t\t\t%0.2f\t\t\t\t%s\t\t\t\t%d",i,companies[i],share_price[i],pro_loss[i],available[i]);
				}
		    }
		    printf("\n\nSelect the Choice number of the Company you Wish to Invest : ");
		    scanf("%d",&i);
		    printf("\n Please Enter the Amount You Wish To Invest : ");
		    	scanf("%f",&h);
		    	s_qua=(h/share_price[i]);
		    	printf("\nThe Shares you get for %d : %0.1f ",u,s_qua);    
	    	printf("\n\nIf you wish to continue to payment press 'p'");
		    	scanf(" %c",&l);
		    	if(l=='p')
				{
		    	printf("\n d-->Debit/Credit Cards");
		    	printf("\n u-->UPI");
		    	printf("\n\nSelect your Payment Method");
		    	scanf(" %c",&y);
		    	if(y=='d')
		    	{
		    		printf("\nEnter Following Details");
		    		printf("\n\nCard Number : ");
		    		scanf("%d",&k.card_no);
		    		printf("\n\nExpiry Month/Year:");
		    		scanf("%d",&k.expiry);
		    		printf("\n\nCVV");
		    		scanf("%d",&k.cvv);
		    		printf("Card Holder Name");
		    		scanf("%s",k.name);
		    		printf("Press c to confirm you purchase");
		    		scanf(" %c",&fg);
		    	
		    		if(fg=='c')
		    		{
		    			printf("\n\nYour Purchase is in Process......");
		    			printf("\n\nEnter 6 Digit OTP Sent To your Mobile Number");
		    		    scanf("%d",&k.otp);
		    		    printf("\n\nYour Purchase has been Confirmed");
		    	        printf("\n\n----------------------------------------------------------------Purchase Details-------------------------------------------------------------------------------------------------------------------");
		    		    printf("\n\n\t\t\t\t\tChoice : %d\n\t\t\t\t\tCompany : %s\n\t\t\t\t\tAmount Invested : %f\n\t\t\t\t\tShares Got : %0.1f",i,companies[i],h,s_qua);
					}
				}
				else if(y=='u')
				{
					printf("\n\nEnter Your UPI ID : ");
					scanf("%s",k.upi);
					printf("\n Payment Request Has Been Sent....");
					printf("\nContinue You Transanction On your UPI App.......");
					printf("Please Enter Transaction Id Of your Purchase : ");
					scanf("%d",&k.tran_id);
					printf("\n\nYour Purchase has been Confirmed");
		    	        printf("\n\n----------------------------------------------------------------Purchase Details-------------------------------------------------------------------------------------------------------------------");
		    		    printf("\n\n\t\t\t\t\tChoice : %d\n\t\t\t\t\tCompany : %s\n\t\t\t\t\tAmount Invested : %f\n\t\t\t\t\tShares Got : %0.1f",i,companies[i],h,s_qua);	
				}
			
				break;
		}
		    
		    case'b':
		    		printf("\n\nAll Companies Are");
		    		printf("\n\nChoice\t\tCompany\t\t\t\t\t\t\t\t\t\t\tPrice\t\t\t\t Profit/Loss\t\t\tAVAILABLE");
			        printf("\n**\n");
					for(i=0;i<46;i++)
				{
					printf("\n%d\t\t%s\t\t\t\t\t\t\t\t%0.2f\t\t\t\t%s\t\t\t\t%d",i,companies[i],share_price[i],pro_loss[i],available[i]);
				}
			 printf("\n\nSelect the Choice number of the Company you Wish to sell : ");
		    scanf("%d",&i);
		    printf("\n Please Enter the Number of Shares You Wish To Sell : ");
		    	scanf("%f",&h);
		    	s_qua=(h*share_price[i]);
		    	printf("\nThe Shares you get for %f : %0.1f ",h,s_qua); 
		    	printf("\n\nIf you wish to Continue 'p'");
		    	scanf(" %c",&o);
		    	if(o=='p'){
		    	printf("\n d-->Debit/Credit Cards");
		    	printf("\n u-->UPI");
		    	printf("\n\nSelect your Method Through which your amount will be credited");
		    	scanf(" %c",&y);
		    	if(y=='d')
		    	{
		    		printf("\nEnter Following Details");
		    		printf("\n\nCard Number : ");
		    		scanf("%d",&k.card_no);
		    		printf("\n\nExpiry Month/Year");
		    		scanf("%d",&k.expiry);
		    		printf("\n\nCVV");
		    		scanf("%d",&k.cvv);
		    		printf("Card Holder Name");
		    		scanf("%s",k.name);
		    		printf("Press c to confirm you purchase");
		    		scanf(" %c",&fg);
		    	
		    		if(fg=='c')
		    		{
		    			printf("\n\nYour Transaction is in Process......");
		    			printf("\n\nEnter 6 Digit OTP Sent To your Mobile Number");
		    		    scanf("%d",&k.otp);
		    		    printf("\n\nYour Transaction has been Confirmed");
		    	        printf("\n\n--------------------------------------------------------------------------Details----------------------------------------------------------------------------------------------------------");
		    		    printf("\n\n\t\t\t\t\tChoice : %d\n\t\t\t\t\tCompany : %s\n\t\t\t\t\tShares sold : %f\n\t\t\t\t\tAmount Credited : %0.2f",i,companies[i],h,s_qua);	
				}
				}
				else if(y=='u')
				{
					printf("\n\nEnter Your UPI ID : ");
					scanf("%s",k.upi);
					printf("\n Payment Request Has Been Sent....");
					printf("\n Your Transaction is in Process.......");
					printf("\n\nYour Transaction has been Confirmed");
		    	        printf("\n\n--------------------------------------------------------------------------Details----------------------------------------------------------------------------------------------------------");
		    		    printf("\n\n\t\t\t\t\tChoice : %d\n\t\t\t\t\tCompany : %s\n\t\t\t\t\tShares sold : %f\n\t\t\t\t\tAmount Credited : %0.2f",i,companies[i],h,s_qua);	
				}
			
				}
				break;
			}
}
	}
