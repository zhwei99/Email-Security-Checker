Step 1:
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
Press "A" and "Enter"

Step 2:
Import-Module -Name .\DomainHealthChecker.psm1

Step 3 (individual):
Invoke-SpfDkimDmarc "paynet.my"

Step 3 (bulk):
Edit the domain.txt file
"paynet.my
google.com
alibaba.com"

Invoke-SpfDkimDmarc -file "domain.txt"

