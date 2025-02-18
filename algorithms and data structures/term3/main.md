- [1. Обход в глубину](#1-обход-в-глубину)
  - [1.1. Инспектору нужно проверить состояние дорог в городе, для этого он хочет проехать по каждой дороге в каждую сторону (все дороги двусторонние). Постройте кратчайший путь. $\mathcal O(n + m)$](#11-инспектору-нужно-проверить-состояние-дорог-в-городе-для-этого-он-хочет-проехать-по-каждой-дороге-в-каждую-сторону-все-дороги-двусторонние-постройте-кратчайший-путь-mathcal-on--m)
  - [1.2. Правда ли, что если в орграфе существует путь из $u$ в $v$ и время выхода из вершины $u$ больше, чем время выхода из вершины $v$, то $u$ является предком $v$ в дереве обхода в глубину?](#12-правда-ли-что-если-в-орграфе-существует-путь-из-u-в-v-и-время-выхода-из-вершины-u-больше-чем-время-выхода-из-вершины-v-то-u-является-предком-v-в-дереве-обхода-в-глубину)
  - [1.3. Может ли в лесе обхода в глубину получиться дерево из одной вершины, если у этой вершины есть и входящие и исходящие ребра?](#13-может-ли-в-лесе-обхода-в-глубину-получиться-дерево-из-одной-вершины-если-у-этой-вершины-есть-и-входящие-и-исходящие-ребра)
  - [1.4. Удалить из орграфа минимальное число ребер так, чтобы он стал ациклическим.](#14-удалить-из-орграфа-минимальное-число-ребер-так-чтобы-он-стал-ациклическим)
  - [1.5 Правда ли, что для топологической сортировки орграфа можно сортировать не по убыванию времени выхода, а наоборот, по возрастанию времени входа?](#15-правда-ли-что-для-топологической-сортировки-орграфа-можно-сортировать-не-по-убыванию-времени-выхода-а-наоборот-по-возрастанию-времени-входа)
  - [1.6. Запустим алгоритм построения топологической сортировки на орграфе с циклами. Правда ли, что он минимизирует число ребер, ведущих справа налево?](#16-запустим-алгоритм-построения-топологической-сортировки-на-орграфе-с-циклами-правда-ли-что-он-минимизирует-число-ребер-ведущих-справа-налево)
  - [1.7. Покажите, что если делать обход в глубину в неориентированном графе, то перекрестных ребер не будет (то есть каждое ребро соединяет предка с потомком).](#17-покажите-что-если-делать-обход-в-глубину-в-неориентированном-графе-то-перекрестных-ребер-не-будет-то-есть-каждое-ребро-соединяет-предка-с-потомком)
  - [1.8. Проверьте, что в данном орграфе есть только один способ построить топологическую сортировку. $\mathcal O(n + m)$.](#18-проверьте-что-в-данном-орграфе-есть-только-один-способ-построить-топологическую-сортировку-mathcal-on--m)
  - [1.9. Найдите для каждой вершины орграфа самую левую и самую правую из возможных позиций в топологической сортировке. $\mathcal O(nm)$.](#19-найдите-для-каждой-вершины-орграфа-самую-левую-и-самую-правую-из-возможных-позиций-в-топологической-сортировке-mathcal-onm)
    - [Идея](#идея)
    - [Реализация](#реализация)
    - [Построение _(доказательство существования)_](#построение-доказательство-существования)
  - [1.10. Постройте лексографически минимальную топологическую сортировку (если представлять топологическую сортировку как последовательность номеров вершин). $\mathcal O((n + m) \log n)$.](#110-постройте-лексографически-минимальную-топологическую-сортировку-если-представлять-топологическую-сортировку-как-последовательность-номеров-вершин-mathcal-on--m-log-n)
  - [1.11. Постройте в заданном ацикличном орграфе гамильтонов путь, или скажите, что его нет. $\mathcal O(n + m)$.](#111-постройте-в-заданном-ацикличном-орграфе-гамильтонов-путь-или-скажите-что-его-нет-mathcal-on--m)
  - [1.12. Найти в ациклическом взвешенном орграфе кратчайший путь из s в t. $\mathcal O(n + m)$.](#112-найти-в-ациклическом-взвешенном-орграфе-кратчайший-путь-из-s-в-t-mathcal-on--m)
  - [1.13. Модифицируйте алгоритм поиска цикла, чтобы он искал любой простой цикл в заданном неориентированном графе.](#113-модифицируйте-алгоритм-поиска-цикла-чтобы-он-искал-любой-простой-цикл-в-заданном-неориентированном-графе)
  - [1.14. Транзитивным замыканием графа называется такой граф, в котором ребро $(u, v)$ есть тогда и только тогда, когда в исходном графе есть путь из $u$ в $v$. Построить транзитивное замыкание. $\mathcal O(nm)$.](#114-транзитивным-замыканием-графа-называется-такой-граф-в-котором-ребро-u-v-есть-тогда-и-только-тогда-когда-в-исходном-графе-есть-путь-из-u-в-v-построить-транзитивное-замыкание-mathcal-onm)
  - [1.15. Транзитивным остовом графа называется минимальный граф, транзитивное замыкание которого совпадает с транзитивным замыканием исходного графа. Построить транзитивный остов. $\mathcal O(nm)$.](#115-транзитивным-остовом-графа-называется-минимальный-граф-транзитивное-замыкание-которого-совпадает-с-транзитивным-замыканием-исходного-графа-построить-транзитивный-остов-mathcal-onm)
- [2. Компоненты сильной связности](#2-компоненты-сильной-связности)
  - [2.1. Дан ориентированный граф. Какое минимальное число ребер нужно добавить в него, чтобы он стал сильно связным?](#21-дан-ориентированный-граф-какое-минимальное-число-ребер-нужно-добавить-в-него-чтобы-он-стал-сильно-связным)
  - [2.2. Дан ориентированный граф. Постройте граф, с таким же множеством вершин и минимальным числом ребер, чтобы его конденсация совпадала с конденсацией данного графа.](#22-дан-ориентированный-граф-постройте-граф-с-таким-же-множеством-вершин-и-минимальным-числом-ребер-чтобы-его-конденсация-совпадала-с-конденсацией-данного-графа)
  - [2.3. В городе n перекрестков, соединенных m односторонними дорогами. Нужно установить в городе несколько пунктов быстрого реагирования. Установить пункт на перекрестке i стоит ci рублей. Сколько денег нужно потратить, чтобы до каждого перекрестка можно было бы доехать хотя бы из одного построенного пункта?](#23-в-городе-n-перекрестков-соединенных-m-односторонними-дорогами-нужно-установить-в-городе-несколько-пунктов-быстрого-реагирования-установить-пункт-на-перекрестке-i-стоит-ci-рублей-сколько-денег-нужно-потратить-чтобы-до-каждого-перекрестка-можно-было-бы-доехать-хотя-бы-из-одного-построенного-пункта)
  - [2.4. Для каждой вершины графа найти вершину с минимальным номером, достижимую из нее.](#24-для-каждой-вершины-графа-найти-вершину-с-минимальным-номером-достижимую-из-нее)
  - [2.5. Турниром называется ориентированный граф, в котором каждая пара вершин соединена ребром (в одну или другую сторону). Докажите, что в сильно связном турнире есть гамильтонов цикл.](#25-турниром-называется-ориентированный-граф-в-котором-каждая-пара-вершин-соединена-ребром-в-одну-или-другую-сторону-докажите-что-в-сильно-связном-турнире-есть-гамильтонов-цикл)
  - [2.6. Докажите, что если в каждой вершине турнира число входящих и исходящих ребер одинаково, то турнир сильно связен.](#26-докажите-что-если-в-каждой-вершине-турнира-число-входящих-и-исходящих-ребер-одинаково-то-турнир-сильно-связен)
  - [2.7. Дано число n и и m пар (ai, bi). Нужно построить ориентированный граф на n вершинах с минимальным числом ребер, в котором для каждой пары существует путь из ai в bi.](#27-дано-число-n-и-и-m-пар-ai-bi-нужно-построить-ориентированный-граф-на-n-вершинах-с-минимальным-числом-ребер-в-котором-для-каждой-пары-существует-путь-из-ai-в-bi)
- [6. Еще задачи на DFS и все такое](#6-еще-задачи-на-dfs-и-все-такое)
  - [6.1. Неориентированный граф называется реберным кактусом, если каждое ребро содержится не более чем в одном простом цикле. Проверить, что данный граф является реберным кактусом. Время $O(m)$.](#61-неориентированный-граф-называется-реберным-кактусом-если-каждое-ребро-содержится-не-более-чем-в-одном-простом-цикле-проверить-что-данный-граф-является-реберным-кактусом-время-om)
  - [6.2. Неориентированный граф называется вершинным кактусом, если каждая вершина содержится не более чем в одном простом цикле. Проверить, что данный граф является вершинным кактусом. Время $O(m)$.](#62-неориентированный-граф-называется-вершинным-кактусом-если-каждая-вершина-содержится-не-более-чем-в-одном-простом-цикле-проверить-что-данный-граф-является-вершинным-кактусом-время-om)
  - [6.3. Дан вершинный кактус, нужно быстро отвечать на запросы вида: найти число различных реберно простых путей из $u$ в $v$. Предподсчет $O(n \log n)$, запросы за $O(\log n)$.](#63-дан-вершинный-кактус-нужно-быстро-отвечать-на-запросы-вида-найти-число-различных-реберно-простых-путей-из-u-в-v-предподсчет-on-log-n-запросы-за-olog-n)
  - [6.4. Дан реберный кактус. Каждое ребро uv удаляется с вероятностью $p_{uv}$. Найти вероятность того, что граф останется связным после удаления ребер. Время $O(m)$.](#64-дан-реберный-кактус-каждое-ребро-uv-удаляется-с-вероятностью-p_uv-найти-вероятность-того-что-граф-останется-связным-после-удаления-ребер-время-om)
  - [6.5. Дан неориентированный граф. Нужно выбрать в нем две вершины, между которыми есть три вершинно непересекающихся пути (кроме концов), или сказать, что это сделать нельзя. Время O(m log n).](#65-дан-неориентированный-граф-нужно-выбрать-в-нем-две-вершины-между-которыми-есть-три-вершинно-непересекающихся-пути-кроме-концов-или-сказать-что-это-сделать-нельзя-время-om-log-n)
  - [6.6. Дан ориентированный граф. Найти все такие вершины v, что для любой вершины u существует путь либо из u в v, либо из v в u. Время O(m log n).](#66-дан-ориентированный-граф-найти-все-такие-вершины-v-что-для-любой-вершины-u-существует-путь-либо-из-u-в-v-либо-из-v-в-u-время-om-log-n)
  - [6.7. Дан неориентированный граф. Найти все такие ребра, при удалении которых граф становится двудольным. Время O(m log n).](#67-дан-неориентированный-граф-найти-все-такие-ребра-при-удалении-которых-граф-становится-двудольным-время-om-log-n)
  - [6.8. Есть n лампочек, некоторые из которых включены, а некоторые выключены, и m переключателей. Каждый переключатель меняет состояние какого-то подмножества лампочек, при этом для каждой лампочки есть не более двух переключателей, которые меняют ее состояние. Проверить, можно ли выключить все лампочки. Время O(m + n).](#68-есть-n-лампочек-некоторые-из-которых-включены-а-некоторые-выключены-и-m-переключателей-каждый-переключатель-меняет-состояние-какого-то-подмножества-лампочек-при-этом-для-каждой-лампочки-есть-не-более-двух-переключателей-которые-меняют-ее-состояние-проверить-можно-ли-выключить-все-лампочки-время-om--n)
  - [6.9. Есть булева функция в виде 2-КНФ для n+m переменных. Проверить, что для любых значений x1, x2, . . . , xn существуют значения xn+1, xn+2, . . . , xn+m, при которых функция выполняется.](#69-есть-булева-функция-в-виде-2-кнф-для-nm-переменных-проверить-что-для-любых-значений-x1-x2-----xn-существуют-значения-xn1-xn2-----xnm-при-которых-функция-выполняется)
- [9 Обход в ширину](#9-обход-в-ширину)
  - [9.1. Дан ориентированный граф. Найдите все ребра, для которых существует кратчайший путь из s в t, который через него проходит.](#91-дан-ориентированный-граф-найдите-все-ребра-для-которых-существует-кратчайший-путь-из-s-в-t-который-через-него-проходит)
  - [9.2. Дан ориентированный граф. Найдите минимальное число ребер, которое нужно развернуть, чтобы был путь из s в t.](#92-дан-ориентированный-граф-найдите-минимальное-число-ребер-которое-нужно-развернуть-чтобы-был-путь-из-s-в-t)
  - [9.3. Дан ориентированный граф. Разрешается развернуть не более одного ребра, требуется, чтобы расстояние от s до t было минимально.](#93-дан-ориентированный-граф-разрешается-развернуть-не-более-одного-ребра-требуется-чтобы-расстояние-от-s-до-t-было-минимально)
  - [9.4.](#94)
  - [9.5.](#95)
  - [10.2](#102)
  - [10.3](#103)

## 1. Обход в глубину

### 1.1. Инспектору нужно проверить состояние дорог в городе, для этого он хочет проехать по каждой дороге в каждую сторону (все дороги двусторонние). Постройте кратчайший путь. $\mathcal O(n + m)$

dfs.

### 1.2. Правда ли, что если в орграфе существует путь из $u$ в $v$ и время выхода из вершины $u$ больше, чем время выхода из вершины $v$, то $u$ является предком $v$ в дереве обхода в глубину?

Если в разных деревьях леса дфс, то нет.

Если $u\to v$ - перекрестное, то нет.

### 1.3. Может ли в лесе обхода в глубину получиться дерево из одной вершины, если у этой вершины есть и входящие и исходящие ребра?

![](images/1.3.drawio.svg)

Последовательность вызовов: `dfs(y), dfs(x), dfs(z)`

### 1.4. Удалить из орграфа минимальное число ребер так, чтобы он стал ациклическим.

1. Создаем лес обхода графа.
2. В каждой компоненте:
   1. Находим LCA всех стартовых вершин обратных ребер $=a$
   2. Находим свою смерть что за гроб

[Тут есть описание](https://math.stackexchange.com/questions/2997412/fast-algorithm-to-remove-edge-to-get-dag)

### 1.5 Правда ли, что для топологической сортировки орграфа можно сортировать не по убыванию времени выхода, а наоборот, по возрастанию времени входа?

Нет:

![](images/1.5.drawio.svg)

### 1.6. Запустим алгоритм построения топологической сортировки на орграфе с циклами. Правда ли, что он минимизирует число ребер, ведущих справа налево?

Нет, если его запускать от разных вершин???

### 1.7. Покажите, что если делать обход в глубину в неориентированном графе, то перекрестных ребер не будет (то есть каждое ребро соединяет предка с потомком).

Предположим, что в дереве обхода есть перекрестное ребро $a-b$. Пусть в $a$ пришли раньше, чем в $b$. Тогда, когда пришли в $a$, должно было быть проведено ребро $a-b$ и это ребро не было бы перекрестным - противоречие.

### 1.8. Проверьте, что в данном орграфе есть только один способ построить топологическую сортировку. $\mathcal O(n + m)$.

Если топсорт не образует гамильтонов путь, то (по 11) $\exists i : i \not\to (i+1)$ и эти вершины можно переставить. Если топсорт образует гамильтонов путь, то он единственный, т.к. любая перестановка $i$ с $j$ ($i<j$) не является топсортом, т.к. $j$ зависит от $i$.

Другое решение: проверка `queue.size == 1`

### 1.9. Найдите для каждой вершины орграфа самую левую и самую правую из возможных позиций в топологической сортировке. $\mathcal O(nm)$.

#### Идея

- Самая левая позиция - число вершин ($+1$), из которых можно достичь $x$, т.к. $x$ должна стоять после этих вершин.
- Самая правая позиция _(если считать справа)_ - число достижимых вершин ($+1$) из $x$, т.к. любую из этих вершин нельзя поставить раньше, чем $x$.

#### Реализация

- Число достижимых вершин из $x$ считается через dfs c счётчиком вершин, в которые мы зашли.
- Число вершин, из которых достижима $x$ считается разворачиванием графа и аналогичным dfs.

#### Построение _(доказательство существования)_

- Левая: возьмём все вершины, из которых достижим $x$. Топсортнем, присоединим $x$ на последнее место. После присоединения топсорт все ещё верный, т.к. для $x$ требование выполнено, для остальных нет изменений. Остальные вершины тоже можно присоединить.
- Правая: аналогично.

### 1.10. Постройте лексографически минимальную топологическую сортировку (если представлять топологическую сортировку как последовательность номеров вершин). $\mathcal O((n + m) \log n)$.

Условие непонятно

### 1.11. Постройте в заданном ацикличном орграфе гамильтонов путь, или скажите, что его нет. $\mathcal O(n + m)$.

Топологическая сортировка -> получаем последовательность номеров вершин. Путь существует, только если $\forall i \ \ \exist i \to (i+1)$, потому что если пути $i \to (i+1)$ нет, то после ухода из $i$ мы не вернемся в $i+1$, т.к. попадем хотя бы в $i+2$, откуда нельзя прийти в $i+1$ по определению топсорта. Сам путь - последовательность всех ребер $i\to(i+1)$

### 1.12. Найти в ациклическом взвешенном орграфе кратчайший путь из s в t. $\mathcal O(n + m)$.

Линейный дп по топсорту.

```c
sorted = topsort()
ss = sorted[s]
ts = sorted[t]
dp.fill(+inf)
dp[ss] = 0
calc(ss)
return dp[ts]

calc(node):
   for (child, weight) in node.out:
      dp[child] = min(dp[node] + weight, dp[child])
      calc(child)
```

### 1.13. Модифицируйте алгоритм поиска цикла, чтобы он искал любой простой цикл в заданном неориентированном графе.

dfs, помечая пройденные ребра и кладя ребра в стек рекурсии. Если перешли по помеченному ребру, то есть цикл. В таком случае убираем ребра со стека (запоминая вершины), пока не встретим ребро, по которому перешли.

```c
dfs(node, parent):
   for edge in node.out:
      if visited[edge] and edge != { node, parent }:
         cycle = [node]
         cycle_set = {node}
         while true:
            curr = stack.pop()
            if curr == edge:
               return cycle
            if curr.left in cycle_set:
               cycle += curr.right
            if curr.right in cycle_set:
               cycle += curr.left
            // других случаев нет
      else:
         stack.push(edge)
         if edge.left == node:
            dfs(edge.right, node)
         else:
            dfs(edge.left, node)
         stack.pop()
```

### 1.14. Транзитивным замыканием графа называется такой граф, в котором ребро $(u, v)$ есть тогда и только тогда, когда в исходном графе есть путь из $u$ в $v$. Построить транзитивное замыкание. $\mathcal O(nm)$.

```c
for u in V:
   reachable.fill(false)
   dfs(u)
   for v in V:
      if reachable[v]:
         E.add(u, v)
```

### 1.15. Транзитивным остовом графа называется минимальный граф, транзитивное замыкание которого совпадает с транзитивным замыканием исходного графа. Построить транзитивный остов. $\mathcal O(nm)$.

## 2. Компоненты сильной связности

### 2.1. Дан ориентированный граф. Какое минимальное число ребер нужно добавить в него, чтобы он стал сильно связным?

<!-- Сначала сконденсируем граф. От этой операции искомое очевидно не изменилось. Пусть $a$ - число КСС, в которые не входят ребра - $\ge$, чем число КСС, из которых не исходят ребра. Обратный случай - то же самое с точностью до разворота графа. -->

### 2.2. Дан ориентированный граф. Постройте граф, с таким же множеством вершин и минимальным числом ребер, чтобы его конденсация совпадала с конденсацией данного графа.

### 2.3. В городе n перекрестков, соединенных m односторонними дорогами. Нужно установить в городе несколько пунктов быстрого реагирования. Установить пункт на перекрестке i стоит ci рублей. Сколько денег нужно потратить, чтобы до каждого перекрестка можно было бы доехать хотя бы из одного построенного пункта?

### 2.4. Для каждой вершины графа найти вершину с минимальным номером, достижимую из нее. 

Конденсация, будем загонять дфс от всех вершин, не заходя в уже помеченные. Минимум из детей дает минимум в искомой.

### 2.5. Турниром называется ориентированный граф, в котором каждая пара вершин соединена ребром (в одну или другую сторону). Докажите, что в сильно связном турнире есть гамильтонов цикл.

### 2.6. Докажите, что если в каждой вершине турнира число входящих и исходящих ребер одинаково, то турнир сильно связен.

### 2.7. Дано число n и и m пар (ai, bi). Нужно построить ориентированный граф на n вершинах с минимальным числом ребер, в котором для каждой пары существует путь из ai в bi.

## 6. Еще задачи на DFS и все такое

### 6.1. Неориентированный граф называется реберным кактусом, если каждое ребро содержится не более чем в одном простом цикле. Проверить, что данный граф является реберным кактусом. Время $O(m)$.

Поделим на компоненты реберной двусвязности в линию через dfs: [вики](https://en.wikipedia.org/wiki/Biconnected_component) и для каждой компоненты проверим, является ли она $C_k$ или одним ребром.

### 6.2. Неориентированный граф называется вершинным кактусом, если каждая вершина содержится не более чем в одном простом цикле. Проверить, что данный граф является вершинным кактусом. Время $O(m)$.

Поделим на компоненты вершинной двусвязности в линию через dfs в реберном графе. Аналогично предыдущей задаче.

### 6.3. Дан вершинный кактус, нужно быстро отвечать на запросы вида: найти число различных реберно простых путей из $u$ в $v$. Предподсчет $O(n \log n)$, запросы за $O(\log n)$.

Сжимаем компоненты вершинной двусвязности, каждый цикл - 2, остальное - 1. LCA через двоичные подъемы.

### 6.4. Дан реберный кактус. Каждое ребро uv удаляется с вероятностью $p_{uv}$. Найти вероятность того, что граф останется связным после удаления ребер. Время $O(m)$.

Найдем все циклы dfs-ом
$$\prod_{C} \left(\prod_{e\in C} (1-p_{e}) + \prod_{e\in C} \left(p_{e}\prod_{f\in C, f\not=e} (1-p_{f})\right)\right)$$

Очев это не считается в линию, но если запоминать $\prod_{v, u\in C} (1-p_{vu})$ для подсчета правой части, то считается.

### 6.5. Дан неориентированный граф. Нужно выбрать в нем две вершины, между которыми есть три вершинно непересекающихся пути (кроме концов), или сказать, что это сделать нельзя. Время O(m log n).

### 6.6. Дан ориентированный граф. Найти все такие вершины v, что для любой вершины u существует путь либо из u в v, либо из v в u. Время O(m log n).

### 6.7. Дан неориентированный граф. Найти все такие ребра, при удалении которых граф становится двудольным. Время O(m log n).

### 6.8. Есть n лампочек, некоторые из которых включены, а некоторые выключены, и m переключателей. Каждый переключатель меняет состояние какого-то подмножества лампочек, при этом для каждой лампочки есть не более двух переключателей, которые меняют ее состояние. Проверить, можно ли выключить все лампочки. Время O(m + n).

### 6.9. Есть булева функция в виде 2-КНФ для n+m переменных. Проверить, что для любых значений x1, x2, . . . , xn существуют значения xn+1, xn+2, . . . , xn+m, при которых функция выполняется.

## 9 Обход в ширину

### 9.1. Дан ориентированный граф. Найдите все ребра, для которых существует кратчайший путь из s в t, который через него проходит.

Дэйкстра и идём назад от $t$ по всем ребрам $e=u\to v$, для которых $w(v) - w(e) = w(u)$.

### 9.2. Дан ориентированный граф. Найдите минимальное число ребер, которое нужно развернуть, чтобы был путь из s в t.

Построим два множества $A$ и $B$ - вершины, достижимые из $s$ по прямым ребрам и
из $t$ по обратным. Найдем минимальное расстояние от $B$ до $A$. Это очевидно
находится, если добавить $a$ и $b$, такие что $a$ соединено со всеми вершинами
$A$, $b$ - со всеми вершинами $B$. Тогда найдем путь $a\to b$ минимальной длины
(не считая ребра $a\to A, b\to B$), получим искомое.

### 9.3. Дан ориентированный граф. Разрешается развернуть не более одного ребра, требуется, чтобы расстояние от s до t было минимально.

Построим граф $\mathfrak G$, который содержит в себе граф $G$ и еще копию этого
графа $G'$. $v\to u'$ ($v\in G, u'\in G'$) $\Leftrightarrow \exists uv\in G$.
Тогда кратчайший путь будет между $s$ и $t'$.

### 9.4.

Развернем граф, запустим Дейкстру $t\to s$, пойдем назад от $s$, как в 9.1, но
будем брать минимальное (лексикографически) ребро.

### 9.5.

Построим граф $0\ldots M-1$, в нём $M$ вершин и $2M$ ребер. Найдем кратчайший
путь в линию через bfs.

### 10.2

https://cs.stackexchange.com/questions/118336/dijkstra-with-max-instead-of-sum

### 10.3

dfs находит ребра, достижимые из $s$ = $A$, достижимые по обратным из $t$ = $B$.


$\forall P : s\rightsquigarrow t P\subset A\cap B$. Тогда найдём минимальное
ребро $\in A\cap B$ и построим произвольный путь, который проходит по этому ребру.