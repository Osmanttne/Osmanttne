- 👋 Hi, I’m @Osmanttne
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Osmanttne/Osmanttne is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
using System;

namespace tt
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}
#include <stdio.h>

void checkPrimeNumber();

int main()
{
    checkPrimeNumber();    // argument is not passed
    return 0;
}

// return type is void meaning doesn't return any value
void checkPrimeNumber()
{
    int n, i, flag = 0;

    printf("Enter a positive integer: ");
    scanf("%d", &n);

    for (i = 2; i <= n / 2; ++i)
    {
        if (n % i == 0)
        {
            flag = 1;
        }
    }
    if (flag == 1)
        printf("%d is not a prime number.", n);
    else
        printf("%d is a prime number.", n);
}
#include <stdio.h>
int getInteger();

int main()
{
    int n, i, flag = 0;

    // no argument is passed
    n = getInteger();

    for (i = 2; i <= n / 2; ++i)
    {
        if (n % i == 0)
        {
            flag = 1;
            break;
        }
    }

    if (flag == 1)
        printf("%d is not a prime number.", n);
    else
        printf("%d is a prime number.", n);

    return 0;
}

// returns integer entered by the user
int getInteger()
{
    int n;

    printf("Enter a positive integer: ");
    scanf("%d", &n);

    return n;
}
#include <stdio.h>
void checkPrimeAndDisplay(int n);

int main()
{
    int n;

    printf("Enter a positive integer: ");
    scanf("%d", &n);

    // n is passed to the function
    checkPrimeAndDisplay(n);

    return 0;
}

// return type is void meaning doesn't return any value
void checkPrimeAndDisplay(int n)
{
    int i, flag = 0;

    for (i = 2; i <= n / 2; ++i)
    {
        if (n % i == 0)
        {
            flag = 1;
            break;
        }
    }
    if (flag == 1)
        printf("%d is not a prime number.", n);
    else
        printf("%d is a prime number.", n);
}
#include <stdio.h>
int checkPrimeNumber(int n);

int main()
{
    int n, flag;

    printf("Enter a positive integer: ");
    scanf("%d", &n);

    // n is passed to the checkPrimeNumber() function
    // the returned value is assigned to the flag variable
    flag = checkPrimeNumber(n);

    if (flag == 1)
        printf("%d is not a prime number", n);
    else
        printf("%d is a prime number", n);

    return 0;
}
h
// int is returned from the function
int checkPrimeNumber(int n)
{
    int i;

    for (i = 2; i <= n / 2; ++i)
    {
        if (n % i == 0)
            return 1;
    }

    return 0;
}
return  0
    return 1;
for (if=1 2> OverflowException)
            void setup 
    void loop 
    for (if 1=2> Overflowexeption )=?
    int configuration
    include
     include <selim serez
       else HashCode async s4a databace 
        
     if (HashCode rf
        else (EventHandler)
       delay (1000)
  
    where include trig 
   where
   selim hello world where
 #include <stdio.h>
#include <stdlib.h>

int main()
{
    int num;
    FILE* fptr;

    // use appropriate location if you are using MacOS or Linux
    fptr = fopen("C:\\program.txt", "w");

    if (fptr == NULL)
    {
        printf("Error!");
        exit(1);
    }

    printf("Enter num: ");
    scanf("%d", &num);

    fprintf(fptr, "%d", num);
    fclose(fptr);

    return 0;
},
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int num;
    FILE* fptr;

    if ((fptr = fopen("C:\\program.txt", "r")) == NULL)
    {
        printf("Error! opening file");

        // Program exits if the file pointer returns NULL.
        exit(1);
    }

    fscanf(fptr, "%d", &num);

    printf("Value of n=%d", num);
    fclose(fptr);

    return 0;
}
#include <stdio.h>
#include <stdlib.h>

struct threeNum
{
    int n1, n2, n3;
};

int main()
{
    int n;
   struct threeNum num;
FILE* fptr;

if ((fptr = fopen("C:\\program.bin", "wb")) == NULL)
{
    printf("Error! opening file");

    // Program exits if the file pointer returns NULL.
    exit(1);
}

for (n = 1; n < 5; ++n)
{
    num.n1 = n;
    num.n2 = 5 * n;
    num.n3 = 5 * n + 1;
    fwrite(&num, sizeof(struct threeNum), 1, fptr); 
   }
   fclose(fptr);

return 0;
}
#include <stdio.h>
#include <stdlib.h>

struct threeNum
{
    int n1, n2, n3;
};

int main()
{
    int n;
   struct threeNum num;
FILE* fptr;

if ((fptr = fopen("C:\\program.bin", "rb")) == NULL)
{
    printf("Error! opening file");

    // Program exits if the file pointer returns NULL.
    exit(1);
}

for (n = 1; n < 5; ++n)
{
    fread(&num, sizeof(struct threeNum), 1, fptr);
printf("n1: %d\tn2: %d\tn3: %d", num.n1, num.n2, num.n3);
   }
   fclose(fptr);

return 0;
}
#include <stdio.h>
#include <stdlib.h>

struct threeNum
{
    int n1, n2, n3;
};

int main()
{
    int n;
   struct threeNum num;
FILE* fptr;

if ((fptr = fopen("C:\\program.bin", "rb")) == NULL)
{
    printf("Error! opening file");

    // Program exits if the file pointer returns NULL.
    exit(1);
}

// Moves the cursor to the end of the file
fseek(fptr, -sizeof(struct threeNum), SEEK_END);

for (n = 1; n < 5; ++n)
{
    fread(&num, sizeof(struct threeNum), 1, fptr);
printf("n1: %d\tn2: %d\tn3: %d\n", num.n1, num.n2, num.n3);
fseek(fptr, -2 * sizeof(struct threeNum), SEEK_CUR);
   }
   fclose(fptr);

return 0;
}
include < stdio.h >
int main()
{
    char name[50];
    int marks, i, num;

    printf("Enter number of students: ");
    scanf("%d", &num);

    FILE* fptr;
    fptr = (fopen("C:\\student.txt", "w"));
    if (fptr == NULL)
    {
        printf("Error!");
        exit(1);
    }

    for (i = 0; i < num; ++i)
    {
        printf("For student%d\nEnter name: ", i + 1);
        scanf("%s", name);

        printf("Enter marks: ");
        scanf("%d", &marks);

        fprintf(fptr, "\nName: %s \nMarks=%d \n", name, marks);
    }

    fclose(fptr);
    return 0;
# include <stdio.h>
    int main()
    {
        char name[50];
        int marks, i, num;

        printf("Enter number of students:s ");
        scanf("%d", &num);

        FILE* fptr;
        fptr = (fopen("C:\\student.txt", "a"));
        if (fptr == NULL)
        {
            printf("Error!");
            exit(1);
        }

        for (i = 0; i < num; ++i)
        {
            printf("For student%d\nEnter name: ", i + 1);
            scanf("%s", name);

            printf("Enter marks: ");
            scanf("%d", &marks);

            fprintf(fptr, "\nName: %s \nMarks=%d \n", name, marks);
        }

        fclose(fptr);
        return 0;
    }
    #include <stdio.h>
struct student
{
    char name[50];
    int height;
};
int main()
{
    struct student stud1[5], stud2[5];
FILE* fptr;
int i;

fptr = fopen("file.txt", "wb");
for (i = 0; i < 5; ++i)
{
    fflush(stdin);
    printf("Enter name: ");
    gets(stud1[i].name);

    printf("Enter height: ");
    scanf("%d", &stud1[i].height);
}

fwrite(stud1, sizeof(stud1), 1, fptr);
fclose(fptr);

fptr = fopen("file.txt", "rb");
fread(stud2, sizeof(stud2), 1, fptr);
for (i = 0; i < 5; ++i)
{
    printf("Name: %s\nHeight: %d", stud2[i].name, stud2[i].height);
}
fclose(fptr);
}
printlnf 
    printlnf= fopen (ParamArrayAttribute)

    fwrite (stud1 ) sizeof (StringComparer)



















