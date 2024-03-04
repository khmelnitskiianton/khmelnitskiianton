# Git Help

## Start & Create SSH Keys

```c
git config --global user.name "name"
git config --global user.email "email@mail.ru"
```

```c
>ssh-keygen -t ed25519 -C "your_email@example.com"  #generate ssh-key
>ls ~/.ssh
>eval "$(ssh-agent -s)"                             #ssh-agent
```

+ Open file with key and copy it
+ Go to github in Settings/SSH_Key - New Key insert key

```c
>ssh -T git@github.com  #check for complete
```

## Init & Push Repo

```c
>cd ./new_project                                                   #create folder
>git init                                                           #add git to this folder
>echo "Bla-bla" >> README.md                                        #create readme
>git add .                                                          #add all files tracking
>git commit -m "<changes>"                                          #commit 
>git branch -M main                                                 #set current branch
>git remote add origin git@github.com:khmelnitskiianton/Books.git   #before check ssh keys
>git push -u origin main                                            #push to main
```

## Other Functions

```c
>git clone <url>
>git status
>git log
>git log —all —decorate —oneline —graph
```

