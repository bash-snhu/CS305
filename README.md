# CS305
## Reflection

- Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?

Artemis Financial is a financial institution that wished to serve a secure web application utilizing Spring. Through that web application, they wished to safely encrypt important archived financial records as well as generate a checksum to be able to verify uncorrupted files.

- What did you do very well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?

Software security is paramount. A single security breach can irrevocably damage a company’s reputation, but more importantly its customers, who own that data. Adding software security ensures that its important resources cannot be accessed by malicious parties. To ensure the client’s security, I did a manual check of their existing code, an OWASP dependency check, integrated https connectivity through a generated certificate, and added checksum functionality.

- What part of the vulnerability assessment was challenging or helpful to you?

Because I haven’t worked on large projects used by many users, it was useful to look at our assignments through the frame of public access. The API, Cryptography, and Client/Server aspects were illuminating to me. Dependency checking can ensure that APIs and dependencies don’t have known vulnerabilities. Cryptography is not as difficult to integrate as I imagined, though I would like to see how it is introduced at scale and in a production environment.

- How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

As the software evolves, dependency vulnerability checks should be run to ensure that new vulnerabilities are managed as they crop up. Increased layers of security should be planned and built into the system with proper planning. Patched or piecemeal security can introduce weaknesses and flaws.

- How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?

I did a manual verification to check for obvious issues with the code. New vulnerabilities were assessed using the OWASP dependency check.

- What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?

Dependency checking is a good tool for ensuring that your program doesn’t have any blatant, known vulnerabilities. Enforcing HTTPs connections via certificate authentication ensures that users are able to connect to the service without risk. These will be useful to integrate into future projects.

- Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?

The Project Two assignment committed to this distro is a good example of my attention to detail and ability to make nuanced assessments based on the user’s functional and nonfunctional requirements.
