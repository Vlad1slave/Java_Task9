# Completed java task 9

ClassLoader - Загружает классы (JvmComprehension, Object, Integer, System) в метаспейс.

Стэк - Хранит фреймы методов (main, printAll) и локальные переменные (i, o, ii, uselessVar).

Хип - Хранит объекты (new Object(), Integer(2), Integer(700), строки).

Метаспейс - Хранит метаданные классов.

Код:

Строка 1: int i = 1 — в стэке создается переменная i.

Строка 2: Object o = new Object() — в хипе создается объект, ссылка o сохраняется в стэке.

Строка 3: Integer ii = 2 — в хипе создается Integer(2), ссылка ii сохраняется в стэке.

Строка 4: printAll(o, i, ii) — создается фрейм для printAll, аргументы передаются в стэк.

Строка 5: Integer uselessVar = 700 — в хипе создается Integer(700), ссылка uselessVar сохраняется в стэке.

Строка 6: System.out.println(o.toString() + i + ii) — создаются временные строки в хипе, вывод в консоль.

Строка 7: System.out.println("finished") — строка "finished" создается в хипе, вывод в консоль.

Сборщик мусора - После завершения printAll, объект Integer(700) становится недостижимым и может быть удален.
