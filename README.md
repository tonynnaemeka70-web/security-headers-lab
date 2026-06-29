Security Headers Lab

A cybersecurity lab project demonstrating Nginx security header hardening with Docker.  
This project implements browser-side protections against common client-side attacks such as Clickjacking, MIME sniffing, and Cross-Site Scripting (XSS).



Repository Structure
- DOC/ Contains project documentation  
  - [PROJECT GUARD-POST_ AUTOMATED WEB HEADER HARDENINGt.pdf](./DOC/PROJECT%20GUARD-POST_%20AUTOMATED%20WEB%20HEADER%20HARDENINGt.pdf)  



Security Controls Implemented
- X-Frame-Options: DENY → Prevents Clickjacking  
- X-Content-Type-Options: nosniff → Blocks MIME-type sniffing  
- Content-Security-Policy: default-src 'self'Restricts unauthorized script execution  



 Lab Environment
- Host: VMware Workstation  
- OS: Ubuntu Linux  
- Container Platform: Docker  
- Web Server: Nginx  
- Validation Tools: `curl`, Firefox  



 Deployment Steps
1. Install Docker on Ubuntu Linux.  
2. Pull the official Nginx Docker image.  
3. Configure hardened security headers in `nginx.conf`.  
4. Deploy and run the container.  
5. Validate headers using `curl -I http://localhost:8080`.  



 Documentation
Full details of the project, including configuration files, validation screenshots, and security assessment, are available in the PDF under the [`DOC`](./DOC) folder:  
[Open Project Document](./DOC/PROJECT%20GUARD-POST_%20AUTOMATED%20WEB%20HEADER%20HARDENINGt.pdf)








