# checkSystem
Пытаемся сделать проверяющую систему


		/*------------------------
		 * 
		 * Использование: 
		 * 1). Создать экземпляр Tester (работать одновременно будет только один!)
		 * 		Конструктор: new Tester(String путь_до_директории, String название_файла)
		 * 		путь_до_директории: по этому пути должен лежать файл название_файла.java и файл tests.txt
		 * 		путь_до_директории: обязательно абсолютный путь!
		 * 		путь_до_директории: работает только с двойными обратными слешами! C:\\TEST\\
		 * 		путь_до_директории: обязательно заканчивается на обратный слеш!
		 * 2). экземпляр.run_tests();
		 * 		поток заторможен до выполнения всех тестов 
		 * 		(при достижении Time Limit = 1сек выполнение теста прерывается, TL)
		 * 3). t.getResult() возвращает информацию о выполненном тестировании.
		 * 		Формат:
		 * 		TEST: (номер)
		 * 		VERDICT: (результат)
		 * 		SUB: (пояснение)
		 * 
		 *		Результаты:
		 *			OK - успешно
		 *			WA - неверный ответ на тест
		 *			RE - ошибка во время выполнения
		 *			CE - ошибка во время компиляции
		 *			TL - превышено время выполнения (1000сек) 
		 *
		 * 		Пояснения: в случае ОК - время выполнения, в случае ошибки - её содержание
		 * 		
		 * 	Формат файла test.txt:
		 * 	Первая строка: кол-во_тестов/макс_баллы    (например 4/50)
		 * 	Далее такое-же кол-во строк, сколько тестов, формата
		 * 		баллы_за_тест:ВХОДНЫЕ_ДАННЫЕ:ВЫХОДНЫЕ_ДАННЫЕ
		 * 		например 10:2:2 3
		 * 		т.е. за тест получим 10 баллов, входные данные - "2", ожидаемый ответ на тест - "2 3"	
		 * 		данные вводятся и считываются через стандартный поток
		 * 		
		 * 		
		 */
