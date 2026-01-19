# Django Authentication Code Map.

## A custom authentication flow for complete user:
- User Sign up
- User Login
- OTP Verification
- Reset Password
- Update Password
- JWT Token Authentication
- Database-level lock for OTP abuse security
- Good for mid-level inspiration

## Improvements possible
- Need to follow the updated code file structure serializer per file
- Use Redis for OTP store - with proper locking.
- Or use the stateless OTP verification with proper rate limiting with the help of Redis.
- Use Proper HTML mail structure with a stateless password reset mechanism.
- Use Redis for proper email sending or mobile phone message sending with a dedicated queue setup.
- Use the stateless password update mechanism
- Use Redis or a DB for token blacklisting and write a cron job to clear all the blacklisted tokens so that the database remains efficient.
