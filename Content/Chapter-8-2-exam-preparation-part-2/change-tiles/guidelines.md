### Насоки и подсказки

Следващата задача изисква от нашата програма да приема повече входни данни и извърши по-голям брой изчисления, въпреки че решението е **идентично**. Приемането на данните от потребителя извършваме по добре **познатия ни начин**. Обърнете внимание, че в раздел **Вход** в условието е упоменато, че всички входни данни ще бъдат **реални числа** и поради тази причина бихме използвали тип **`decimal`**.

След като вече разполагаме с всичко необходимо, за да изпълним програмната логика, можем да пристъпим към следващата част. Как бихме могли да **изчислим** какъв е **необходимият** брой плочки, които ще бъдат достатъчни за покритието на целия под? Условието, че плочките имат **триъгълна** форма, би могло да доведе до объркване, но на практика задачата се свежда до съвсем **прости изчисления**. Бихме могли да пресметнем каква е **общата площ на пода** по формулата за намиране на площ на правоъгълник, както и каква е **площта на една плочка** по съответната формула за триъгълник.

За да пресметнем какъв **брой плочки** са необходими, **разделяме площта на пода на площта на една плочка** (като не забравяме да прибавим 5 допълнителни броя плочки, както е по условие).

<table>
<tr>
<td width="10%"><img src="/assets/alert-icon.png" style="max-width:50px" /></td>
<td>Обърнете внимание, че в условието е упоменато да закръглим броя на плочките, получен от делението, до по-високо цяло число, след което да прибавим 5. Потърсете повече информация за системната функционалност за това: <code><strong>Math.Ceiling(…)</strong></code>.
</td>
</tr>
</table>

До крайния резултат можем да стигнем, като **пресметнем общата сума**, която е необходима, за да бъде покрит целия под, като **съберем цената на плочките с цената за майстора**, която имаме от входните данни. Можем да се досетим, че **общият разход** за плочките можем да получим, като **умножим броя плочки по цената за плочка**. Дали сумата, с която разполагаме, ще бъде достатъчна, разбираме като сравним събраните до момента пари (от входните данни) и общите разходи.

### Тестване в Judge системата

Тествайте решението си тук: [https://judge.softuni.bg/Contests/Practice/Index/517#1](https://judge.softuni.bg/Contests/Practice/Index/517#1).