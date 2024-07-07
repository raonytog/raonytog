```c
#include <stdio.h> 
#include <stdlib.h>
#include <string.h>

#define MAX 20

typedef struct self{
    char name[MAX], role[MAX], mainLanguage[MAX], secondLanguage[MAX];
    int age;
} self;

self *__Init__ () {
    self *me = (self*) malloc(sizeof(self));
    me->age = 20;
    strcpy(me->name, "Raony");
    strcpy(me->role, "Comp.Sci student");
    strcpy(me->mainLanguage, "pt_BR");
    strcpy(me->secondLanguage, "en_US");
    return me;
}

void HeyThere (self *myself) {
    printf("\n-======================@==========================-\n");
    printf("Hi!, im a Comp.Sci student in third semester at UFES\n");
    printf("Also, I have 7 years of experience with Adobe PhotoShop\n");
    printf("Am I current learning: C (1y), Python(2y), Java(<1y) and Swift(<1y)");
    printf("\n-======================@==========================-\n");
}

void GoodBye (self *myself) {
    printf("\n-======================@==========================-\n");
    printf("Thanks for visiting my profile!\n");
    printf("See you soon, friend!\n");
    printf("-======================@==========================-\n");
    free(myself);
}

int main () {
    self *myself = __Init__();
    HeyThere(myself);
    GoodBye(myself);
    return 0;
}
```

<div style="display: flex; justify-content: center; align-items: center;">
  <img width="600" height="200" src="https://github-readme-stats.vercel.app/api?username=raonytog&show_icons=true&theme=github_dark">
  <img width="400" height="200" src="https://github-readme-stats.vercel.app/api/top-langs/?username=raonytog&size_weight=0.0005&count_weight=0.3&layout=compact&theme=github_dark">
</div>


<div id="header" align="center">
  <img src="https://komarev.com/ghpvc/?username=raonytog&style=for-the-badge&color=blue" alt=""/>
</div>




