# Back-End Interview Topics

This repository contains a list of Back-End interview topics that I had to review, or want to deepen.

Feel free to contribute, it would be highly appreciated!

## <a name="toc">Table of Contents</a>

- [Programming Languages](#languages)
  - [JavaScript](#javascript)
- [Object Oriented Programming (OOP)](#oop)
- [Networking](#networking)
- [Architectures and Design Patterns](#architecture):
  - [Mircoservices](#microservices)
- [Security](#security)
- [Git](#git)

### <a name="languages">Programming Languages</a>

- <a name="javascript">JavaScript</a>:

    - What are the programming paradigms supported by JavaScript?
    - What is the difference between classical inheritance and prototypal inheritance?
    - What is asynchronous programming, and why is it important in JavaScript?
    - What is the difference between between global scope, and local scope (function scope, and block scope)?
    - What is hoisting, and IIFE?
    - What is closures? How to emulate encapsulating using it?
    - What is the different between ```.__proto__``` and ```.prototype```?
    - How to change the context of functions using ```.call()```, ```.apply()```, or ```.bind()```?
    - What happens when we call a function with the ```new``` keyword?
    - Consider the following code:

        ```javascript
        (function() {
            var a = b = 5;
        })();
        console.log(b);
        ```

        What will be printed on the console? If the *strict mode* was enabled using ```'use strict';```, what will be the output?

    - Define a repeatify function on the String object. The function accepts an integer that specifies how many times the string has to be repeated. The function returns the string repeated the number of times specified. For example:

        ```javascript
        console.log('hello'.repeatify(3));
        ```

        It should print hellohellohello.

    - What is the result of the following code snippets?

        ```javascript
        var fullname = 'John Doe';
        var obj = {
            fullname: 'Colin Ihrig',
            prop: {
                fullname: 'Aurelio De Rosa',
                getFullname: function() {
                    return this.fullname;
                }
            }
        };
        console.log(obj.prop.getFullname());

        var test = obj.prop.getFullname;
        console.log(test());
        ```

        ```javascript
        const obj1 = {
            value: 'hi',
            print: function() {
                console.log(this);
            },
        };

        const obj2 = { value: 17 };

        obj1.print.call(obj2);
        new obj1.print();
        ```

### <a name="languages">Object Oriented Programming (OOP)</a>

- What are the pros and cons of functional programming vs object-oriented programming?
- When is classical inheritance an appropriate choice?
- When is prototypal inheritance an appropriate choice?
- What does “favor object composition over class inheritance” mean?

### <a name="networking">Networking</a>

- What does the term network topology refer to? Describe the star topology and its cons?
- What are the layers of the OSI reference model? *(A brief description for each layer)*
- What are the layers of the TCP/IP model? *(A brief description for each layer)*
- What are the differences between IPv4 and IPv6?
- What are the differences between TCP and UDP?
- What are DNS, DHCP, and NAT?
- What does the tracert tool (Windows) or the traceroute tool (Linux) do?
- What are CDNs? What are its pros and cons?
- What are the differences between reverse proxies and forward proxies?
- What does the term AAA mean in network security?
- What is DoS/DDoS? How can protect servers from it?

**[[⬆]](#toc) return to Table of Contents**

### <a name="architecture">Architectures and Design Patterns</a>

- <a name="microservices">Microservices Architecture</a>:

    - What is the Microservices architecture?
    - What are the pros and cons of the Microservices architecture?
    - What are the differences between Monolithic, SOA and Microservices?
    - What is the API Gateway pattern?
    - What are the decomposition patterns used in Mircroservices?
    - What are the deployment strategies used in Mircoservices?

**[[⬆]](#toc) return to Table of Contents**

### <a name="security">Security</a>

- What is JSON Web Token? And when to use it?
- What is the JSON Web Token structure? And How does it work?
- What is OAuth 2.0? What are its roles?
- What are the five grants for acquiring an access token in OAuth 2.0?

**[[⬆]](#toc) return to Table of Contents**

### <a name="git">Git</a>

- What is Git? And what it is used for?
- What are the pros and cons of distributed version control systems like Git over centralized ones like SVN?
- What is Git fork? What is difference between fork, branch and clone?
- What is the difference between "git pull" and "git fetch"?
- How to revert previous commit in git?
- What is "git cherry-pick"?
- What is the difference between HEAD, working tree and index, in Git?
- Explain the Gitflow workflow?
- What is "git stash"? And when to use it?
- How to remove a file from git without removing it from the file system?
- When to use "git rebase" instead of "git merge"?

**[[⬆]](#toc) return to Table of Contents**