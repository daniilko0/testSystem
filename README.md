
testSystem v3.0

Тестовая система, позволяющая практически любому пользователю (нужны лишь минимальные знания jQuery и умение следовать инструкциям) создать свой тест.

Известные проблемы:
1. Не работает кнопка "Еще раз"

Как подключить?

(В этой версии проще всего изменять исходники самостоятельно). Для этого:
1. Откройте файл testV3.js 
2. В функции variables() измените значения нужных переменных:

 $currentQuestion - номер текущего вопроса. Если тест должен начинаться с первого вопроса, не меняйте

 $amountOfQuestions - общее количество вопросов, укажите свое (значение должно соответствовать количеству вопросов в массиве $quiz (об этом ниже)

 $amountOfTrueAnswers - количество верных ответов, изменяется программно

 $quiz - массив перечислений, содержащий непосредственно вопросы:

 "question" - текст вопроса

 "questionImg" - фотография к вопросу, указывается путь к фотографии относительно HTML (используется параллельно с текстовым вопросом)

 "textAnswers" - текстовые варианты ответов. Указываются внутри квадратных скобок, каждый вариант - в отдельных кавычках (взаимозаменяемые с "imgAnswers" )

 "imgAnswers" - варианты ответов картинками. Указываются внутри квадратных скобок, каждый вариант - в отдельных кавычках. Путь к фотографиям относительно HTML (взаимозаменяемые с "textAnswers" )

 "trueAnswer" - переменная (от $a0 до $a3), в котором находится верный вариант ответа

      $a0 - Первый вариант ответа
      $a1 - Второй вариант ответа
      $a2 - Третий вариант ответа
      $a3 - Четвертый вариант ответа



Описание одного вопроса находится в рамках одной пары фигурных скобок

После изменения необходимых переменных тест будет готов к работе!
