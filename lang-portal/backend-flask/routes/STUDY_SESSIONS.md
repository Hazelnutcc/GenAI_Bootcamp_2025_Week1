# The two missing endpoints required by the challenge:

## 1. POST /study_sessions
- Creates a new study session
- Requires group_id and study_activity_id in the request body
- Validates that both group and study activity exist
- Returns the created session details

## 2. POST /study_sessions/:id/review
- Logs a review attempt for a word in a study session
- Requires word_id and correct in the request body
- Validates that both session and word exist
- Returns the created review details

### Both endpoints include:
- Input validation
- Error handling
- Proper HTTP status codes
- Meaningful response messages
- Database transaction management
