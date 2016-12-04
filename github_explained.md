# LICENSE

LICENSE е името на един специялен файл, който всяко хранилище в Github трябва да има, това както може би се досещата е лиценза под, който вие публикувате вашия код. Този лиценз оказва какво е легалното ползване на вашият сорс код (софтуер)

# .gitignore

Tова отново е име на специялен файл, който оказва, кои файлове не искате да се следят, тоест да са под version control. Това най-често са файлове съдържащи така наречената sensitive data, тоест неща, които са необходими на вашият проект, но не бива да са публични или най-чесо вие искате да игнорирате всички файлове, които не предствалват source code. За C++ това са обектни файлове, изходни файлове, изпълними файлове като например .exe или .out динамични библиотеки, компилирани файлове или прекомпилирани header файлове.

Пример за C++ (template-а на Github)

```
# Compiled Object files
*.slo
*.lo
*.o
*.obj

# Precompiled Headers
*.gch
*.pch

# Compiled Dynamic libraries
*.so
*.dylib
*.dll

# Fortran module files
*.mod
*.smod

# Compiled Static libraries
*.lai
*.la
*.a
*.lib

# Executables
*.exe
*.out
*.app
```

Пример за sensitive дата са например файлове съдржащи token-и за api-та, които вашият прокет използва.

# README файл

Това е файл с име README, и задължително трябва да си има extention, които най-често е или .txt за текстови файл или .md за MarkDown файл (този файл е писан на MarkDown).

# Issue

Issue или на български проблем. Терминът за създаване на ново на английски език е open, а на български отваряне на нов проблем. Issue-та най-често се използват за докладване на проблем (bug reporting) или за искане на добавяне на нова функционалност (future request) и по-рядко за въпроси. Използват се за комуникация, за това какво трябва да се направи.

# Pull request

Pull request на български няма точен превод, но най-близкия превод можеби е "заявка за синхронизация" изхождайки от git командата `git pull`. Това реялно представляват заявки за промяна на кода на хранилището. Използват се за заявки, с които се оказва, че се оправя даден проблем (bug fixing) или за заявка за добавяне на код, които имплементира нова функионалност. Добра практика е да се отвори ново issue, в което да се опише по-детайлно какво не е на ред или какво смятате да добавите и след това да напривте нов Pull request, в който да кажете, че той оправя този и този проблем (на анг. Fixing Issue или Closing Issue).

Спецялно Github се използва единна идентификационна система на Issue-та и Pull request-ите, за всяко хранилище по-отделно един и същ номер се инкрементира последователно при отваряне на issue и при правене на pull request, с цел одобство при рефериране (линкване, цитиране). Това става чрез #\<номер на issue или pull request\>.

Пример:

След създаване на едно хранилище някой отваря ново issue, то ще има номер #1 и към него отново може да се реферира с #1. След, което някой прави pull request за да затвори това issue този pull request ще има номер #2 и към него отнво може да се рефирира с #2. И човека направил този pull request може да каже следното:
> Fixing #1

или

> Closing #1