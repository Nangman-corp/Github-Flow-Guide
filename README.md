# Github Flow Guide

<aside>
ð¡ ë³¸ë¬¸ì ë­ë§(Nangman)ì Github Flow ê°ì´ë ìëë¤.

</aside>

## ëª©ì°¨

---

### [1. ìê° / ì¬ì© ê°ì´ë](https://github.com/Nangman-corp/Github-Flow-Guide/blob/main/README.md#1-%EC%86%8C%EA%B0%9C--%EC%82%AC%EC%9A%A9-%EA%B0%80%EC%9D%B4%EB%93%9C-1)

- [1.1 Github Flow](https://github.com/Nangman-corp/Github-Flow-Guide/blob/main/README.md#11-github-flow--develop-branch)

- [1.2 ìììì ë³ GIT ëªë ¹ì´ ê°ì´ë](https://github.com/Nangman-corp/Github-Flow-Guide/blob/main/README.md#12-%EC%9E%91%EC%97%85-%EC%88%9C%EC%84%9C-%EB%B3%84-git-%EB%AA%85%EB%A0%B9%EC%96%B4-%EA%B0%80%EC%9D%B4%EB%93%9C)

### [2. ì»¨ë²¤ì](https://github.com/Nangman-corp/Github-Flow-Guide/blob/main/README.md#2-%EC%BB%A8%EB%B2%A4%EC%85%98-1)

- [2.1 ê¸°ë¥êµ¬í ì­í  ë¶ë°°](https://github.com/Nangman-corp/Github-Flow-Guide/blob/main/README.md#21-%EA%B8%B0%EB%8A%A5%EA%B5%AC%ED%98%84-%EC%97%AD%ED%95%A0-%EB%B6%84%EB%B0%B0)

- [2.2 Feature Branch ë¤ì´ë° ì»¨ë²¤ì](https://github.com/Nangman-corp/Github-Flow-Guide/blob/main/README.md#22-feature-branch-%EB%84%A4%EC%9D%B4%EB%B0%8D-%EC%BB%A8%EB%B2%A4%EC%85%98)

- [2.3 Commit Message ì»¨ë²¤ì](https://github.com/Nangman-corp/Github-Flow-Guide/blob/main/README.md#23-commit-message-%EC%BB%A8%EB%B2%A4%EC%85%98)

- [2.4 Pull Request - Create ì»¨ë²¤ì](https://github.com/Nangman-corp/Github-Flow-Guide/blob/main/README.md#24-pull-request---create-%EC%BB%A8%EB%B2%A4%EC%85%98)

- [2.5 Pull Request - Code Review ì»¨ë²¤ì](https://github.com/Nangman-corp/Github-Flow-Guide/blob/main/README.md#25-pull-request---code-review-%EC%BB%A8%EB%B2%A4%EC%85%98)

---

# 1. ìê° / ì¬ì© ê°ì´ë

---

íì ê° ì¬ì©í  Github Flowì ëí ìê° ë° ì¬ì© ê°ì´ëë¥¼ ì¤ëªí©ëë¤.

## 1.1. Github Flow + develop Branch

---

íì ê° ì¬ì©í  Github Flowì ëí´ ì¤ëªí©ëë¤.

![img/description](img/description.png)

- Github Flowë Git flowì ë³µì¡ì±ì ì ê±°í ë¨ìí ë°©ìì flow ìëë¤.
- **main** / **develop** / **feature** branchë¡ êµ¬ì±ë©ëë¤.

```markdown
feature branch : ê¸°ë¥ êµ¬íì ìí ë¸ëì¹ë¡, ìì± - ì­ì ê° ë°ë³µëë ìì ê³µê°ìëë¤.
develop branch : ìë¡ ìë°ì´í¸ ë  ë²ì ì ì½ëê° ìë°ì´í¸ ëë ë¸ëì¹ìëë¤. 
main branch : íì¬ **ì¶ìë** ìµì  ë²ì  íë¡ëí¸ì ì½ëê° ì¡´ì¬íë ë©ì¸ ë¸ëì¹ìëë¤.
```

### feature branch

- feature branchë ë¨ì ê¸°ë¥ ë³ êµ¬íì ìí´ ìì± - ì­ì ê° ë°ë³µëë branch ìëë¤.
- feature branchë í­ì develop branchìì ë¶ê¸°ëë©°, ìµì  ë²ì ì develop branch ì½ëë¥¼ pull íì¬ ììí©ëë¤.
- feature branchë main branchì ì§ì ì ì¼ë¡ ìí¸ìì©íì§ ììµëë¤.
- feature branchìì ë¨ì ê¸°ë¥ ë³ ì ì ëìì íì¸í í develop branchì ë³í©í©ëë¤.

### develop branch

- develop branchë feature branchìì ë³í©ë ë¤ì ë²ì ì ê¸°ë¥ë¤ì´ ê´ë¦¬ëë ê³ ì  branch ìëë¤.
- ìë¡­ê² ìë°ì´í¸ ë  ë²ì ì ê¸°ë¥ êµ¬íì´ ëª¨ë develop branchì ë³í©ëìë¤ë©´ ìµì¢ì ì¼ë¡ íì¤í¸ë¥¼ ìíí í main branchì í´ë¹ develop branchë¥¼ ë³í©í©ëë¤.

### main branch

- main branchë íì¬ ì¶ìë ìµì  ë²ì ì í´ë¹íë íë¡ëí¸ì ì½ëê° ì¡´ì¬íë ê³ ì  branch ìëë¤.
- develop branchìì ë¤ì ë²ì ì í´ë¹íë ê¸°ë¥ì´ ëª¨ë êµ¬íëì´ í´ë¹ main branchì ë³í©ëìë¤ë©´, ë¤ì ë²ì ì í´ë¹íë ë²ì  ë²í¸ë¥¼ tagë¡ ì¤ì íì¬ main branchì ë²ì ì ê´ë¦¬í©ëë¤.

## 1.2. ìì ìì ë³ GIT ëªë ¹ì´ ê°ì´ë

---

Github Flow ìì ììì ë°ë¥¸ GIT ëªë ¹ì´ ê°ì´ëë¥¼ ì¤ëªí©ëë¤.

**í ê¸ì í¼ì¹ë©´ ììì í´ë¹íë GIT ëªë ¹ì´ ê°ì´ëê° ëíë©ëë¤.**

/ / main : íì¬ Command Line ê¸°ì¤ main branchê° checkout ëì´ììì ìë¯¸í©ëë¤.

/ / develop : íì¬ Command Line ê¸°ì¤ develop branchê° checkout ëì´ììì ìë¯¸í©ëë¤.

/ / feature : íì¬ Command Line ê¸°ì¤ feature branchê° checkout ëì´ììì ìë¯¸í©ëë¤.

- 0.  (ìµì´ 1í) ìê²© ì ì¥ìì ì½ëë¥¼ ìì ì ì»´í¨í°ì ë³µì (Clone) í©ëë¤.
    
    ```c
    git clone [URL] [ìì¤ì½ëê° ì ì¥ë  í´ëëª]
    ```
    

- 1. êµ¬íí  ê¸°ë¥ì´ ì£¼ì´ì¡ì ê²½ì°, develop branchìì ìë¡ì´ branchë¥¼ ìì±í©ëë¤.
    
    ```c
    git checkout develop // main
    git checkout -b [ë¸ëì¹ëª] // develop
    
    git push -u origin [ë¸ëì¹ëª] // feature, ìê²© ì ì¥ìì í´ë¹ branch ìì±
    ```
    
    - ë³¸ ëªë ¹ì´ë¥¼ íµí´ branchë¥¼ ìì±í¨ê³¼ ëìì í´ë¹ branchë¡ checkout ë©ëë¤.

- 2. ìì±í Branchìì ì½ëë¥¼ ìì±í©ëë¤.
    - ë¨ì ê¸°ë¥ êµ¬í ì¤ gitìì ë³ëë¡ ì²ë¦¬í  ììì ììµëë¤.

- 3. êµ¬í ììì ëí´ íëì ìì ë¨ì ë³ë¡ ì»¤ë° ë©ìì§ë¥¼ í¬í¨íì¬ ì»¤ë°ì ê¸°ë¡í©ëë¤.
    
    ```c
    git add . // Feature
    git commit -m "[ì»¤ë° ë©ìì§]"
    ```
    

- 3-1. ììì´ ëª¨ë ìë£ë ê²½ì° ëë ìì ì¤ ë¶íìí ì»¤ë°ì´ ì¡´ì¬íë ê²½ì° ì»¤ë°ì í©ì¹  ì ììµëë¤.
    - **í´ë¹ Squash ììì ë°ëì push ì ì ìíí´ì¼ í©ëë¤.**
    
     
    
    ```c
    git log --pretty=oneline // Feature
    ```
    
    ì ì»¤ë§¨ë ìë ¥ ì ìëì ê°ì ë¡ê·¸ê° ì¶ë ¥ë©ëë¤.
    
    ```c
    						[COMMIT ID]                    [COMMIT MESSAGE]
    
    1da8660499416696d8079da36f29d054c69b7d8a (HEAD -> master) add: r4
    4741e7919acb7e7658003aca658bca3623b904ed add: New2
    a595fbe76a1998a52da9c749d07cef453e8fb9bf add: New1
    879e279266224de9aeb4e82ae925c4e0e73ecef3 refactor: int bbbb change
    fb2dde72ad021740ddc57930e7b455f7c847fa08 add: Company
    a86002156495a27ad95594b3e1a56608e7d7d24e refactor: getName
    d89549e893b685d8ea2400ab45088104cbfb8308 add: User Entity
    458576123ffa41092eb0a57f880b598dccff9a00 init
    ```
    
    **add: New1** ì»¤ë°ê³¼ **add: New2** ì»¤ë°ì í©ì¹ë¤ê³  ê°ì íì ë, í©ì¹  ì»¤ë°ì ë°ë¡ ìë ì»¤ë° idë¥¼ ë³µì¬íê³ , 
    
    ìë ëªë ¹ì´ë¥¼ ìë ¥í©ëë¤.
    
    ```c
    git rebase -i [ë³µì¬í ì»¤ë° ID] // Feature
    ```
    
    ì´í ë¬¸ì í¸ì§ê¸°ê° ì¤íëë©° ìëì ê°ì ë¬¸ìì´ì´ ì¶ë ¥ë©ëë¤.
    
    ```c
    pick add: New2
    pick add: New1 
    ```
    
    ë¬¸ì í¸ì§ê¸°ë¥¼ íµí´ add: New1ì pickì s(ëë squash)ë¡ ìì íì¬ ìì pick ì»¤ë°ê³¼ í©ì³ì§ ê²ìì ìë¦½ëë¤.
    
    ```c
    pick add: New2
    s add: New1 
    ```
    
    ì´í ì ì¥ì ìííë©´, ë¬¸ì í¸ì§ê¸°ê° ì¤íëë©° ìëì ê°ì ë¬¸ìì´ì´ ì¶ë ¥ë©ëë¤.
    
    ```c
    # This is a combination of 2 commits.
    # This is the 1st commit message:
    
    add: New2
    
    # This is the commit message #2:
    
    add: New1
    
    # Please enther the commit message ...
    ```
    
    ê¸°ì¡´ì ì»¤ë° ë©ìì§ ììë #ì ë¶ì¬ ìì ê³ , # This is a combination of N commits ìëì ìë¡ì´ ì»¤ë° ë©ìì§ë¥¼ ìì±í©ëë¤.
    
    ```c
    # This is a combination of 2 commits.
    [ìë¡ ìì±í  ì»¤ë° ë©ìì§]
    # This is the 1st commit message:
    
    # add: New2
    
    # This is the commit message #2:
    
    # add: New1
    
    # Please enther the commit message ...
    ```
    
    í´ë¹ ë¬¸ìë¥¼ ì ì¥íë©´ ì»¤ë° í©ì¹ê¸°ê° ìë£ë©ëë¤.
    

- 4. êµ¬íì´ ìë£ëë©´ develop branchì ì»¤ë° ë´ì­ì ëí´ Rebaseë¥¼ ìíí©ëë¤.
    
    ```c
    git checkout develop // feature
    git pull // develop
    git checkout [ë¸ëì¹ëª] // develop
    git rebase develop // feature
    ```
    
    - ì´ ë, ì¶©ë(Conflict)ì´ ë°ìí ê²½ì° Rebaseê° ì¼ìì ì§ë©ëë¤.
    - ì¶©ëì´ ë°ìí ê²½ì°, ì¶©ëë ì½ëì ìì±ìì íìë¥¼ íµí´ ì½ëë¥¼ ìì í©ëë¤.
    - í´ë¹ ì½ë ìì  ìë£ í ìë ëªë ¹ì´ë¥¼ ìë ¥í´ Rebaseë¥¼ ë¤ì ì§íí©ëë¤.
    
    ```c
    git rebase --continue // feature
    ```
    
    - í´ë¹ ëªë ¹ì´ ìë ¥ í ë¤ë¥¸ ì¶©ëì´ ë°ìí ê²½ì° ì ê³¼ì ì ë°ë³µí©ëë¤.
    - âApplying: ~â ë©ìì§ê° ë¬ë¤ë©´ Rebaseê° ìë£ë ê²ìëë¤.

 

- 5. ìê²© ì ì¥ìì í´ë¹ branchì ì»¤ë° ë´ì­ì pushí©ëë¤.
    
    ```c
    git push -u origin [ë¸ëì¹ëª] // feature
    ```
    

- 6. í´ë¹ branchë¥¼ develop branchì ë³í©(Merge) ìì²­íë Pull Requestë¥¼ ìì±í©ëë¤.
    - Githubì í´ë¹ íë¡ì í¸ Repositoryìì í´ë¹ branch â developì PRì ìì±í©ëë¤.

- 7. íì ê° Pull Requestì ëí´ ì½ë ë¦¬ë·° ë° ê¸°ë¥ì ì ì ëì ì¬ë¶ë¥¼ íì¸í©ëë¤.
    
    

- 8. íì¤í¸ê° ìë£ë ê²½ì°, í´ë¹ Pull Requestì ëí´ develop branchë¡ì ë³í©ì ìíí©ëë¤.
    - Githubì í´ë¹ íë¡ì í¸ Repositoryìì í´ë¹ PRì ëí´ **Rebase and Merge**

- 9. ììì´ ìë£ ë feature branchë ìê²© ì ì¥ì / ë¡ì»¬ ì ì¥ììì ì­ì í©ëë¤.
    
    ```c
    git checkout develop // feature
    git push origin --delete [ë¸ëì¹ëª] // develop, ìê²© ì ì¥ììì branch ì­ì 
    git branch -D [ë¸ëì¹ëª] // develop, ë¡ì»¬ ì ì¥ììì branch ì­ì 
    
    git pull // develop, ìµì  ë²ì ì develop branch ìì¤ì½ë ê°ì ¸ì¤ê¸°
    ```
    

# 2. ì»¨ë²¤ì

---

íì ê° ì­í  ë¶ë°°, ë¤ì´ë°ê³¼ ê°ì ì¼ê´ë ì»¨ë²¤ìì ì¤ëªí©ëë¤.

## 2.1. ê¸°ë¥êµ¬í ì­í  ë¶ë°°

---

ê¸°ë¥ êµ¬íì ìí í ë´ ì­í  ë¶ë°°ì ëí´ ì¤ëªí©ëë¤.

1. íìë¥¼ íµí´ êµ¬íí´ì¼ í  ë´ì©ì ì¤íë¦°í¸ ë³ë¡ ì ë¦¬í©ëë¤. 
2. ì¤íë¦°í¸ë¥¼ íµíì¬ êµ¬íë´ì©ì ìì°¨ì ì¼ë¡ ëì´í©ëë¤. ìì ë¨ìë¡ ëë ì§ ì¤íë¦°í¸ë **Ticket** í¹ì **card**ë¼ê³  ë¶ë¦ëë¤.
3. ê°ë°ìë ì»¤ë®¤ëì¼ì´ìì íµí´ Ticketì ê°ì ¸ê°ê³ , í´ë¹ ê¸°ë¥ì ì£¼ì´ì§ ì¤íë¦°í¸ ê¸°ê° ëì êµ¬íí©ëë¤.

### ì­í  ë¶ë°°ìì ì£¼ìí  ì 

- íì ê° Code Conflictë¥¼ ë°©ì§íê¸° ìí´ ê° ìì ë¨ìë ë¤ë¥¸ ììì ììì ì¹¨ë²íì§ ììì¼ í©ëë¤.
- ë§ì½ íëì ììì ëí´ ì¬ë¬ ê¸°ë¥êµ¬íì´ ëëì´ì ¸ ìë¤ë©´, ê°ê¸ì  í ëªì´ í´ë¹ ììì Ticketë¤ì ë§¡ìµëë¤.

## 2.2. Feature Branch ë¤ì´ë° ì»¨ë²¤ì

---

ê° ìì ë³ë¡ ìì±ëë feature branchì ë¤ì´ë° ì»¨ë²¤ìì ì¤ëªí©ëë¤.

### Category

- **feature :** ê¸°ë¥ êµ¬í
- **issue** : Github Repositoryì ë±ë¡ë issueì ëí í´ê²°

### Description

- feature description: êµ¬íí  ê¸°ë¥ì ì¤ëªí©ëë¤. ìë¬¸ì¼ë¡ ìì±íë©°, ê³µë°±ì â-âì¼ë¡ êµ¬ë¶í©ëë¤.
- issue description: #issue ë²í¸ë¥¼ ì ìµëë¤. ì¸ë¶ì ì¸ descriptionì issue í­ìì íì¸í©ëë¤.

```c
feature/user-signup
feature/company-address-edit

issue/#8
issue/#122
```

## 2.3. Commit Message ì»¨ë²¤ì

---

ë¨ì ìì ìë£ í ì»¤ë° ì ë©ìì§ì ëí ì»¨ë²¤ìì ì¤ëªí©ëë¤.

### Behavior

- **feat :** ìë¡ì´ ê¸°ë¥ ì¶ê°
- **fix** : ë²ê·¸, ì½ë ì¶©ë ìì 
- **docs** : ë¬¸ì ìì  (ì£¼ì ë±)
- **style** : ì½ë í¬ë§·í ë± ì½ë ë¡ì§ì ë³ê²½ì´ ìë ê²½ì°
- **refactor**: ì½ë ë¦¬í©í ë§
- **test**: íì¤í¸ ì½ë
- **chore**: Build ê´ë ¨ ìì  (build.gradle etcâ¦)

### Title

- íê¸ / ìì´ ëª¨ë ìì± ê°ë¥í©ëë¤.
- 50ì ì´ë´ë¡ ìì±í©ëë¤.
- ìì´ë¡ ìì± ì ì ëª©ì ì²« ê¸ìë ëë¬¸ìë¡ ìì±í©ëë¤.
- ìì ë´ì©ì ëªííê² ì´í´í  ì ìëë¡ ìì í©ëë¤.
- ë§ì¹¨íë¥¼ ë¶ì´ì§ ììµëë¤.

```c
[Behavior: Title]

feat: User-Company Entity ì°ê´ê´ê³ ìì 
```

### Body

- ì íì¬í­ì¼ë¡, ëª¨ë  ì»¤ë°ì ë³¸ë¬¸ì ìì±í  íìë ììµëë¤.
- ë¶ì°ì¤ëªì´ íìíê±°ë, Titleë§ì¼ë¡ë ì¤ëªì´ ë¶ì¡±í ê²½ì° ìì±í©ëë¤.
- Titleê³¼ì êµ¬ë¶ì ìí´ í ì¤ì ëê³  ìì±í©ëë¤.

## 2.4. Pull Request - Create ì»¨ë²¤ì

---

Pull Requestë¥¼ ìì±í  ë ìì±í  ë´ì©ì ì¤ëªí©ëë¤.

### Title

Ticketì ì ëª©ê³¼ ëì¼íê² ìì±í©ëë¤.

### Description

êµ¬íí ê¸°ë¥, í´ê²°í ì´ìì ëí´ ë¦¬ì¤í¸ íìì¼ë¡ ëì´í©ëë¤.

í´ë¹ ìì­ì Ticketì ë³¸ë¬¸ ë´ì©ê³¼ ì¼ì¹í  ìë ìê³ , ì¤ì  êµ¬íì ë°ë¼ ë¬ë¼ì§ ìë ììµëë¤.

```c
- User íìê°ì êµ¬í
- User íìê°ì Validation
- UserSignupService Test
```

![img/description_1](img/description_1.png)

## 2.5. Pull Request - Code Review ì»¨ë²¤ì

---

ìì±ë Pull Requestì ëí ì½ë ë¦¬ë·°ë¥¼ ì¤ëªí©ëë¤.

<aside>
ð¡ í´ë¹ ì¹ìì ë´ë¶ íìë¥¼ íµí´ ëªíí Ruleì ì í  íìê° ììµëë¤.

</aside>

### Contributors
---
[ë°íì±](https://github.com/HunSeongPark)ì´ ìì±íììµëë¤.
- [Contributors](https://github.com/Nangman-corp/JSON-Value-Style-Guide/graphs/contributors)
