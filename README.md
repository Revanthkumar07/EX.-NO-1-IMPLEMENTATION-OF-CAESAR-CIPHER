# EX. NO: 1(A) : IMPLEMENTATION OF CAESAR CIPHER
## NAME:VESHWANTH.
## REG NO:212224230300
## AIM:
To implement the simple substitution technique named Caesar cipher using C language.

## ALOGORITHM:

STEP-1: Read the plain text from the user.

STEP-2: Read the key value from the user.

STEP-3: If the key is positive then encrypt the text by adding the key with each character in the plain text.

STEP-4: Else subtract the key from the plain text.

STEP-5: Display the cipher text obtained above.

## PROGRAM:
    #include <stdio.h>
    void encryptcaesar(char text[],int key){
      for(int i=0; text[i]!='\0'; i++){
        if(text[i]>= 'a' && text[i] <='z'){
          text[i]=(text[i] - 'a' + key) % 26 + 'a';
        } else if (text[i] >= 'A' && text[i] <= 'Z'){
            text[i] = (text[i]- 'A' + key) % 26 + 'A';
        }
        
      }
    }
    int main(){
      char text[100];
      
      gets(text);
      
      printf("The Original Text is :%s\n",text);
      
      int key;
      
      scanf("%d",&key);
      
      printf("The Key value is :%d\n",key);
      
      encryptcaesar(text,key);
      
      printf("The Encrypted Text Using Caeser Cipher is : %s\n",text);
      
      return 0;
    }
## OUTPUT:

<img width="628" height="163" alt="image" src="https://github.com/user-attachments/assets/09489f52-a817-4188-b8f8-d060cdf5076b" />

## RESULT :
 Thus the implementation of ceasar cipher had been executed successfully.
