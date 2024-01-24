<p align="center">
  <img src="./github-header-image.png" alt="Header">
</p>

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

typedef struct self{
    char name[10], role[20], mainSpokenLanguage[10], secondSpokenLanguage[10];
    int age;
} self;

self * InitMyself () {
    self * me = (self *) malloc(sizeof(self));
    me->age = 19;
    strcpy(me->name, "Raony");
    strcpy(me->role, "Comp.Sci student");
    strcpy(me->mainSpokenLanguage, "pt_BR");
    strcpy(me->secondSpokenLanguage, "en_US");
    return me;
}

void HeyThere (self * myself) {
    printf("\n-======================@==========================-");
    printf("\nHi!, im %s, a Comp.Sci student at third semester\n", myself->name);
    printf("I'm learning new languages:\n");
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

I'm a 19yo Computer Science student at Universidade Federal do Espírito Santo, in Brazil. Also, i'm at the third semester and learning the C, Pyhton and Java!



