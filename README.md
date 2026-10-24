# post-lab8
#include <stdio.h>

int main() {
int arr[2][3][4];
    int i ,j,total,pass=0,sec1=0,sec2=0,sec1best=0,sec2best=0,sec1high=0,
    sec2high=0;
    float avg1,avg2;
for( i=0;i<2;i++){
    for( j=0;j<3;j++){
           total=0;
        printf(" enter marks of 4 subjects for every section %d,student %d\t \n",i+1,j+1);
       for(int k=0;k<4;k++){
           scanf("%d",&arr[i][j][k]);
           total+=arr[i][j][k];
          
       }
        printf("\n total %d\n",total);
       int avg = total/4;
        printf("avg %d\n",avg);
        if(avg>=50){
            pass++;
        }
        if(i==0){
            sec1+=total;
           if(total>sec1high){
               sec1high=total;
               sec1best=j+1;
           }
        }
            else{
                sec2+=total;
                if(total>sec2high){
                    sec2high=total;
                    sec2best=j+1;
                }
            }
        }
        }
    
    avg1=sec1/12.0;
    avg2=sec2/12.0;
   
printf("%d\n",sec1best);
printf("%d\n",sec2best);
printf("%d\n",pass);
 if(avg1>avg2)  {
     printf("section1 has highest avg %f\n", avg1);
 } else if(avg2>avg1){
     printf("section2 has highest avg %f\n",avg2);
     }else{
     printf("both have identical avg %2f\n",avg1);
     return 0
     }

     # task 2 
     #include <stdio.h>
int main() {
int arr[2][3][4];
    int i,j,k,branch1=0,branch2=0,sale1=0,sale2=0,week1=0,week2=0;
    int weeklysale[4]={0};
 for(i=0;i<2;i++){
 for(j=0;j<3;j++){
     printf("enter 4 weeks sale of 3 products \n");
 for(k=0;k<4;k++){
     scanf("%d",&arr[i][j][k]);
 }
     }
 }
     for(i=0;i<2;i++){
 for(j=0;j<3;j++){
    int total=0;
 for(k=0;k<4;k++){
    total+=arr[i][j][k];
    weeklysale[k]+=arr[i][j][k];
 }
     printf("total %d\n",total);
     if(i==0){
         branch1+=total;
         if(sale1<total){
             sale1=total;
            }
         }else{
             branch2+=total;
         }if(sale2<total){
             sale2=total;
            
         
     }
     }
 }
    for(k=0;k<4;k++){
      if( weeklysale[k]>week1){
          week1=weeklysale[k];
      }
    }
         printf(" highest sale in branch1 %d",sale1);
         printf(" highest sale in branch1 %d",sale2);
         printf("highest sale of a week %d\n",week1);
         if(branch1>branch2){
             printf("branch1 has greater sales \n");
         }else if (branch1<branch2){
             printf("branch2 has greater sales\n ");
         }else{
             printf("both has same sales\n");
         }
    return 0;
}

# task 3


     # task 2
     
     }
    return 0;
}
