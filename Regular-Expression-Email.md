# Matching an Email

## Summary

The regular expression being described is:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This regular expression matches a string that represents a valid email address. The email address should consist of a username (consisting of one or more alphanumeric characters, underscores, dots, and hyphens), followed by the "@" symbol, followed by a domain name (consisting of one or more alphanumeric characters, dots, and hyphens), and ending with a valid top-level domain (consisting of two to six letters or dots).

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

The regular expression begins and ends with the / symbol, which are used in JavaScript to delimit a regular expression. The ^ anchor matches the start of the string, while the $ anchor matches the end of the string. Together, these anchors ensure that the entire string matches the regular expression, rather than just a portion of it.

### Quantifiers

The + quantifier matches one or more of the preceding character or group. In this regular expression, it is used to match one or more instances of alphanumeric characters, underscores, dots, or hyphens in the username and domain name. The {2,6} quantifier matches between 2 and 6 instances of the preceding character or group, in this case the letters or dots in the top-level domain.

### Character Classes

Character classes are denoted by square brackets [] and match any single character within the brackets. In this regular expression, [a-z0-9_\.-] matches any lowercase letter, digit, underscore, dot, or hyphen. [\da-z\.-] matches any digit, lowercase letter, dot, or hyphen. Finally, [a-z\.] matches any lowercase letter or dot, which are used in the top-level domain.

### Grouping and Capturing

Parentheses () are used to group and capture parts of the regular expression. In this regular expression, there are three groups being captured:

([a-z0-9_\.-]+) captures the username.
([\da-z\.-]+) captures the domain name.
([a-z\.]{2,6}) captures the top-level domain.

### Bracket Expressions

Bracket expressions are used to match a single character from a range or set of characters. In this regular expression, [a-z] matches any lowercase letter, while [0-9] matches any digit.

### Boundaries

The ^ and $ anchors are used as boundaries to match the start and end of the string, respectively.

## Author

Hello, my name is George Doyle. I am a novice full-stack developer who recently completed a bootcamp in web development. Before transitioning to tech, I worked as a project manager in the real estate and remodeling industry, where I managed over 30 crews with installations totaling over 1 million dollars a month.

During my time in real estate and remodeling, I gained extensive experience in project management, team leadership, and client communication. I learned how to manage complex projects from start to finish, from initial client consultation to final project delivery.

My passion for technology and creative problem-solving led me to pursue a career in web development, where I can apply my skills in project management and teamwork to build innovative and effective web solutions. During my bootcamp, I gained experience in HTML, CSS, JavaScript, and various web development frameworks.

I am constantly seeking to learn and improve my skills, both as a developer and a project manager. You can find some of my projects and code samples on my Github page https://github.com/GeorgeDoyle1175.
