Hi, I hope you are doing good.

I select the second task and reivew and rewrite a code little bit. However, due to
shortage of my time and my busy schedule I did not write and review code in depth.

#Good points in code:
1) Code is following a repository pattern which is very good to manage code.
2) Function names and variable names are proper. Which makes code easy to read.

#Things needs to improve
1)	Unnecessary Variables (like return $user = UserMeta::where('user_id', $user_id)->first()->$key; ) No need of $user here.
2)	Unreachable codes (like code after return statements).
3)	If conditions not properly structured. (like in function willExpireAt).
4)  Too many redundant code. We can use short methods like using relationships, by breaking
    code into small functions.
5) Laravel Functions are not utilize like upateOrCreate, firstOrCreate.
6) In code base repository class in defined by not utilized properly, like validations methods
    are not in use in this code.

#Performance Issues
1) Unnecessary if else and too much use loops, which slow down the code execution speed.
2) Unncessary Variable declarations (Memory management is not good).
3) Lazy loading approach is used, There must be eager loading while fetching data from relations.
4) Laravel builtin and Eloquent functions should be there instead of loops.
