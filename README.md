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
## Git
## Laravel
## Docker