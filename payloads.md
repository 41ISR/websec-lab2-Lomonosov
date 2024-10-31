## Payload 1

При переходе по ссылке `https://google-gruyere.appspot.com/351320745252871235370896829056166734910/`. Можно добавить в конце url пейлоад `<script>alert('XSS')</script>` для выполнения Reflected XSS инъекции. Этот payload внедряется в параметр URL и вызывает выполнение JavaScript кода на странице.

## Payload 2

При создании нового снипета на странице `https://googlegruyere.appspot.com/351320745252871235370896829056166734910/newsnippet.gtl`, можно использовать пейлоад <img src=x onerror=alert('XSS')>  для выполнения инъекции в теге <img>, что приведет к выполнению alert-скрипта при ошибке загрузки изображения.

## Payload 3

При обновления иконки профиля на странице `https://googlegruyere.appspot.com/351320745252871235370896829056166734910/editprofile.gtl`, можно использовать пейлоад <img src=x onerror=alert('XSS')>  для выполнения инъекции в теге <img>, что приведет к выполнению alert-скрипта при ошибке загрузки изображения.

## Payload 4

Можно вывзвать payload через вставку img c onerror=alert('xss') на странице профиля в при создании private snipet: `https://google-gruyere.appspot.com/547594091525851475734108652343278146611/editprofile.gtl`, что вызовет ошибку и вывод сообщение alert.

