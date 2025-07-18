# security-engineer-interview-questions
The question list which I share on linkedin to prepare for security engineering jobs including scenario based questions.
# Security Engineer/ Application Security/ Information security Question List

1. You are a security engineer in a startup having customers which store a lot of sensitive info in the servers. How are you going to secure it and which cloud platform is best for it ? Additionally, what may be the best way for password storage? 
2. You are part of the application security team for a Fortune 500 company. It was recently found out that sensitive email communication has been leaked to the press. It is suspected to be an inside job. What steps would you deal to prevent insider threat and detect future incidents to a certain extent ? 
3. Your team deploys regular phishing attacks via email to make employees give out their personal details like passwords.
Now it's a running joke among CEO and other employees that phishing comes only via email and link clicks . This has embarrassed the CISO . How are you going to prove them wrong and surprise them with a different phishing technique( red team campaign ) this time around ?
4. Your website is sending cookies via set-cookie HTTP header. The web dev team have not set any same site attribute. 
In your previous org, 7 yrs back, the same scenario was observed and fixed. How is the browser going to treat requests as of today or you are going to flag it now too ?
5. You have developed a React application and computed the logic to generate high score for the particular user in client side. Suppose in this case, the user can manipulate the score value from 30 to 90 (max 100) by intercepting the post request to db . 
How can we send that highscore value to DB without the user being able to tamper with his original highscore or it is not all possible to prevent the manipulation via proxy ? 
6. What is QUIC Protocol and which HTTP version uses it ? 
7. What is the difference between localhost and 127.0.0.1 ?
8. What is Mutation XSS and how to prevent it ?
9. What is phtml ? What type of security flaws can arise in applications using it?
10. What is GRUB in Linux?
11. Why messages are encrypted but passwords are hashed ?
12. What is the use of Idempotency keys and why are they used in payment systems ?
13. What is a XHR request and also explain the readyState property.
14. As an Offensive security engineer, how can you use Exponential backoff method during a particular pentest? 
15. What would you suggest the Junior Backend Developer in your company who wants help in designing simple check/prevention to fix File path traversals attacks ?
16. A major fintech company's payment application, processing over 1 million transactions daily, recently experienced a security incident where unauthorized access was detected due to compromised authentication tokens. The investigation revealed that the token revocation system failed to properly invalidate tokens across all services, allowing attackers to continue using revoked tokens for up to 30 minutes after users logged out. How would you implement a proper token revocation system?
17. You are a senior security engineer at a company, and it was detected that a critical API endpoint on a subdomain is vulnerable due to a CORS misconfiguration. This endpoint handles sensitive user data. What top 3 actions or (more) would you take to address the CORS misconfiguration, and how would you ensure that the vulnerability is remediated without disrupting legitimate access?
18. You have a web application hosted on an EC2 instance in a public subnet. You need to configure security to allow only HTTP and HTTPS inbound traffic from the internet while permitting outbound traffic for essential services like DNS and S3. How would you design this setup using Security Groups and Network ACLs, and how would their stateful and stateless characteristics influence your approach? ( * this question is more about STATE than your understanding and less about how to configure *)
19. What does aws sts get-caller-identity command result in and what is it's use?
20. What does an Air Gap Environment mean and why is it used?
21. What is the benefit of CIS benchmarking ?
22. Are Kubernetes pods mutable or immutable by default ?
23. Explain wrap around method in low level programming? (hint: modular arithmetic)
24. You accidentally publicly share one AMI from your AWS account. The ami in itself is harmless with no sensitive api keys. Still, can the now public ami cause any financial bill for you or not if others start using it / deploying instances ?
25. You're inside a Kubernetes pod in an AWS EKS cluster. The pod has outbound internet access and no egress restrictions. You notice you can access http://169.254.169.254. What can you do as an attacker with this access?
26. In a real-time chat application that includes a typing indicator feature implemented via WebSockets, how would you approach securing this feature against potential Denial-of-Service (DoS) attacks? Describe how you would identify potential weaknesses, and outline your approach to detecting misuse, and maintaining the availability and integrity of the overall messaging infrastructure.
27. You got recently onboarded as Security Engineer Intern at a company. You’ve just joined as a Security Engineer Intern. In your first week, you receive a ticket from the SOC team about a suspicious activity alert: "An IAM user appears to have created new EC2 instances in a region we typically don’t use (ap-southeast-1)."
Your task is to investigate and confirm this activity and who performed it ? Which AWS service would you use to begin the investigation CloudTrail or CloudWatch and why?
28. Users receive a one-time access token (a long random string) via email which then opens a web interface. The access_tokens table stores only the token’s SHA-256 hash, expiration timestamp, and “used” flag. After six months, it has grown to hundreds of thousands of rows, most expired/used causing storage bloat. Occasionally you still need to verify which token a given user clicked (like "Which token did user XYZ use two weeks ago?"). As a security engineer, what retention policy would you implement for old tokens to keep the database lean yet preserve the ability to perform such forensic lookups?
29. You are reviewing a social networking application where users can upload a profile picture. The current implementation accepts JPEG and PNG files and stores them in an AWS S3 bucket, however, the security team recently discovered that a someone uploaded a disguised .php file, which executed due to a misconfigured image URL. As a Security Engineer, how would you secure the profile picture upload feature to prevent abuse such as file upload attacks, remote code execution, and data exfiltration?
30. Perform secure code review for the following terraform statefile . (see linkedin)
31. You're a Security Engineer at a company using multiple AWS regions. You've configured CloudTrail to log all management events across all regions, and you created an EventBridge rule in us-east-1 to trigger alerts on ConsoleLogin events. However, the rule isn't triggering for logins in other regions, even though those events appear in the CloudTrail logs. Why is this happening, and how would you modify the setup to ensure you catch ConsoleLogin events from all regions?


