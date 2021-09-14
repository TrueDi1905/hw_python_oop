# calculator
### Описание
Калькулятор денег и калорий
### Технологии
Python 3.7
### Инструкция

#### Калькулятор денег умеет:
- Сохранять новую запись о расходах методом add_record()
- Считать, сколько денег потрачено сегодня методом get_today_stats()
- Определять, сколько ещё денег можно потратить сегодня в рублях, долларах или евро — метод get_today_cash_remained(currency)
- Считать, сколько денег потрачено за последние 7 дней — метод get_week_stats()
#### Калькулятор калорий умеет:
- Сохранять новую запись о приёме пищи— метод add_record()
- Считать, сколько калорий уже съедено сегодня — метод get_today_stats()
- Определять, сколько ещё калорий можно/нужно получить сегодня — метод get_calories_remained()
- Считать, сколько калорий получено за последние 7 дней — метод get_week_stats()
#### Пример использования.
#Создадим калькулятор денег
cash_calculator = CashCalculator(1000)


    cash_calculator.add_record(Record(amount=145, comment="кофе"))
    cash_calculator.add_record(Record(amount=300, comment="Серёге за обед"))
    cash_calculator.add_record(Record(amount=3000, comment="бар в Танин др", date="08.11.2019"))
    print(cash_calculator.get_today_cash_remained("usd"))
### Автор
Агафонов Дмитрий
