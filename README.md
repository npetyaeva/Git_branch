## Git : HW_2

Branch : master

1. На локальном репозитории сделать ветки для:  
    - Postman  
`git branch postman`
    - Jmeter  
`git branch jmeter`
    - CheckLists  
`git branch checklist`  
`git branch -m checklist checklists`
    - Bag Reports  
`git branch bugreports`
    - SQL  
`git branch sql`
    - Charles  
`git branch charles`
    - Mobile testing  
`git branch mobiletesting`

2. Запушить все ветки на внешний репозиторий  
    `git remote add origin https://github.com/npetyaeva/Git_branch`  
    `git push -u origin master`  
    `git push origin --all`  
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта  
    `git checkout bugreports`  
    `vim bugreport.txt`
    ```
    ID: 
    Summary:
    Discription:
    Project:
    Steps to reproduce:
    Actual result:
    Expected result:
    Severity:
    Priority:
    Status:
    Environment:
    Author:
    Assingned to:
    Attachement: 
    ```
    `Esc :wq`  
4. Запушить структуру багрепорта на внешний репозиторий  
    `git add .`  
    `git commit -m "Added bugreport.txt"`  
    `git push`  
5. Вмержить ветку Bag Reports в Main  
    - На GitHub-e открыть вкладку Pull requests
    - Кликнуть по кнопке New pull request  
    - Выбрать ветки: `base: master -> compare: bugreports`  
    - Нажать на кнопку Create pull request
    - Подтвердить слияние веток
6. Запушить main на внешний репозиторий.  
    `git pull`
7. В ветке CheckLists набросать структуру чек листа.
8. Запушить структуру на внешний репозиторий
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
10. Синхронизировать Внешнюю и Локальную ветки Main
