# Ilshat Galimov

### Contact information:
* **Phone and Telegram** +7(937)2997666
* **E-mail:** ilshat999.galimov@yandex.ru
* **GitHub:** [i-galimov](https://github.com/i-galimov)

### Education and courses:
* **Bachelor of Management (Kazan Federal University)**
* **Master of Quality Management (Kazan National Research Technological University)**
* [**Skolkovo SKlab Certificate**](https://github.com/i-galimov/My_certificates_and_courses/blob/main/Skolkovo_SClab_Certificate.pdf)
* [**Internet-marketing (Google Skills) Certificate**](https://github.com/i-galimov/My_certificates_and_courses/blob/main/Google_skills_internet_marketing_Certificate.pdf)
* [**Data Science (HSE University)**](https://github.com/i-galimov/My_certificates_and_courses/blob/main/HSE_Data_Science_Certificate.jpg)
* [**Other**](https://github.com/i-galimov/My_certificates_and_courses)

### Skills:
* **HTML**, **Markdown**, **CSS**
* Version control **Git** (remote service GitHub)
* **Python** (basic)
* **C\C++** (basic)
* **Java Script** (basic)
* Relational **SQL** (basic)
* **Shell**

### Code example on C:
```
#include "ft_printf.h"

void	ft_define_print(const char *format, va_list ap, int *i)
{
	if (*format == 'c')
		ft_putchar(va_arg(ap, int), i);
	else if (*format == 's')
		ft_putstr(va_arg(ap, char *), i);
	else if (*format == 'p')
		ft_putpointer(va_arg(ap, unsigned long long), i);
	else if (*format == 'd' || *format == 'i')
		ft_putnbr(va_arg(ap, int), i);
	else if (*format == 'u')
		ft_putplusnbr(va_arg(ap, unsigned int), i);
	else if (*format == 'x')
		ft_lower_hexadecimal(va_arg(ap, unsigned int), i);
	else if (*format == 'X')
		ft_upper_hexadecimal(va_arg(ap, unsigned int), i);
	else if (*format == '%')
		ft_putchar('%', i);
	else
	{
		write(1, format, 1);
		i++;
	}
}

int	ft_printf(const char *format, ...)
{
	va_list	ap;
	int		i;

	i = 0;
	va_start(ap, format);
	while (*format)
	{
		if (*format != '%')
		{
			write(1, format, 1);
			format++;
			i++;
		}
		if (*format == '%')
		{
			ft_define_print(++format, ap, &i);
			format++;
		}
	}
	va_end(ap);
	return (i);
}
```
### Code example on Python:
```
import random

len_all = len(base_dict) 
print(f'Всего {len_all} слов в словаре')
user_input = input('Введите слово или фразу на английском, которые хотите перевести, или цифры, чтобы сгенерировать случайную фразу\n')
check_type = user_input.isdigit()
if check_type == False:
	user_input = user_input.lower().split()
else:
	user_input = int(user_input)

def fn_translate(user_input):
    count_not_dict = 0 
    count_dict = 0 
    for element in user_input:
      if element in base_dict:
      	print(element, base_dict[element])
      	count_dict += 1
      elif element not in base_dict:
      	print(element, "?")
      	count_not_dict += 1
    count_all_dict = count_dict + count_not_dict 
    percent_dict = (count_dict / count_all_dict) * 100 
    print(f'Всего использовано {count_all_dict} слов\nУдалось перевести {count_dict} слов\nНе удалось найти {count_not_dict} слов\nПереведено {percent_dict} процентов текста')

def fn_random_word(user_input):
        if user_input > 50:
        	print("Слишком большое число, придумаем 50 слов")
        	user_input = 50
        while user_input > 0:
        	en_random = random.choice(list(base_dict.keys()))
        	print(en_random)
        	user_input -= 1
		
if check_type == True:
	fn_random_word(user_input)
else:
	fn_translate(user_input)
```
### About Myself:
I am a man of many talents: 
* **Chess** 
* **Basketball** 
* **Table Tennis**
*  **Sales**
*  **Internet Marketing**
*  **Programming**
*  **Guitar**
I am open to new knowledge!

### Work experience:
* ***Telecom Services Sales Agent*** **2014-2020**
* ***Manager Of The Active Sales Group*** **2020-2021**

### Languages:
* **Russian** - native
* **English** - A2
* **Deutsch** - A1

> *"Knowledge is power."* - Francis Bacon

![](https://cdn.pixabay.com/photo/2015/11/19/21/10/glasses-1052010__340.jpg)
