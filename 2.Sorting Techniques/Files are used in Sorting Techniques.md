

1.Creating a file contains the elements size of the array more than 1000.

#include <stdio.h>

#include <stdlib.h>

int main(){

int  arr[1200];

FILE   *fptr;

int    i=0,n;

int    str;

fptr = fopen("inputFile1.txt", "w");

if(fptr == NULL){

printf("ERROR Creating File!");

exit(1);

}

while(i<1000){

fprintf(fptr,"%d \t",rand()% 1000);

i++;

}

fprintf(fptr,"%d\t",arr[i]);

printf("file created succesfully");

fclose(fptr);

fptr = fopen("inputFile1.txt", "r");  

printf("\n The content of the file %s is  :\n",fptr);

str = fgetc(fptr);

while(str != EOF)	{

printf ("%c", str);

str = fgetc(fptr);

}

fclose(fptr);

return 0;

}
	
output:

![Screenshot (3152)](https://user-images.githubusercontent.com/91931504/207869104-2fa5caca-50c1-4c23-931a-07c168b28f6b.png)

inputFile.txt
![Screenshot (3154)](https://user-images.githubusercontent.com/91931504/207870330-1db59234-ad8b-46aa-af92-d2d8a0eb9bfb.png)



