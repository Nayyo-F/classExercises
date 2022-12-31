#include<iostream>
#include<string>
#include<cstring>
#include<fstream>

using namespace std;

const int SIZE=10;


struct clinic

{
// personal information
int id;
int date;
int month;
int year;
char fname[20];
char lname[20];
int age;
char sex;
char address[20];
char occupation[20];

// current health situation
char examination_room[30];
char in_out_patient[5];
char laboratory_examination[50];
char finding_diagnosis[50];
char result[50];
char medicine[50];
int appointment_date;
int appointment_month;
int appointment_year;
char suggestion[5000];

};

int new_register();
int search_All_patient();
int search_patient();
int no;
int No_patient;
int i=0;

clinic hos[SIZE];

int main()

{


int choice;
cout<<endl<<"JIT CLINIC REGISTRSTION SYSTEM!\n";
cout<<"****************************************************************************"<<endl;
menu:
cout<<"Enter your choice\n\n";
cout<<"\t\t>> 1 New patient Registration \n";
cout<<"\t\t>> 2 search detail of All patient\n";
cout<<"\t\t>> 3 search detail of existing  patient\n";
cout<<"\t\t>> 0 Exit system\n";

cin>>choice;

switch(choice){

case 1:
new_register();
goto menu;
break;
case 2:
search_All_patient();
goto menu;
break;
case 3:
search_patient();
goto menu;
break;
case 0:
goto end;
break;
default :
cout<<"make a correct choice\n";
goto menu;
break;
}

end:

return 0;
}



int new_register(){

ofstream out("CLINIC_REPORT.txt");
if(!out){

cout<<"cannot open CLINIC REPORT file.\n";
return 1;

}

//filling information
char key;


do
{
cout<<"\n\n============personal information===";
cout<<"\nEnter the personal information of the patient \n";
//cout<<"Enter the personal information of the patient\n";

cout<<"Id No: ";
//out<<"Id No: ";
cin>>hos[i].id;
//cout<<endl;
//cout<<hos[i].id;
cout<<endl;

date:

cout<<"Date: ";
//cout<<endl;


cin>>hos[i].date;

if(hos[i].date<1||hos[i].date>31){



cout<<"Enter the proper format of date that is from 1 to 31 maximum \n";
goto date;

}



//cout<<hos[i].date;
cout<<endl;
month:

cout<<"month: ";
//cout<<"\nmonth :";

cin>>hos[i].month;


if(hos[i].month<1||hos[i].month>12){

cout<<"Enter the proper format of month that is from 1 to 12 maximum\n";

goto month;

}

//cout<<hos[i].month;
cout<<endl;

year:

cout<<"year: ";

//cout<<"\nyear: ";

cin>>hos[i].year;\


if(hos[i].year<2022||hos[i].year>2024){

cout<<"Enter the proper format of year that is from year 2022 to 2024\n";
goto year;

}


//cout<<hos[i].year;
cout<<endl;
cout<<"First Name: ";

//cout<<"\nName: ";

cin>>hos[i].fname;

//cout<<"\nName: ";
cout<<endl;
cout<<"Last Name: ";

cin>>hos[i].lname;

//cout<<hos[i].name;
cout<<endl;
Age:

cout<<"Age: ";

//cout<<"\nAge: ";

cin>>hos[i].age;


if(hos[i].age<0||hos[i].age>100){

cout<<"Enter the proper format of Age that is up to 120 maximum\n";
goto Age;

}



//cout<<hos[i].age;
cout<<endl;
sex:
cout<<"Sex: ";

//cout<<"\nSex: ";

cin>>hos[i].sex;

if(hos[i].sex!='M'&& hos[i].sex!='F'&& hos[i].sex=='m'&& hos[i].sex=='f'){
cout<<"Enter the proper format of sex that is M or F\n";
goto sex;

}



//cout<<hos[i].sex;
cout<<endl;
cout<<"Address: ";

//cout<<"\nAddress: ";
cin>>hos[i].address;

//cout<<hos[i].address;
cout<<endl;

//cout<<"occupation: ";
cout<<"Occupation: ";

cin>>hos[i].occupation;
cout<<endl;
//cout<<hos[i].occupation ;
cout<<endl;

newre:

int select;

cout<<"Examination room:\n";
//out<<"\nExamination room:  ";
cout<<"\t\t>>1 :Pediatrics 0PD\n";
cout<<"\t\t>>2 :Adult OPD\n";
cout<<"\t\t>>3 :ANC OPD\n";
cout<<"\t\t>>4 :Emergency OPD\n";
cout<<"\t\t>>5 :TB OPD\n";
cout<<"\t\t>>6 :Gynae OPD\n";
//cout<<endl;

cin>>select;


if(select==1){

strcpy(hos[i].examination_room,"Pediatrics OPD");
cout<<hos[i].examination_room;

}


else if(select==2){

strcpy(hos[i].examination_room,"Adult OPD");
out<<hos[i].examination_room;
}

else if(select==3){

strcpy(hos[i].examination_room,"ANC OPD");
out<<hos[i].examination_room;
}

else if(select==4){

strcpy(hos[i].examination_room,"Emergency OPD");
cout<<hos[i].examination_room;

}
else if(select==5){

strcpy(hos[i].examination_room,"TB OPD");
out<<hos[i].examination_room;
}

else if(select==6){

strcpy(hos[i].examination_room,"Gynae OPD");
out<<hos[i].examination_room;
}
else{

cout<<"Make a correct choice\n";
goto newre;
}

int location;
loc:
cout<<"Patient Location : \n";
//cout<<"\npatient Location : ";
cout<<"\t\t>>1 : Home\n";
cout<<"\t\t>>2 : Ward\n";
cin>>location;
if(location==1)
{
strcpy(hos[i].in_out_patient,"Home");
cout<<hos[i].in_out_patient;
}
else if(location==2)
{
strcpy(hos[i].in_out_patient,"Ward");
cout<<hos[i].in_out_patient;
}
else
{
cout<<"Make a correct choice \n";
goto loc;
}
lab:
cout<<"Laboratory Examination: \n";
//cout<<"\n laboratory Examination";

cout<<"\t\t>>1 : Hematology\n";
cout<<"\t\t>>2 : Urine analysis\n";
cout<<"\t\t>>3 : stool\n";
cout<<"\t\t>>4 : Gram stain\n";
cout<<"\t\t>>5 : Blood sugar\n";
cout<<"\t\t>>6 : Coagulogram\n";
cout<<"\t\t>>7 : Blood urea nitrogen\n";
cout<<"\t\t>>0 : None\n";
int laboratory_exam;
cin>>laboratory_exam;
if(laboratory_exam==1){
strcpy(hos[i].laboratory_examination,"Hematology");
cout<<hos[i].laboratory_examination;

}
else if(laboratory_exam==2){

strcpy(hos[i].laboratory_examination,"Urine analysis");
cout<<hos[i].laboratory_examination ;

}
else if(laboratory_exam==3){

strcpy(hos[i].laboratory_examination,"stool");
cout<<hos[i].laboratory_examination;
}
else if(laboratory_exam==4){

strcpy(hos[i].laboratory_examination,"Gram stain");
cout<<hos[i].laboratory_examination;

}

else if(laboratory_exam==5){

strcpy(hos[i].laboratory_examination,"Blood sugar");
cout<<hos[i].laboratory_examination;

}

else if(laboratory_exam==6){

strcpy(hos[i].laboratory_examination,"Coagulogram");
cout<<hos[i].laboratory_examination;

}

else if(laboratory_exam==7){

strcpy(hos[i].laboratory_examination,"Blood urea nitrogen");
cout<<hos[i].laboratory_examination;

}


else if(laboratory_exam==0){

strcpy(hos[i].laboratory_examination,"None");
cout<<hos[i].laboratory_examination;
}

else{
cout<<"Make a correct choice\n";
goto lab;
}
//finding

finding:
cout<<"Finding Diagnosis:\n";
//out<<"\nFinding Diagnosis:";
cout<<"\t\t>>1 : Malaria\n";
cout<<"\t\t>>2 : TB\n";
cout<<"\t\t>>3 : HIV\n";
cout<<"\t\t>>4 : Malnutrition \n";
cout<<"\t\t>>5 : Diabetes\n";
cout<<"\t\t>>6 : Anemia\n";
cout<<"\t\t>>0 : None\n";

int diagnosis_no;
cin>>diagnosis_no;
if(diagnosis_no==1){

strcpy(hos[i].finding_diagnosis,"Malaria");
cout<<hos[i].finding_diagnosis;

}
else if(diagnosis_no==2){

strcpy(hos[i].finding_diagnosis,"TB");
cout<<hos[i].finding_diagnosis;
}
else if(diagnosis_no==3){

strcpy(hos[i].finding_diagnosis ,"HIV");
cout<<hos[i].finding_diagnosis;

}
else if(diagnosis_no==4){

strcpy(hos[i].finding_diagnosis,"Malnutrition");
cout<<hos[i].finding_diagnosis;

}
else if(diagnosis_no==5){

strcpy(hos[i].finding_diagnosis,"Diabetes");
cout<<hos[i].finding_diagnosis;

}
else if(diagnosis_no==6){

strcpy(hos[i].finding_diagnosis,"Anemia");
cout<<hos[i].finding_diagnosis;

}
else if(diagnosis_no==0){

strcpy(hos[i].finding_diagnosis,"None");
cout<<hos[i].finding_diagnosis;
}
else{

cout<<"Make a correct choice\n";
goto finding;

}

Result:
cout<<"Result of the finding :\n";
//out<<"\nResult of the finding:";
cout<<"\t\t>>1 : Plasmodium \n";
cout<<"\t\t>>2 : Tuberculosis bacteria \n";
cout<<"\t\t>>3 : HIV positive\n";
cout<<"\t\t>>4 : Malnutrition\n";
cout<<"\t\t>>5 : Glucose level\n";
cout<<"\t\t>>6 : Gram positive bacteria\n";
cout<<"\t\t>>7 : Clotting problems\n";
cout<<"\t\t>>0 : None\n";

//accepting result
int result;
cin>>result;

if(result==1){

strcpy(hos[i].result,"Plasmodium");
cout<<hos[i].result;

}
else if(result==2)
{
strcpy(hos[i].result,"Tuberculosis bacteria");
cout<<hos[i].result;
}
else if(result==3){

strcpy(hos[i].result,"HIV positive");
cout<<hos[i].result;

}
else if(result==4){

strcpy(hos[i].result,"Malnutrition");
cout<<hos[i].result;
}
else if(result==5){

strcpy(hos[i].result,"Glucose level");
cout<<hos[i].result;
}
else if(result==6){

strcpy(hos[i].result,"Gram positive bacteria");
cout<<hos[i].result;
}
else if(result==7){

strcpy(hos[i].result,"Clotting problems");
cout<<hos[i].result;
}
else if(result==0)
{
strcpy(hos[i].result,"None");
cout<<hos[i].result;
cout<<"error";
}
else
{
cout<<"Make a correct choice\n";
goto Result;
}
//cout<<"\n medication given to the patient:";
cout<<"\n Medication given to the patient:";
cout<<endl;
cin>>hos[i].medicine;
//cout<<hos[i].medicine;
cout<<endl;
cout<<"**********Appointment to patient**********";

//cout<<"\nAppointment to patient:";
cout<<endl;

//cout<<"If no appointment fill 0 0 0 to all fields\n";
appointment_year:
cout<<"\nAppointment Year :";
//cout<<"\nYear :";
cin>>hos[i].appointment_year;


if(hos[i].appointment_year<2022||hos[i].appointment_year>2024){
cout<<"Enter the proper format of year that is from 2022 to 2024 maximum\n";
goto appointment_year ;
}

//cout<<hos[i].appointment_year;
appointment_month:
cout<<"\nAppointment month :";
//cout<<endl;
//cout<<"\n month:";
cin>>hos[i].appointment_month;

if(hos[i].appointment_month<=1 && hos[i].appointment_year>12)
{
cout<<"Enter the proper format of month that is from 1 to 12 maximum\n";
goto appointment_month  ;
}

//cout<<hos[i].appointment_month;
appointment_date:
cout<<"\nAppointment Date:";
//cout<<endl;
//cout<<"\nDate:";
cin>>hos[i].appointment_date;
if(hos[i].appointment_date<1 && hos[i].appointment_date>31)
{
cout<<"Enter the proper format of date that is from 0 to 31 maximum\n";
goto appointment_date ;
}
//cout<<hos[i].appointment_date;

cout<<"Suggestion given to the patient "<<endl;
cout<<endl;
//cout<<"Suggestion given to the patient:"<<endl;

cin.getline(hos[i].suggestion,5000,'#');

cout<<hos[i].suggestion;

cout<<"\n========";

cout<<"Do you want to continue? Y/N \n";

cin>>key;

i++;

No_patient=i;

}while(key!='N' && key!='n');


//end of loop



/*out.open("CLINIC_REPORT");
out.close*/

return 0;

}



// searchng patient by id

int search_patient(){


int search_ID;
cout<<"\n\n A patient that have a card already \n\n";
cout<<"Search a patient history by his/her id number\n";
cout<<"Enter the ID number to be searched:";
cin>>search_ID;

for(int j=0;j<No_patient;j++){


if (hos[j].id==search_ID){

cout<<"======search Result====";
cout<<"ID_NO:"<<hos[j].id;
cout<<"\n Event Date:\n";
cout<<"Date:"<<hos[j].date;
cout<<"\n Month:"<<hos[j].month ;
cout<<"\n Year:"<<hos[j].year ;
cout<<"\n Name:"<<hos[j].fname ;
cout<<"\n Name:"<<hos[j].lname ;
cout<<"\n Age:"<<hos[j].age ;
cout<<"\n Sex:"<<hos[j].sex;
 cout<<"\n Address:"<<hos[j].address;
cout<<"\n Occupation:"<<hos[j].occupation ;
cout<<"\n Examination room:"<<hos[j].examination_room;
cout<<"\n Patient Location :"<<hos[j].in_out_patient;
cout<<"\n Laboratory examination:"<<hos[j].laboratory_examination;
cout<<"\n Finding Diagnosis:"<<hos[j].finding_diagnosis;
cout<<"\n Result of the finding:"<<hos[j].result;
cout<<"\n medication given to the patient:"<<hos[j].medicine;
cout<<"\n Appointment date given to the patient \n";
cout<<"Date:"<<hos[j].appointment_date;
cout<<"\n Month:"<<hos[j].appointment_month ;
cout<<"\nYear:"<<hos[j].appointment_year ;
cout<<"\n Suggestion given to the patient:\n";
cout<<hos[j].suggestion;
cout<<endl;

cout<<"=====End of suggestion====\n";
}


}

return 0;

}
//searching all patients function

int search_All_patient(){

ifstream in("CLINIC_REPORT.txt");


int hosp;

cout<<"\n\n A  patient that have a card already\n\n";
if(!in){

cout<<"Can not open CLINIC_REPORT file.\n";
return 1;


}

for(int j=0;j<No_patient;j++){

cout<<"======Search Result=======\n";
cout<<"ID_NO:"<<hos[j].id;
cout<<"\n Event Date:\n";
cout<<"Date:"<<hos[j].date ;
cout<<"\n Month:"<<hos[j].month ;
cout<<"\n Year:"<<hos[j].year ;
cout<<"\n Name:"<<hos[j].fname ;
cout<<"\n Name:"<<hos[j].lname ;
cout<<"\n Age:"<<hos[j].age ;
cout<<"\n Sex:"<<hos[j].sex;
cout<<"\n Address:"<<hos[j].address;
cout<<"\n Occupation:"<<hos[j].occupation ;
cout<<"\n Examination room:"<<hos[j].examination_room;
cout<<"\n Patient Location :"<<hos[j].in_out_patient;
cout<<"\n Laboratory examination:"<<hos[j].laboratory_examination;
cout<<"\n Finding Diagnosis:"<<hos[j].finding_diagnosis;
cout<<"\n Result of the finding:"<<hos[j].result;
cout<<"\n medication given to the patient:"<<hos[j].medicine;
cout<<"\n Appointment date given to the patient \n";
cout<<"Date:"<<hos[j].appointment_date;
cout<<"\n Month:"<<hos[j].appointment_month ;
cout<<"\n Year:"<<hos[j].appointment_year ;
cout<<"\n Suggestion given to the patient:\n";
cout<<hos[j].suggestion;
cout<<endl;
}
return 0;

}
