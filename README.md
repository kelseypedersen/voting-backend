# voting-backend

#Schema

Model
Question
- text (required)(string)
- user_id (not required)(string)
- nickname (not required)(string)
- created_date(date)
- expiration_date (required) - to make questions expire for next meeting(date)
- votes_id(int)

Answer
- question_id(int)
- user_id (not required)(int)
- nickname (not required)(string)

User
- name (not required)(string)

Votes
- question_id (#)
- count (int)

# Views
MVP
1. Shows all questions
- For all questions: 
  - ordered by highest vote count to lowest vote count
- For each question: 
  - click to see associated answers (index.html)
  - new answer form to question
  - upvote & downvote buttons - vote automatically updates the vote count
  - display vote count total
2. Add new question form (new.html)

Future
- Edit question, only if you created it (no new page)
- Delete question, only if you created it (no new page)


