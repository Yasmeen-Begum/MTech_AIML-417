

1.Creating a file contains the elements size of the array more than 1000.
#include <stdio.h>
#include <stdlib.h>
int main(){
int arr[1200];
FILE *fptr;
int i=0,n;
int str;
fptr = fopen("inputFile1.txt", "w");
if(fptr == NULL){
printf("ERROR Creating File!");
exit(1);
}
while(i<1000){
fprintf(fptr,"%d \t",rand()% 1000);
i++;}
fprintf(fptr,"%d\t",arr[i]);
printf("file created succesfully");
fclose(fptr);
fptr = fopen("inputFile1.txt", "r");
printf("\n The content of the file %s is :\n",fptr);
str = fgetc(fptr);
while(str != EOF) {
printf ("%c", str);
str = fgetc(fptr);
}
fclose(fptr);
return 0;
}
output:
![Screenshot (3151)](https://user-images.githubusercontent.com/91931504/207857343-977e4d82-fc47-4b29-8652-201d08aa1c63.png)



