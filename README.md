# base64_encode_decode
Кодировка Base64 позволяет преобразовывать байты, содержащие двоичные или текстовые данные, в символы ASCII

Данная программа представляет собой приложение с графическим интерфейсом для кодирования и декодирования произовльных файлов на основе алгоритма Base64

Для компиляции этой программы у вас должны быть установлены Python версии 3.9

# Функционал:

-Кодирование, декодирование

-Работа с любым типом файлов

-GUI с модулем tkinter

# Запуск проекта на вашем компьютере:

git clone https://github.com/GeroinovayaLady/base64_encode_decode.git 

Запуск модуля графического взаимодействия пользователя с файлами:

	python Interface.py 

# Краткое описание алгоритма:
1.	входные данные представляются в двоичном формате (потоке битов)
2.	последовательность разбивается на блоки по 6 бит каждый
3.	если количество полученных блоков не делится 6, то в конец последовательности дописываются нулевые блоки по 8 бит в таком количестве, чтобы их число было кратно 6
4.	фрагменты 6-битных двоичных данных преобразовываются в формат десятичных чисел;
5.	по значению каждого блока определяется соответствующий ему символ, согласно индексам алфавита base64. Блоки с нулевыми битами, которые добавлялись в конец определяются символом “=”
