```c
#include <stdio.h> 
#include <stdlib.h>
#include <string.h>

#define MAX 20

typedef struct self{
    char name[MAX], role[MAX], mainLanguage[MAX], secondLanguage[MAX];
    int age;
} self;

self *InitMyself () {
    self *me = (self*) malloc(sizeof(self));
    me->age = 20;
    strcpy(me->name, "Raony");
    strcpy(me->role, "Comp.Sci student");
    strcpy(me->mainLanguage, "pt_BR");
    strcpy(me->secondLanguage, "en_US");
    return me;
}

void HeyThere (self *myself) {
    printf("\n-======================@==========================-");
    printf("\nHi!, im a Comp.Sci student in third semester at UFES\n");
    printf("Also, I have 3 years of experience with Adobe PhotoShop");
    printf("Am I current learning: C (1yo), Python(2yo), Java(-1yo) and Swift(-1yo)\n");
    printf("\n-======================@==========================-");
}

void GoodBye (self *myself) {
    printf("\n-======================@==========================-");
    printf("Thanks for visiting my profile!\n");
    printf("See you soon, friend!\n");
    printf("-======================@==========================-\n");
    free(myself);
}

int main () {
    self *myself = InitMyself();
    HeyThere(myself);
    GoodBye(myself);
    return 0;
}
```
