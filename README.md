#include<stdio.h>
int main(){
int ash;
int ds;        
double wil;                
printf("Please enter your :\n1-Average sleep hours\n2-Daily steps\n3-water intake in liters\n ");        
scanf("%d", &ash);
scanf("%d", &ds); 
scanf("%lf",&wil);         
 int hi=0;       
  if(ash<5){
       hi+=30;         
        }      
      else if (ash>=5&&ash<7){
        hi+=50; 
        }  
      else if (ash>=7&&ash<9){
        hi+=70;
        }  
      else {
        hi+=60;
        }  

  if(ds>8000){
    hi+=15;
  }
    else if(ds<=8000&&ds>=4000){
      hi+=5;
    }   
    else {
      hi-=10;
    }
    
  if(wil>=2){
     hi+=10;
  }  
    else{
      hi-=5;
    } 
  if(hi>=85){
    printf("excellent health");
  }
    else if(hi<=84&&hi>=70) {
       printf("good health");
    }
    else if(hi<=69&&hi>=50) {
       printf("average health");
    }
    else{
      printf("poor health");
    }
return 0;
}

