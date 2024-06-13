Common Steps

->Main banda folder and iniital files bnaayega
->Ab usse github par upload krde
->Collaborators add kre(mtlb kon kon project pr kam krega )



->Saare bande us repo se cloning karein
[Very Imp]
->Har banda apni branch crete karein apna code usi brnch mein likhein
->Complete hone pr commit krde and push krde.
->Inform kre teammate ko about commit
->merger bnda fetch karega and merge karega and re-push krega.


<!-- How to upload code on GitHub -->

Step-1 ) Create a repo

Step-2 ) Open Terminal
-->echo "# repo-name" >>README.md (ye basic commands mil jayenge github pr he jb hum repo create krenge )

-->git init

-->git add .(isse sari file add ho jayenge  originally command hai git add README.md pr hum bs git add . use krenge wo better hai  )

-->git commit -m "firsr-commit"

-->git branch -M main

--> git remote add origin repo-url("isse hum vscode ko ye bta rhe ki mera work kis url pr upload hona chaiaye)

--> git push -u origin main(main branch ka namm hai koi bhi nam de skte ho i.e jo feature add kr rhe wo namm de do i.e git push -u origin feature-abc
)


<!-- How to add Collaborators -->
Step-1) Go to Settings

Step-2 ) Go to Collaborators

Step-3) Click on add people and write username and email.



Suppose ek project hai usme 2 bande kam kr rhe A and B. A jo hai leader hai project ka tu wo basic set-up krega aur main branch ko push krega github pr and  Collaborators add krega.


Ab B jo hai clone krega repo ko apne  pc pr aur jo code krna hai krega

<!-- How to clone repo -->

Step -1) Open terminal

Step-2 ) git clone repo-url

Step-3) Do changes you want to do and push it



Ab A jo hai usko update mila B sai ke code mai changes hogye hai tu ab A fetch krega branch ko jo B ne upload kre hai aur usko merge krega aur main branch mai push krdega 
<!-- How to merge 2 branchs if you are working with collaborators  if we are working alone than we just can directly merge to main branch -->

Step -1) Open terminal

Step-2) git fetch

Step -3) git switch branchName

Step-4) git merge branchName

Step-5) git push origin main(sara code main branch pr push krdenge )



Ab B ko agr agye kuch aur features add krne hai tu wo kya krega ki usko fetch krega aur pull krdega. To updated code uske pc mai ajayega 


->git fetch

->git pull