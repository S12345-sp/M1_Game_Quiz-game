#include "unity.h"

#include <quiz.h>

/* Modify these two lines according to the project */

#include <quiz game.h>
  
#define PROJECT_NAME    "quiz-game"

/* Prototypes for all the test functions */
  
void show_record(void);


/* Required by the unity test framework */
  
void reset_score(){}
  
/* Required by the unity test framework */
  
void help(){}

/* Start of the application test */
  
int main()
  
{
  
/* Initiate the Unity Test Framework */
  
  UNITY_BEGIN();

/* Run Test functions */
  
  RUN_TEST(test_quiz);


  /* Close the Unity Test Framework */
  
  return UNITY_END();
}
  

/* Write all the test functions */
  
void test_quiz(void) {
  
  TEST_ASSERT_EQUAL(1, open(show.dat));
  
  TEST_ASSERT_EQUAL(2, open(record.dat));
  
  TEST_ASSERT_EQUAL(3, open(score.dat));
  
 
    /* Dummy fail*/
  
  // TEST_ASSERT_EQUAL(0, file does not exist);
  
}
