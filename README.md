# Git-Branch

**1.** In the local repository make branches for : Postman, Jmeter, CheckLists, Bug Reports, SQL, Charles, Mobile testing.

* `$ git branch Postman`
* `$ git branch Jmeter`
* `$ git branch CheckLists`
* `$ git branch Bag_Reports`
* `$ git branch SQL`
* `$ git branch Charles`
* `$ git branch Mobile_testing`

**2.** Push all branches to the external repository.

* `$ git push origin --all`

**3.** In the Bug Reports branch make a text document with the bug report structure.

* `$ git checkout Bag_Reports`


* `$ cat >> bug_report.txt`
```
ID: 123456
Environment: Windows 10 x 64
Browser: Google Chrom, Firefox
Reporter: Olha Chernikova
Priority: Medium
Severity: Major
Status: Open

Title: The image is not shown on the main page.

Description: The third image is not shown on the main page.

Steps To Reproduce:
        1. Open the site http://trainingcentre.wixsite.com/dogblog.
        2. Pay attention to the third image on the main page.

Actual result: The third image is not shown on the main page, but other images are shown on the main page.
Expected result: All images are shown on the main page.
```
* `Enter` ---> `Ctrl+C`

**4.** Push the bug report structure to the external repository.

* `$ git add bug_report.txt`
* `$ git commit -m "add bug_report.txt"`
* `$ git push`

**5.** Merge the Bug Reports branch into Main.

* `$ git checkout main`
* `$ git merge Bag_Reports`

**6.** Push main to external repository.

* `$ git push -u origin main`

**7.** In the CheckLists branch, outline the checklist structure.

* `$ git checkout CheckLists`
* `$ cat >> Checklist.txt`
```
Site http://opencart.qatestlab.net/


1. Home page
1.1     Design Integration (compare mockup and site)
1.2     Site logo
a       Check the logo image availability
1.3     Navigation Menu:
a       Check styling
b       Category images (different size, if applicable by design)
1.4     Banner
a       Location relative to each other
b       Spelling/grammar
1.5     Footer
a       Check footer content
b       Check footer social media links
c       Footer copyright message


2. Product Details Page
2.1     Picture
a       The product image matches its name
2.2     Active Elements
a       Check the response of active elements of the product page to hovering the mouse over
2.3     Product Specification
a       Сonformity of the product and its specification


3. Other
3.1     Correct display of currency
3.2     Check the absence of horizontal scrolling after zooming in to 150%
3.3     Notification after adding an item to the cart
```
* `Enter` ---> `Ctrl+C`

**8.** Push the structure to the external repository.

* `$ git add Checklist.txt`
* `$ git commit -m "add Checklist.txt"`
* `$ git push`

**9.** In the external repository make a Pull Request of the CheckLists branch to main Merge.

* Create pull request on GitHub :

   * `Compare and pull request`
   * `Create pull request`

**10.** Synchronize External and Local branches Main.

* `$ git checkout main`
* `$ git pull`





