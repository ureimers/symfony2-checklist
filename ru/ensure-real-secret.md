Убедиться, что задан секретный ключ
безопасность
Убедитесь, что на production сервере задан уникальный секретный ключ. Проверить параметр можно в файле `app/config/parameters.yml`:

    secret:  please_use_a_real_secret_here

Значение по умолчанию *не* является достаточным значением секретного ключа, *необходимо* заменить его на другой.