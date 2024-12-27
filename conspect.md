### устоновка

что бы устоновить parcel глобально надо иметь node js и написать команду
- bun install -g parcel
- npm install --save-dev parcel

### Работа

перед изпользованием parcel надо сделать bun init -y говорите вы? НЕТ! package.json не нужен!!!

пишем: parcel -D build src/index.html
но можно сделать в scripts(в package.json)
- "dev": "parcel src/index.html"
- "build": "parcel build src/index.html"

### КРУТО!!

bun run build
теперь мы можем делать Супер Сборку - у нас появится dist, package.json и поставятся библиотеки: есле у нас в src pug, ts, scss то тогда поставятся нужние библиотеки для pug,ts,scsss
и не забываем про bun run dev - он сделает нам localhost вместо go live и запуска файла отдельно
