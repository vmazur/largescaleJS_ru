# Паттерны для масштабируемых JavaScript-приложений

Перевод на русский язык. Эдди Османи [в курсе][1].

## Участники

    project  : largescaleJS_ru
    repo age : 9 weeks
    active   : 51 days
    commits  : 373
    files    : 132
    authors  : 
        278  Shuvalov Anton          74.5%
        42  Vladimir Starkov        11.3%
        22  Rakhim Davletkaliyev    5.9%
        10  andreyr82               2.7%
         7  FMRobot                 1.9%
         2  theghostbel             0.5%
         2  Sergei Khaletskiy       0.5%
         2  Vlad Tsepelev           0.5%
         1  rakeev                  0.3%
         1  Andrew                  0.3%
         1  Artem Sapegin           0.3%
         1  Andrey Rachkov          0.3%
         1  croupier                0.3%
         1  finico                  0.3%
         1  Nikita Bayev            0.3%
         1  Mikhail Baranov         0.3%


## Разработчикам

Главы на английском языке и на русском лежат в директории *[./_includes/translation/][2]*

В оформлении markdown мы стараемся придерживаться [правил][3] от Frontender Magazine.

Локально сайт можно запустить примерно так:

    git clone https://github.com/shuvalov-anton/largescaleJS_ru.git largescalejs
    cd $_
    bundle install
    stylus -w -o assets/css/ ./_stylus/main.styl
    jekyll serve --watch

Версия для электронных книг, к сожалению, совершенно не зависит от других файлов.
Собирать новые книги так:

    cd ./epub
    pandoc epub.md -o largescale-js.epub --toc-depth=2 --epub-cover-image=cover.jpg --epub-chapter-level=2
    pandoc epub.md -o largescale-js.fb2 --toc-depth=2 --epub-cover-image=cover.jpg --epub-chapter-level=2
    kindleGen -c1 -locale ru  largescale-js.epub -o largescale-js.mobi

[1]: https://twitter.com/addyosmani/status/415195066895171584
[2]: https://github.com/shuvalov-anton/Patterns-For-Large-Scale-JavaScript-Application-Architecture/tree/gh-pages/_includes/translation
[3]: https://github.com/FMRobot/FM-guidelines
