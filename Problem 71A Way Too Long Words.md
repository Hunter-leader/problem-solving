Problem Link: https://codeforces.com/problemset/problem/71/A

```C
#include <stdio.h>
#include <string.h>

int main() {
    int n;
    scanf("%d", &n); // Read the number of words

    char word[101]; // Each word can be up to 100 characters long

    for (int i = 0; i < n; i++) {
        scanf("%s", word); // Read the word
        int len = strlen(word);

        if (len > 10) {
            // Print the abbreviation
            printf("%c%d%c\n", word[0], len - 2, word[len - 1]);
        } else {
            // Print the word as it is
            printf("%s\n", word);
        }
    }

    return 0;
}
```

