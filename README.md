# PDT Core Module

**Photodynamic Therapy (PDT) Core Module** — медицинский Python-модуль для расчёта дозировки и экспозиции при терапии с фотосенсибилизатором **Radachlorin®**.

## 🧩 Состав модуля
 
- `pdt/models.py` — медданные и структуры (датаклассы) для PDT 
- `pdt/radachlorin.py` — параметры Radachlorin®
- `pdt/calculators.py` — функции расчёта дозы, экспозиции и энергии
- `pdt/enums.py` — справочные константы и перечисления
- `examples/demo_calculators.py` — демонстрация работы калькулятора 
- `README.md` — документация
- `DISCLAIMER.md` — юридические и медицинские предупреждения  

## ⚡ Пример использования

```python
from pdt.calculators import calculate_cervix_fdt

result = calculate_cervix_fdt(length_cm=2.5, power_mw=150, dose_j_cm2=50)
print(result)
Выход:

{'K': 312, 'T_minutes': 18.72, 'minutes': 18, 'seconds': 43}
🚀 Установка и запуск
Клонируем репозиторий:

git clone https://github.com/rolloerro/pdt-core.git
cd pdt-core
Запуск демо-калькулятора:

python3 -m examples.demo_calculators
⚠️ Важно
Этот модуль предназначен только для образовательных и исследовательских целей.
Не использовать в клинической практике без консультации специалиста.

💡 Дальнейшие планы
Добавление ML-модулей для прогнозирования эффективности

Подключение GUI или веб-сервиса

Расширение базы фотосенсибилизаторов


Если хочешь, я могу прямо **сделать второй коммит с этим README** и предложить **красивый вариант для GitHub**, чтобы репо выглядело как настоящий продакшн-модуль.  

Хочешь, чтобы я это сделал сейчас?
Вот полный пример README.md, брат, прямо вставляй — уже готово к пушу:

# PDT Core Module

**Photodynamic Therapy (PDT) Core Module** — медицинский Python-модуль для расчёта дозировки и экспозиции при терапии с фотосенсибилизатором **Radachlorin®**.

---

## 🧩 Состав модуля

- `pdt/models.py` — медданные и структуры (датаклассы) для PDT  
- `pdt/radachlorin.py` — параметры и состав Radachlorin®  
- `pdt/calculators.py` — функции расчёта экспозиции, энергии и времени сеанса  
- `pdt/enums.py` — константы, диффузоры, мощности, дозы  

---

## ⚡ Установка

Клонируем репо:

```bash
git clone https://github.com/rolloerro/pdt-core.git
cd pdt-core
(Модуль пока локальный, можно использовать через PYTHONPATH или устанавливать как пакет.)

🧪 Пример использования
from pdt.calculators import calculate_cervix_fdt

result = calculate_cervix_fdt(length_cm=3.5, power_mw=100, dose_j_cm2=50)
print(result)
Пример запуска демо:

PYTHONPATH=. python3 examples/demo_calculators.py
📚 Лекарственный препарат
Radachlorin® — концентрат для приготовления раствора для инфузий.

Состав на 100 мл концентрата:

Действующее вещество: Radachlorin® 5 г

Сумма натриевых солей хлорина e6, хлорина p6, пурпурина 5 — 0,35 г

Вспомогательные вещества: Меглюмин 0,20 г; вода для инъекций

📝 Лицензия
MIT License — свободно использовать для исследований и обучения.

