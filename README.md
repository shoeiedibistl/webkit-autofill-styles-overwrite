# input-autofill-overwrite-browser-styles

<b>особенности работы:</b><br>
    -   <b>Решено</b> <s>заливка инпута после автозаполнения применяется не стандартная, а остается из состояния "focus" (возможно, и что-то еще кроме заливки). но ее можно назначить отдельно </s><br>
    -   <b>Больше не требуется</b> <s>можно устанавливать свою заливку для инпута при автозаполнении (свойство box-shadow inset)</s>  <br>
    -   <b>Решено</b> <s>не работает transition для box-shadow после автозаполнения, в т.ч. и для заливки фона (резкое появление) </s><br>
    -   <b>Решено</b> <s>не накладывается заливка фона при :hover, даже через js </s><br>
    -   <b>Проверить</b> автоматически может не сбрасываться состояние focus при очистке input.value скриптом, только после ручного прокликивания. теоретически может помочь дополнительная установка и снятие фокуса скриптом после такой очистки (проверить). По идее, сейчас должно сбрасываться как надо <br>
    -   хром вроде как блокирует автозаполнения пароля. в фф не работает на инпутах tel, password, возможно, каких-то еще <br>
    -   Пока неясно, как работает в совокупности с parsley или другими валидаторами, особенно с масками телефона. По идее, проблем быть не должно <br>
    -   <b>!!! протестировано в хроме и фф !!!</b> 
возможно, для других браузеров потребуется дописать скрипт и стили для фокуса, ховера, селекта и тд по аналогии с input:-webkit-autofill
