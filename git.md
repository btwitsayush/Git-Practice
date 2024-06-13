stages:
U- untracked (it means git is now aware of the file)
A- added or staged(it means git is aware of the file)
C- Commited(it means git is tracking your progress)

git commands

<!-- It shows the current status of saved points-->
git log --oneline 

<!-- If we want to ignore a file from our project 

then we create a file using extenstion .gitignore
and write the name of the file.
-->

<!-- To go back to some previous saved point  -->
git reset --hard HEAD ~1
(iise 1 saved point peeche jayenge aur hard hai tu iska mtlb hai jo file us saved point pr nhi the wo remove ho jayege i.e maine 1 save point bnaya uske baad ek file banye git ignore tu ab mai jb hard reset krunga tu mai saved point pr chla jaunga mere jo file hai wo bhi remove ho jayege q ki maine usko save nhi kiya tha)
git reset --soft
git reset --mixed




<!-- how git works? -->

Jb bhi hum el folder create krte hai project bnaane ke loye tu git ko uske baare mai kuch pta nhi hota ,issiliye hum sbse pehle git ko initalize krte hi.Initialize krte kaise hi?uske liye hme jana hota hai source control pr.
Ab initalize krne ke baad git kaam krne ke liye ready hota hai .Git ab hume help krega untracked ,tracked ,modified staged files  and save checked points ko manage krne mai.

git allow us to do following things

-->we can check ke konsi file kis stage mai hai =>git status -s(pr ye command bs un file ka status btate hai jo ya to commit nhi hue hi ya phir commit hone ke baad unme koi chnages kiye gye hoo)
-->check kr skte hai ke kitne saved checkpoint hai file mai git log--oneline




<!-- Git Branch -->

-->Branch ka basic mtlb hota hai apne main code ke ek copy bnana.

git branch branchname   (branch name hmesha usefull hona chaiye tu aise dete hai branchname i.e feature/nav-bar baki koi bhi nam dena allow hai);

<!-- To check how many branch are there  -->
git branch
 

 <!-- To switch to some other Branch(by default we will be in the main) -->


 git switch branchname(jha pr switch krna ho)
 
 <!-- To create a branch and switch at same time -->
 git switch -C newbranchname(branch create krega aur same time pr switch bhi kr jayega  )

<!-- Ab switch krne ke bad jo code hum nayi branch mai likhenege wo main ya baki branch mai visible nhi hoge agr humne commit krdiya wo bs us branch mai he avilabale hoge jis branch mai likhe jayege -->

<!-- Ab ek branch ka code main mai ajaye uske liye hum krte hai merge

kesi bhi branch ko merge krne ke liye hume pehle main pr hon jrrori hota hai 

phr command likhna hota hai
 -->

 git merge branchname(jisko merge krna ho)

 <!-- Conflict -->

 Agr main branch mai same line pr kuch different code ya data likha hai aur jis branch ko merge krna cha rhe uspe kuch alag data likha hai tu problem ate hai .

 i.e main branch ke line 10 pr different code hai aur dusre branch pr 10 line pr alag code hai.

conflict krne ke baad hme 3 option milta hai
1)Accept Current change(mtlb main branch ke code ko accept krdo or dusre branch ke code ko hta do)
2)Accept Incoming Chnage(mtlb ke dusre branch ke code ko accept krlo aur main brach ke code ko hta do)
3)Accept both the Chnage(mtlb ki dono branch ke code ko accept krlo ){3rd condition krne ke baad hme code ko phir sai commit krna hoga}


<!-- how to delete a branch -->

git branch -d branchname(jo delete krna hai )


<!-- Stashing -->

Suppose hum main branch mai kam kr rhe aur code reffrence ya kese kaam sai dusre branch pr switch krna cha rhe aur jo latest code main branch pr likha hai wo save bhi nhi kiya hai. To jb switch krne ka try krenge to kya hoga ki git hme allow nhi krega switch krne ke liye wo hme bolega ya tu iss code ko delete krdo ya stash krlo.
Ab stash kya krega ki wo recent code ko git ke memory mai rkh dega aur hme allow krdega switch krne ke liye . Phir jb wps main branch pr ayenge tu hum stash apply krke code wps laa skte hai . Aur agr stash ko clear krna hua tu wo bhi kr skte hai.


<!-- How to do stash -->
git stash
<!-- how to apply stash -->
git stash apply
<!-- how to delete stash -->
git stash clear 

