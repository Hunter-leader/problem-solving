Problem Link: https://codeforces.com/problemset/problem/59/A

```C
#include <stdio.h>
#include <string.h>
#include <ctype.h>

int main() {
    char s[101]; 
    scanf("%s", s); 

    int upper = 0, lower = 0;
    int len = strlen(s);

    
    for (int i = 0; i < len; i++) {
        if (isupper(s[i])) {
            upper++;
        } else {
            lower++;
        }
    }

    
    if (upper > lower) {
        for (int i = 0; i < len; i++) {
            s[i] = toupper(s[i]);
        }
    } else {
        for (int i = 0; i < len; i++) {
            s[i] = tolower(s[i]);
        }
    }

    printf("%s\n", s); 
    return 0;
}

```
