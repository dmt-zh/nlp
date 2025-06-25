## Предварительные требования

Для начала работы нужны:
* Linux (Ubuntu22+, Debian) либо Windows10/11 + WSL2
* Python версии 3.12.x

<hr>


## Настройка окружения:

Копируем репозиторий:
```bash
git clone https://github.com/dmt-zh/nlp.git && cd nlp
```

Создаем виртуальное окружение с помощью команды:
```bash
python3.12 -m venv env
```

Активируем виртуальное окружение с помощью команды:
```bash
source env/bin/activate
```

Внутри виртуального окружения устанавливаем poetry:
```bash
pip install poetry
```

Устанавливаем зависимости в виртуальном окружении с помощью команды:
```bash
poetry install --no-root
```

<hr>

## Для работы с кодом ноутбуков необходимо:

Запутить Jupyter server в фоновом режиме

```sh
nohup python -m notebook &> logging.log &
```
Перейти по url адресу в браузере
```
http://localhost:8888/
```

После завершения работы деактивировать виртуальное окружение командой:
```bash
deactivate
```
<hr>

## Интерактивные ноутбуки

| Ноутбук                       | Тема                    | Содержание                                                                                                                                                                         | TF-IDF score                     |
| ----------------------------- | ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
| `Text Representation. Part 1` | Векторная модель текста | Стемминг<br>Лемматизация<br>One-Hot Encoding<br>BoW (Bag of Words)<br>BoN (Bag of N Grams)<br>TF-IDF (Term Frequency Inverse Document Frequency)<br>LDA (Latent Semantic Analysis) | NLTK, spaCy, regex, scikit-learn |
| `Text Representation. Part 2` | Векторная модель текста | Word2Vec                                                                                                                                                                           | gensim                           |

