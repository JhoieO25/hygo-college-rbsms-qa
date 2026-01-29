# BUG_GRADE_01 — System Allows Submission of Invalid Score Values Greater Than 100%

## Summary
The Grades API allows submission and persistence of invalid score values greater than 100%, resulting in incorrect academic records being saved and displayed in the UI.

## Environment
- Application: HyGo College Portal  
- Module: Results 
- User Role: Teacher  
- Browser: Chrome 144.0.7559.60  
- Operating System: Windows 10  
- API Endpoint: `POST /api/teacher/results`  

## Preconditions
- Teacher account exists and is logged in successfully.  
- Student and subject records exist in the system.  
- Teacher has permission to upload or update results.  
- A valid JWT token is available for API authentication.  

## Steps to Reproduce (API)
1. Log in via the API and obtain a valid JWT token.  
2. Send a `POST` request to `/api/teacher/results` with the following payload:  

```json
{
  "studentId": 33,
  "subjectId": 2,
  "term": "FIRST_TERM",
  "academicYear": "2025",
  "subjectCode": "MTH101",
  "subjectScores": [
    {
      "subjectId": 2,
      "subjectName": "Mathematics",
      "subjectCode": "MTH101",
      "score": 101.00,
      "grade": "B"
    }
  ]
}

3. Submit the request.
4. Open the UI at /teacher/results and view the saved record.

## Expected Result
API should reject the request with 400 Bad Request (or 422 Unprocessable Entity). Validation error message such as: "Score must be between 0 and 100."
and score shouldn't be saved.

## Actual Result
API returns 200 OK. Record is successfully saved.
