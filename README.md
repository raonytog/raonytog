```c
#include <stdio.h> 
#include <stdlib.h>
#include <string.h>

typedef struct self{
    char name[6], role[17], mainLanguage[6], secondLanguage[6];
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
    printf("\nHi!, im %s, a Comp.Sci student in third semester at UFES\n", myself->name);
    printf("Current learning: C, Python, Java and Swift\n");
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
