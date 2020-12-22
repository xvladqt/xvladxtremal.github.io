# Cheat sheet
## Git 
* Не следить за изменениями в файле 
    ```console
    $ git update-index --assume-unchanged FILE_NAME
    ```
* Следить за изменениями в файле 
    ```console
    $ git update-index --no-assume-unchanged FILE_NAME
    ```
* Удалить только из репозитория
    ```console
    $ git rm --cached file
    $ git rm -r --cached dir
    ```
* commit diff to archive
    ```console
    $ git diff-tree -r --no-commit-id --name-only --diff-filter=ACMRT $COMMIT_SHA | xargs zip -r0 update.zip $1
    $ git diff-tree -r --no-commit-id --name-only --diff-filter=ACMRT $COMMIT_SHA | xargs tar -rf update.tar
    ```
  

## Docker
* Привязка домена к контейнеру
    ```yaml
    services:
      service:
        networks:
          default:
            aliases:
              - demo.local  
    ```

# Resources
* Деплой с помощью
   [git hooks](https://gist.github.com/noelboss/3fe13927025b89757f8fb12e9066f2fa)
* [Несколько аккаунтов git](https://medium.com/uncaught-exception/setting-up-multiple-gitlab-accounts-82b70e88c437)
