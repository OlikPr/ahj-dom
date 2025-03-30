### Перемещение элемента

[![Build status](https://ci.appveyor.com/api/projects/status/ym1tnda9jkg1ki9b?svg=true)](https://ci.appveyor.com/project/EvgeniyPryanichnikov/ahj-dom-t447b)

deployment:
#### Легенда

Игра на подобие игры, где гномы или другие существа выскакивают из отверстий, и по ним нужно бить молотком:

![](./src/img/GracefulMiniatureBustard-small.gif)

Copyright gfycat.com

#### Описание

Инфраструктура проекта собрана на базе Webpack, ESLint, Babel, Jest, Webpack Dev Server.
Реализована лишь первую часть этой игры — перемещение объекта в DOM Tree.

Игровое поле 4x4 и персонаж в виде картинки `img`. При загрузке страницы персонаж программно генерируется и ставится в рандомную позицию внутри игрового поля. С помощью функции `setInterval`  существующий объект `img` перемещается в другое поле. Алгоритм — рандомное перемещение, без перемещения в то же самое поле.

Для картинки персонажа используете следующая:

![](./src/img/goblin.png)


Всё собирается через Webpack, включая картинки и стили, и выкладывается на GitHub Pages через CI.