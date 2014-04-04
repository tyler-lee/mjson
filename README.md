JSON (JavaScript Object Notation) is a lightweight data-interchange format. You knew that already. If not, continue reading on http://www.json.org.

It's supposed to be about simplicity and clarity. Something minimal, intuitive, direct. Yet, I couldn't find a Java library to work with it in this way. The GSON project is pretty solid and comprehensive, but while working with REST services and coding some JavaScript with JSON in between, I got frustrated of having to be so verbose on the server-side while on the client-side manipulating those JSON structures is so easy. Yes, JSON is naturally embedded in JavaScript, so syntactically it could never be as easy in a Java context, but it just didn't make sense all that strong typing of every JSON element when the structures are dynamic and untyped to being with. It seemed like suffering the verbosity of strong typing without getting any of the benefits. Especially since we don't map JSON to Java or anything of the sort. Our use of JSON is pure and simple: structured data that both client and server can work with. 

After a lot of hesitation and looking over all Java/JSON I could find (well, mostly I examined all the libraries listed on json.org), I wrote yet another Java JSON library. Because it's rather independent from the rest of the project, I separated it. And because it has a chance of meeting other programmers' tastes, I decided to publish it. 

