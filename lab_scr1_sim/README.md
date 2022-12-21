# Проектирование систем на кристалле <br> Лабораторная работа №2

## Задание

Модифицировать обработку исключений в ядре `SCR1` в соответствии с вариантом задания.

Необходимо отредактировать список тестов, модифицировать обработку исключений `trap_vector`, установить параметры ядра `Reset Vector` и `Trap Vector`, а также изменить linker-скрипт для корректного запуска теста.

Вариант | Вид исключения |  Тест  | Reset Vector | Trap Vector | Обработчик
:-----: |:-------------: | :----: | :----------: | :---------: | :--------:
7  | Illegalinstruction | `isa/rv32mi/illegal.S` | 0x600 | 0x300 | Вывод строки `instructionillegal`

## Результаты работы

![image](https://user-images.githubusercontent.com/110569071/208876923-a6ec0a95-069f-4ec2-ac74-edba44012d60.png)

Результаты симуляции: [sim_results.txt](results/sim_results.txt) и [simx.vcd](results/simx.vcd)  
Дамп-файл теста: [illegal.dump](results/illegal.dump)
