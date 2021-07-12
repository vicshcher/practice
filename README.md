# РУКОВОДСТВО К ИСПОЛЬЗОВАНИЮ

Для быстрого построения графов можно использовать данную утилиту: **http://magjac.com/graphviz-visual-editor/**. 
Для этого необходимо открыть нужный .dot файл любым текстовым редактором и скопировать все содержимое в текстовое поле утилиты.

# Как использовать программу:

dijkstra.exe и требуемый .dot файл должны лежать в одной папке. При запуске программа требует имя .dot файла с графом, оно вводится **с расширением** (например, "test.dot"). 

Далее, требуются имена вершин, между которыми нужно построить путь, они вводятся в соответствии с их именованием в .dot файле. 

В завершении, если загруженный граф отвечает требованиям, программа запрашивает имя файла для вывода. 
Файл содержит исходный граф, в котором вершины и ребра оптимального пути подсвечены **зеленым** цветом. 

# Требования к графу

- Граф должен быть неориентированным (в .dot файле он будет обозначен как **graph**, но не как **digraph**);

- Все ребра графа должны иметь вес (атрибут **[weight = ...]** в .dot файле). Если у какого то ребра не указан его вес, он принимается равным **0**;

- Мультиграфы не поддерживаются (кратные ребра и петли).