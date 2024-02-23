```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

typedef struct self{
    char name[10], role[20], mainLanguage[10], secondLanguage[10];
    int age;
} self;

self * InitMyself () {
    self * me = (self *) malloc(sizeof(self));
    me->age = 19;
    strcpy(me->name, "Raony");
    strcpy(me->role, "Comp.Sci student");
    strcpy(me->mainLanguage, "pt_BR");
    strcpy(me->secondLanguage, "en_US");
    return me;
}

void HeyThere (self * myself) {
    printf("\n-======================@==========================-");
    printf("\nHi!, im %s, a Comp.Sci student at third semester\n", myself->name);
    printf("I'm learning:\n");
    printf("* C\n");    printf("* Python\n");    printf("* Java\n");
    printf("\nThanks for visiting my profile!\n");
}

void GoodBye (self * myself) {
    printf("See you soon, friend!\n");
    printf("-======================@==========================-\n");
    free(myself);
}

int main () {
    self * myself = InitMyself();
    HeyThere(myself);
    GoodBye(myself);
    return 0;
}
```

This is probably unnecessary big
