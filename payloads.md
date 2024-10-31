## Payload 1

При переходе по ссылке `https://google-gruyere.appspot.com/351320745252871235370896829056166734910/`. Можно добавить в конце url пейлоад `<script>alert('XSS')</script>` для выполнения Reflected XSS инъекции. Этот payload внедряется в параметр URL и вызывает выполнение JavaScript кода на странице.

## Payload 2

При создании нового снипета на странице `https://googlegruyere.appspot.com/351320745252871235370896829056166734910/newsnippet.gtl`, можно использовать пейлоад <img src=x onerror=alert('XSS')>  для выполнения инъекции в теге <img>, что приведет к выполнению alert-скрипта при ошибке загрузки изображения.

## Payload 3

При обновления иконки профиля на странице `https://googlegruyere.appspot.com/351320745252871235370896829056166734910/editprofile.gtl`, можно использовать пейлоад <img src=x onerror=alert('XSS')>  для выполнения инъекции в теге <img>, что приведет к выполнению alert-скрипта при ошибке загрузки изображения.

## Payload 4

При обновления иконки профиля на странице `https://googlegruyere.appspot.com/351320745252871235370896829056166734910/editprofile.gtl`, можно использовать пейлоад <iframe%20src="javascript:alert(document.cookie);"></iframe>  для выполнения инъекции в теге <img>, что приведет к выполнению alert-скрипта, которые выведит куки.

## Payload 5

Можно вывзвать payload через вставку js кода в url по примеру: `https://google-gruyere.appspot.com/409795454757263309323652174942897092634/<img src=x onerror=alert('XSS')>`, что вызовет переход на несуществующую страницу и вызов alert с сообщением.
