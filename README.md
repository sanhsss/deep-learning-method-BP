﻿# deep-learning-method-BP
Проект лабораторной работы #1 по курсу "Глубокое обучение"

"Реализация метода обратного распространения ошибки для двуслойной полностью связанной нейронной сети"

## Инструкция по сборке и запуску приложения

1. Перейдите в папку `build` и запустите в ней командную строку
2. В зависимость от версии вашей `Visual Studio` вызовите одну из следующих команд:

	```bash
	cmake -G "Visual Studio 10 2010" ..
	```
	```bash
	cmake -G "Visual Studio 12 2013" ..
	```
	```bash
	cmake -G "Visual Studio 15 2017" ..
	```
	
3. Откройте файл `config.txt` и задайте необходимые параметры. Данный конфигурационный файл имеет следующую структуру:

    - Путь до изображений обучающей выборки
	
			`fileTrainImageMNIST, MNIST_Database/train-images.idx3-ubyte`
	
	- Путь до меток обучающей выборки
	
			`fileTrainLabelsMNIST, MNIST_Database/train-labels.idx1-ubyte`

	- Путь до изображений тестовой выборки
	
			`fileTestImageMNIST, MNIST_Database/t10k-images.idx3-ubyte`

	- Путь до меток тестовой выборки
	
			`fileTestLabelsMNIST, MNIST_Database/t10k-labels.idx1-ubyte`

	- Количество нейронов на скрытом слое
	
			`numberHiddenNeurons, 200`

	- Максимальное число эпох
	
			`numberEpochs, 50`

	- Скорость обучения
	
			`learningRate, 0.008`

	- Требуемая точность
	
			`errorCrossEntropy, 0.005`
	
4. Откройте в `Visual Studio` собранное решение. В свойствах решения укажите, что первым запускаемым проектом должен быть `MethodBackPropagation`.
   Скомпилируйте и запустите приложение.
5. По завершению работы приложение выдаст точность классификации на обучающей и тестовой выборках.

## Отчёт по лабораторной работе

Отчёт с описанием метода обратного распространения ошибки и с кратким описанием программного кода находится в папке `report`.

## Результаты экспериментов

В результате экспериментов удалось получить следующую точность классификации:

	на обучающей выборке: 0.999700
	
	на тестовой выборке: 0.98150
