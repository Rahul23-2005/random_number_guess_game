# random_number_guess_game
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    // Initialize random number generator
    srand(time(0));

    // Generate random number between 1 and 100
    int randomNumber = (rand() % 100) + 1;
int no_of_guesses =0;
int guessed;
    // Print the random number
   // printf("Random number between 1 and 100: %d\n", randomNumber);
printf("Guess the number");
do
{
   printf("Guess the number");
   scanf("%d",&guessed);
   if(guessed > randomNumber){
    printf("Lower number please\n");
   }
   else if(randomNumber<guessed) {
    printf("Higher number please\n");
   }
   else{
    printf("congrats");
   }
   no_of_guesses++;
} while (guessed != randomNumber);

printf("You guessed the number in %d guesses",no_of_guesses);
    return 0;
}
