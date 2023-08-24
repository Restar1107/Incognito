# Incognito
2023-2 CAU Incognito party


code rule
1. Do not write over 35~40 lines in one file
2. Place newline characters after the '{' symbol. 2.
3. All defined preprocessors are capitalized.
4. Use the `return` function instead of the `exit` function to prevent the file from being twisted.
5. Include "pch.h" to create a separate pch.h file for header files. (To prevent file from header twisted)

// exemple.c argv1 argv2

#include "pch.h"
#define HELLOLEN

void execute_exemple(char v1) {
  if(!memcmp(v1, "hello world", HELLOLEN)){ // instead of using `if (memcmp() == 0)`, use `if(!memcmp())`
    printf(" ------- same word ------- ");
  }
  else {
    for(;;) { // instead of using while(True), use for(;;)
      printf("id\t: %s", v1 > "hello world" ? "Upper case" : "Lower case");
      break;
    }
  }
}

int main(int argc, char* argv[]) {
  if (argc < 3) {
    fprintf(stderr, "There is Less arguments);
    return -1; // DO NOT USE `exit(1)`
  }
  printf("%s\n %s\n", argv[1], argv[2]);
  execute_exemple(argv[3]);
  return 0;
}

// pch.h

#include <stdio.h>
#include <Windows.h>




