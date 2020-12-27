# O'BOOKS :books::sparkles:

CLI to download and generate books from [O'Reilly](https://www.oreilly.com/) | Safaribooks.

# USAGE IN DOCKER

You need to hold an account in [O'Reilly](https://www.oreilly.com/) | Safaribooks to be able to download books.

```
$ docker pull jennyfive/obooks
$ docker run -it --rm -v "$(pwd)/obooks/:/usr/app/books/" obooks -b "<BOOK ID>" -c "<COOKIES>"
```

The book will be available in the new `obooks` folder in the current directory.
  
## **CLI flags explained**

-  **`-b <BOOK ID>`**: This is the book identification in O'Reilly. You can find it in the url of the book you'd like to download. For [this example](https://learning.oreilly.com/library/view/java-the-complete/9781260440249/), the book id would be: **9781260440249**.

-  **`-c <COOKIES>`**: O'Reilly session cookie. Logged in O'Reilly, copy the 'cookie' header in the 'Request Headers'.
