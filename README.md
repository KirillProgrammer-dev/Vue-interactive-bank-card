# Vue-interactive-bank-card
<h1>Проверка банковской карты на Vue.js 3</h1>
<p>
    Этот валидатор может определять 5 видов платежных систем 
    <ul>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Visa <img width="5%" src="img/systems/visa.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Mir <img width="5%" src="img/systems/mir.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Mastercard <img width="5%" src="img/systems/mastercard.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Maestro <img width="5%" src="img/systems/maestro.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >American-express <img width="5%" src="img/systems/american-exp.png"> </li>
    </ul>
    И 10 банков
    <ul>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Альфа банк <img width="5%" src="img/banks/alpha.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Газпром банк <img width="5%" src="img/banks/gazprombank.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Мтс банк <img width="5%" src="img/banks/mts-bank.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Банк Открытие <img width="5%" src="img/banks/otkrytie.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Райфайзен банк <img width="5%" src="img/banks/raiffaizen.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Росбанк банк <img width="5%" src="img/banks/rosbank.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Банк Русский стандарт<img width="5%" src="img/banks/russian_standart.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Сбербанк<img width="5%" src="img/banks/sberbank.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Втб банк <img width="5%" src="img/banks/vtb.png"> </li>
        <li style=" display: flex;align-items: center;flex-direction: row;" >Тинькофф банк <img width="5%" src="img/banks/tinkoff.png"> </li>
    </ul>
    <h2>Алгоритм Луна</h2>
    <p>
        Алгоритм позволяет добится максимальной валидации карты.
    </p>
    <ul>
        <li>Цифры проверяемой последовательности нумеруются справа налево.</li>
        <li>Цифры, оказавшиеся на нечётных местах, остаются без изменений.</li>
        <li>Цифры, стоящие на чётных местах, умножаются на 2.</li>
        <li>Если в результате такого умножения возникает число больше 9, оно заменяется суммой цифр получившегося произведения — однозначным числом, то есть цифрой.</li>
        <li>Все полученные в результате преобразования цифры складываются. Если сумма кратна 10, то исходные данные верны.</li>
    </ul>
    <img src="img/git/screen1.png">
</p>