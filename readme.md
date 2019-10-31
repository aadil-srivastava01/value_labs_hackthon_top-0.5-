## About Problem Statement:
 - Genre: NLP
 - Problem Type: Contextual Semantic Similarity, Auto generate Text-based answers

**Submission Format**:
 - You need to generate upto 3 distractors for each Question-Answer combination
 - Each distractor is a string
 - The 3 distractors/strings need to be separated with a comma (,)
 - Each value in Results.csv's distractor column will contain the distractors as follows:
	distractor_for_QnA_1 = "distractor1","distractor2","distractor3"

**About the Evaluation Parameter**:
 - All distractor values for 1 question-answer will be converted into a vector form
 - 1 vector gets generated for submitted distractors and 1 vector is generated for truth value
 - cosine_similarity between these 2 vectors is evaluated
 - Similarly, cosine_similarity gets evaluated for all the question-answer combinations
 - Score of your submitted prediction file = mean ( cosine_similarity between distractor vectors for each entry in test.csv)

##Final Model

Used [GPT-2](https://openai.com/blog/better-language-models/) Small and finetuned it on the test set so as to generate the output.
More information is available on this [Link]( https://minimaxir.com/2019/09/howto-gpt2/)

This final model helped me to land in top 0.5% in the hackthon[on Hackerearth](https://www.hackerearth.com/challenges/hiring/valuelabs-ml-hiring-2019/) thus helping me getting shortlisted. 

