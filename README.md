# Упорядочение объектов на основе схемы Беллмана – Заде

## Постановка задачи

Определить, является ли заданный граф двудольным.Федерация фигурного катания некоторого государства решила, что по результатам ближайших Олимпийских игр у государства должен быть олимпийский чемпион. Предложить множество возможных альтернатив X, множество возможных критериев P.

<table>
    <colgroup>
        <col colspan="2" style="background:Khaki"><!-- С помощью этой конструкции задаем цвет фона для первых двух столбцов таблицы-->
        <col style="background-color:LightCyan"><!-- Задаем цвет фона для следующего (одного) столбца таблицы-->
    </colgroup>
    <thead>
        <tr>
            <th  colspan="2" align="center">Число элементов в множествах</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td align="center">X</td><td align="center">P</td>
        </tr>
        <tr>
            <td align="center">7</td><td align="center">5</td>
        </tr>
    </tbody>
</table>

#### Число элементов в множестве

<table>
    <tr>
        <th  rowspan=2 align="center">Критерии</th><th  colspan=7 align="center">Критерии</th>
    </tr>
    <tbody>
        <tr>
            <td align="center">1 спортсмен</td>
            <td align="center">2 спортсмен</td>
            <td align="center">3 спортсмен</td>
            <td align="center">4 спортсмен</td>
            <td align="center">5 спортсмен</td>
            <td align="center">6 спортсмен</td>
            <td align="center">7 спортсмен</td>
        </tr>
        <tr>
            <td align="center">Скорость</td>
            <td align="center">4</td>
            <td align="center">3</td>
            <td align="center">6</td>
            <td align="center">5</td>
            <td align="center">7</td>
            <td align="center">8</td>
            <td align="center">2</td>
        </tr>
        <tr>
            <td align="center">Гибкость</td>
            <td align="center">2</td>
            <td align="center">6</td>
            <td align="center">4</td>
            <td align="center">3</td>
            <td align="center">5</td>
            <td align="center">7</td>
            <td align="center">8</td>
        </tr>
        <tr>
            <td align="center">Музыка</td>
            <td align="center">8</td>
            <td align="center">2</td>
            <td align="center">7</td>
            <td align="center">6</td>
            <td align="center">4</td>
            <td align="center">3</td>
            <td align="center">5</td>
        </tr>
        <tr>
            <td align="center">Техничность исполнения</td>
            <td align="center">5</td>
            <td align="center">7</td>
            <td align="center">4</td>
            <td align="center">8</td>
            <td align="center">2</td>
            <td align="center">6</td>
            <td align="center">3</td>
        </tr>
        <tr>
            <td align="center">Мастерство</td>
            <td align="center">3</td>
            <td align="center">4</td>
            <td align="center">5</td>
            <td align="center">2</td>
            <td align="center">8</td>
            <td align="center">3</td>
            <td align="center">6</td>
        </tr>
    </tbody>
</table>

<table>
  <caption>Меню ресторана "Ромашка"</caption> 
  <tr>
    <th rowspan="2" class="first">Кухня</th>
    <th colspan="2">Холодные блюда</th>
    <th colspan="2">Горячие блюда</th>
    <th rowspan="2">Десерты</th>
  </tr>
  <tr>
    <td class="first">Салаты</td>
    <td class="first">Закуски</td>
    <td class="first">Первые блюда</td>
    <td class="first">Вторые блюда</td>
  </tr>
  <tr>
    <td rowspan="3" class="first">Русская</td>
    <td>Винегрет</td>
    <td>Язык с хреном</td>
    <td>Щи с квашеной капустой</td>
    <td>Вареники с картошкой</td>
    <td>Печеные яблоки с медом</td>
  </tr>
  <tr>
    <td>Оливье</td>
    <td>Студень говяжий</td>
    <td>Рассольник домашний</td>
    <td>Караси запеченые в сметане</td>
    <td>Блинчатый пирог</td>
  </tr>
  <tr>
    <td>Сельдь под "шубой"</td>
    <td>Судак заливной</td>
    <td>Мясная солянка</td>
    <td>Котлеты "Пожарские"</td>
    <td>Пирожное "Картошка"</td>
    </tr>
  <tr>
    <td rowspan="3" class="first">Испанская</td>
    <td>Севиче из гребешков</td>
    <td>Эмпанадас</td>
    <td>Хлебный суп с чесноком</td>
    <td>Паэлья с морепродуктами</td>
    <td>Чуррос</td>
    </tr>
  <tr>
    <td>Тимбал из авокадо и тунца</td>
    <td>Ахотомате</td>
    <td>Астурийская фабада</td>
    <td>Свиное раксо</td>
    <td>Альмойшавена</td>
    </tr>
  <tr>
    <td>Фасоль с ветчиной</td>
    <td>Чанфайна</td>
    <td>Рыбный суп с манными клецками </td>
    <td>Тортилья картофельная</td>
    <td>Бунуэлос</td>
    </tr>
  <tr>
    <td rowspan="3" class="first">Французская</td>
    <td>Вогезский салат</td>
    <td>Рийет из курицы</td>
    <td>Баклажанный крем-суп "Ренуар"</td>
    <td>Картофель огратен</td>
    <td>Бриоши</td>
    </tr>
  <tr>
    <td>Салат "Панзанелла"</td>
    <td>Делисьез из сыра</td>
    <td>Французский тыквенный суп</td>
    <td>Гратин из птицы</td>
    <td>Лигурийский лимонный пирог</td>
    </tr>
  <tr>
    <td>Тар-тар</td>
    <td>Маринованный лосось</td>
    <td>Суп "Конти"</td>
    <td>Тартифлетт</td>
    <td>Саварен "Триумф"</td>
    </tr>
  </table>

## Описание используемых структур данных

Принцип Беллмана-Заде, как правило, применяется совместно с методом иерархий Т. Саати, что позволяет находить степени принадлежности элементов нечетких множеств с помощью процедуры парных сравнений вариантов. Метод иерархий предусматривает формирование матрицы парных сравнений, проверку ее согласованности и отыскание собственного вектора, который определяет искомые степени принадлежности.

Применяются простые расчетные соотношения, содержащие сравнения с наихудшей альтернативой и наименее важным критерием.

## Тестирование

Тестирование проведено на различных входных данных. Ошибок не найдено!

![alt tag](https://github.com/Basharov1210/multi-criteria_optimization/blob/main/img/test_1.png "Тестирование")

![alt tag](https://github.com/Basharov1210/multi-criteria_optimization/blob/main/img/test_2.png "Тестирование")

![alt tag](https://github.com/Basharov1210/multi-criteria_optimization/blob/main/img/test_3.png "Тестирование")

![alt tag](https://github.com/Basharov1210/multi-criteria_optimization/blob/main/img/test_4.png "Тестирование")

![alt tag](https://github.com/Basharov1210/multi-criteria_optimization/blob/main/img/test_5.png "Тестирование")
