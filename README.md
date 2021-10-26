1,2,3  
git init  
git add .  
git status  
git commit -m "пояснения"  
на странице GitHub кнопка "New" -> название , описание, если надо галочка создать readme.md -> скопировать путь HTTPS -> в консоли ->    
git remote add orrigin (скопированный HTTPS сode)  
git push --set-upstream origin master   
4  
git add .  
git status  
git commit -m "added style.css"  
5 создаю ветку version-1 от ветки master  
git checkout -b version-1  
6. возвращаемся на ветку master  
git checkout master  
7. переименовать файл style.css -> styles.css  
mv style.css styles.css  
git add .  
git status  
git commit -m "renamed style in styles"  
8. cоздали и подключили index.js  
git add .  
git status  
git commit -m "added index.js"  
git push origin master  
9i,ii. изменила стили в файле styles.css  
git add .  
git status  
git commit -m "changed  color and font-size"  
git push origin master  
9iii,iv  
git log   
скопировать последний id коммита -> 4ae3af7e84d063606a8111d996117ab204095609  
перейти на ветку version-1  
git checkout version-1  
git cherry-pick 4ae3af7e84d063606a8111d996117ab204095609  
git push origin version-1  