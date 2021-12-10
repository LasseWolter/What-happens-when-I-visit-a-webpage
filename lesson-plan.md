# Lesson Plan

## Objectives

The main learning objective is for students to understand the process behind web-browsing. This includes:

- Understanding which components are involved
- Understanding the unique role/function that each component has
- Understanding the interaction between these components

## Requirements

This is an unplugged activity with a brief introduction presentation. The presentation itself isn't enough to cover all the background knowledge required.
Thus, the following topics should have been covered before:
_(Note: This is not an exhaustive list and further depends on the level of depth at which this activity is carried out)_

- Basic understanding of networks: Different Computers connected to one another which allows them to communicate
- What is an IP?
- What is a domain? What are the different parts of a domain?
- What is a server?

## Introduction

Use the slides provided to give a brief introduction.
The diagram and interactions visualised in the slides can be use to recap prior knowledge together with the students.

# Role Play

## Roles:

1. DNS server: I have the mappings from domain names to IP addresses
2. User: I click on the link and want to check out the webpage
3. Web-Server: Computer that is running the website
4. Browser: I take the input from the user and do all the work for her/him...
5. Internet Connection: deliver request between different components

#### Extension: Roles with Codenames

Codenames can be used with more advanced students to illustrate that the components actually only know parts of the whole system. E.g. the user doesn't know the webserver, nor does he know it's IP address. He doesn't have to know these things to successfully access a website.

- DNS -> Zerbra98
- User -> Elephant49
- Web-Server -> Bird105
- Browser -> Tiger123
- Internet Connection -> Unicorn357

## Materials for different roles

Each role gets an instructions sheet and a set of materials specific to its role.

1. _DNS Server_

- instruction sheet
- Mappings from domain names to ip addresses
  - include the domain of the target website plus some other domains
    - such that an actual look up is needed
    - the ip addresses can be made up but should match the standard format (see dns-records.txt for examples)
    - the domain names are ideally once that students recognise

2. _User_

- instruction sheet
- URL of the website(s) to visit
  - written on a paper slip
  - _Note_: An example of a message containing the URL is given in the User materials. Embedding the URL in a message makes it closer to a real-world situation.

3. _Web-Server_

- instruction sheet
- A labeled printout of the HTML code representing the webpage and some other labeled HTML printouts representing the subpages of the website.
  - such that the student has to look for the correct page to return
  - _extension:_ for more advanced students one could omit the labels such that they have to interpret the HTML code
  - _simplification:_ The Web-Server has labeled printouts of the website and some of its subpages in already readable format.
  - _Note_: An example file as picture (.png) and text (.txt) is given in the Web-Server materials. Need to be adjusted to suit the lesson.

4. _Browser_

- instruction sheet
- (no extra material)

5. _Internet Connection_:

- instruction sheet
- (no extra material)

## Process

**Introduction:**
Explain that all components are fixed except for the Internet Connection and the user. Possibly ask all fixed components to sit down such that it's more obvious that only the User and the Internet Connection can move.

1. User goes to browser and gives him/her the URL (as a message)

---

2. Browser gets domain from URL (strips away protocol part, directory-path, subdomain, etc.)
3. Browser writes a message with the domain name, asking for the corresponding IP.
4. Browser asks Internet Connection to come to him/her (the Browser can't move)
5. Browser addresses the message to the DNS and gives it to the Internet connection

---

6. Internet Connection delivers message to the DNS.

---

7. DNS looks up the IP Address for this domain
8. DNS writes a message with IP address and addresses it to the browser
9. DNS ask the Internet Connection to come over and hands him/her the message.

- _simplification (applies to all message-sending):_ Addressing it to the receiver (e.g. the browser) only works if the sender and receiver are both written on each message. To make it a bit easier the basic instructions state that message is handed to the Internet Connection with the request to send it back to where it came from.

---

10. Internet Connection delivers the message back to the Browser.

---

11. Browser writes a message asking for the website content of the main page and addresses is to the IP address it just received.
12. Browser asks Internet Connection to come over and hands him/her the message.

---

13. Internet Connection delivers message to the Web-Server.

---

14. The message reaches the server
15. The Web-Server and looks for the corresponding webpage-code
16. The Web-Server addresses this page (with the webpage-code) to the Browser
17. The Web-Server calls the Internet Connection over and hands him/her the message.

---

18. Internet Connection delivers message to the Browser.

---

19. the browser transforms the message into human readable webpage

- this could be done by going to the teacher who is the 'HTML-converter' and has the
  corresponding webpage printed out
- _simplification:_ the webpage is already returned in readable format by the server
  - this would mean that the materials of the server have to be changed accordingly

20. The Browser calls the user and hands him the readable webpage

---

21. The browser calls the user over and hands him/her the webpage
