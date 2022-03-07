1) Делаем fork репозитория 2020
1) git init
1) git clone <Url своего KotlinAsFirst2020>
1) git remote add -f upstream-my <Url своего KotlinAsFirst2021>

\7) git remote -v (проверяем, что всё правильно добавилось)

\8) git branch backport (создаем новую ветку)

\9) git checkout backport (переходим на неё)

\10) git branch –a -v (смотрим последние комиты)

\11) git cherry-pick -Xours <комит до первого>..<последний комит> (добавляем комиты)

\12) gitk (проверяем, что всё добавилось)

\13) git checkout master

\14) git merge master (объединяем ветки)

\15) git remote -d backport (удаляем ветку)

\16) git remote add -f upstream-theirs <Url партнёра KotlinAsFirst2021>

\17) git cherry-pick -Xtheirs <комит до первого>..<последний комит>

\18) git add "howto.md"

\19) git commit -m "file howto.md"

\20) git add "remotes.txt"

\21) git commit -m "file remotes.txt"

\22) git push
