# student-performance
#include <stdio.h>
int mains();
int condition();
int forr();
int main() {
   mains();
   condition();
   forr();
}
// basic program.
int mains(){
    printf("today is the result day");
    return 0;
}
//conditional program
int condition() {
    int i;
    char charr;  
    do {
        printf("\nEnter your marks out of 100: ");
        scanf("%d", &i);
        if (i >= 0 && i<=30) {
            printf("you have failed the test\n");
        }
        else if (i>=21 && i<=100) {
            printf("You have passed the test\n");
        } 
        else {
            printf("please check your marks\n");
        }
        printf("\nDo you want to continue? (y/n): ");
        getchar();  
        charr = getchar();  
 } while (charr == 'y' || charr == 'Y'); 
    return 0; 
}
int forr(){
    int i;
    printf("\n enter your roll no: ");
    scanf("%d", &i);
    for(i=1;i<=1;i++){
    int rating;
            printf("Enter your grade from the marksheet (1-5): ");
            scanf("%d",&rating);
            switch (rating) {
                case 1: 
                      printf("excellent performance\n"); 
                      break;
                case 2:
                       printf("good performance\n");
                       break;
                case 3: 
                       printf("better than last result\n");
                       break;
                case 4:
                       printf("you are trying your best\n");
                       break;
                case 5:
                       printf("can do even better\n"); 
                       break;
                default: 
                        printf("not performed well\n"); 
                        break;
     }
  }
}
