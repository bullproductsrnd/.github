## Type of Change
- [ ] Bug fix (non-breaking change which fixes an issue)
- [ ] New feature (non-breaking change which adds functionality)
- [ ] Breaking change (fix or feature that would cause existing functionality to not work as expected)
- [ ] Documentation update

## Pre-Submission Checklist
- [ ] My code follows the style guidelines of this project
- [ ] I have performed a self-review of my own code
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] My changes generate no new warnings
- [ ] All tests pass (`eg.: npm run test`)
- [ ] Lint checks pass (`eg.: npm run lint`)
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] New and existing unit tests pass locally with my changes
- [ ] No sensitive data in commits

## Problem
*The current user authentication system doesn't support social login, causing friction during user onboarding. We're seeing a 40% drop-off rate at the registration step.*

Related ticket: *Link to any related issues or tickets. eg.: AUTH-123*

## Solution
*Provide a brief description of the changes introduced by this pull request.*
*Implemented OAuth2 authentication flow with Google:*
*- Added OAuth2 middleware for handling Google authentication*
*- Created new user profile mapping logic*
*- Implemented session management for social login*

## Technical Details
*- Uses passport-google-oauth20 for authentication*
*- Added new database fields: googleId, socialProfile*
*- Modified user model to support multiple auth methods*

## Testing
*1. Click "Login with Google" button*
*2. Authorize test application*
*3. Verify successful redirect to dashboard*
*4. Check user profile contains Google data*

## Configuration
*New environment variables required:*
*- GOOGLE_CLIENT_ID*
*- GOOGLE_CLIENT_SECRET*
*- OAUTH_CALLBACK_URL*

## Screenshots
*Add screenshots to help explain the changes in this pull request.*

## Additional Notes
*Any additional information that might be useful for the reviewer.*
