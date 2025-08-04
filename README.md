# работа с git



-- посмотреть ветки
 $ git branch
### конфигурируем работу ветки
или $ git config pull.rebase false       -- merge (the default strategy)
-- перестраховаться от того, чтобы случайно не выполнить коммит слияния (merge commit)
или $ git config pull.rebase true        -- rebase история обеих веток сохраняется отдельно
или $ git config pull.ff only            -- fast-forward only, при выполнении pull Git применяет коммиты 
                                         -- из удалённой ветки к локальной в той же последовательности, 
                                         -- без создания новых коммитов слияния. отключить режим: pull.ff false
--  You can replace "git config" with "git config --global" to set a default
--  preference for all repositories. You can also pass --rebase, --no-rebase,
--  or --ff-only on the command line to override the configured default per
--  invocation.


## Сохранили на ПК созданный ранее репозиторий в github:  
$ git clone https://github.com/q7soft/mytest.git  
-- создадим новую ветку attestation  
$ git branch attestation  
-- сделаем ветку  attestation активной  
$ git checkout attestation  
-- созданте исразуже переключение на новую ветку attestation2  
$ git checkout branch attestation2  
-- аналогично, созданте исразуже переключение на новую ветку attestation3  
$ git checkout -b attestation3  
--  -r — при использовании этого ключа мы получим список удаленных веток,  
--  -a — используя этот параметр, в выводе будут удаленные и локальные ветки.  


# mytest
описание
---
## test
описание 2

* пункт  1
* пункт  2
* пункт  3
* пункт  4
