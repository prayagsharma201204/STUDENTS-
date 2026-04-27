#include<stdio.h>

void main()
{
    char name[20], rollNo[5];
    int hindi, english, maths;
    float total, percentage;
    printf("Enter Roll No -- ");
    scanf("%s", &rollNo);
    printf("Enter Name -- ");
    scanf("%s", &name);
    printf("Enter Hindi Marks -- ");
    scanf("%d", &hindi);
    printf("Enter English Marks -- ");
    scanf("%d", &english);
    printf("Enter Maths Marks -- ");
    scanf("%d", &maths);

    total = hindi + english + maths;
    percentage = (total * 100) / 300;
    system("cls");
    printf("Students details are :- \n\n");
    printf("Roll No -- %s\n\n", rollNo);
    printf("Name -- %s\n\n", name);
    printf("Hindi -- %d\n\n", hindi);
    printf("English -- %d\n\n", english);
    printf("Maths -- %d\n\n", maths);
    printf("Total -- %0.2f / 300\n\n", total);
    printf("Percentage -- %.2f%%\n\n", percentage);

    if (percentage >= 60) printf("First Division\n");
    else if (percentage >= 48) printf("Second Division\n");
    else if (percentage >= 36) printf("Third Division\n");
    else printf("Fail\n");
}
