# Игра "Змейка"

---
Игра "Змейка", где главная цель собрать как можно больше фруктов. Существует три уровня сложности, один из которых игрок выбирает до начала игры. С повышением уровня повышается скорость змеи и количество препядствий. При столкновении со стенкой, камнем или собственным хвостом игра оканчивается, а при подборе фрукта увеличивается размер змеи.

Основной функцией является run(), в которой реализуется игра (с использованием других подфункций). В начале идет инициализация поля
без вывода через функцию initialize_play_field(), в которой голова змейки помещается в середину игрового поля и генерируется фрукт 
через функцию generate_food(). Затем игра переходит в цикл, окончание которого определено столкновением змейки со стеной или своим хвостом. Поле выводится через функцию print_play_field(), в которой определяется выводимый символ через функцию get_play_field_value().
Идет постоянное обновление карты функцией update_field(), в которой используется функция move_snake(), куда передаются значения для постоянного движения змеи основанных на заданном направлении. В этой же функции ( move_snake() ) проходит проверка на условие окончания игры и на наличие подобранного фрукта. 
