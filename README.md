# Forked from MarhyCZ/picons
## CZ - Marhyho Picony & Ikony

## Ikony
Nějakou chvíli jsem si dělal svůj vlastní balíček TV ikon jak do Kodi, tak Tvheadend klientů. Protože polovina klasických ikon není vidět na tmavém skinu a polovina není vidět na světlém skinu. Udělal jsem tedy old school čtvercová loga, jejichž pozadí je dominantní barva loga té televizní stanice a to logo samotné je světlé.
Pro mě to vypadá hezky jak na výchozím novém Kodi skinu, tak třeba i v TvhClientu na iOS.

Stáhnout si můžete jak soubor .ai, kde jsou téměř veškerá loga vektorová, můžete si je upravit dle své libosti a vyexportovat do jakéhokoliv rozlišení chcete. 
Anebo tu mám už hotový balíček s rozlišením 640px, což se mi ukázalo jako ideál pro Kodi do většiny skinů

Pro 4K panely mám vyexportovaný balíček v 1024px. Pro uživatele 4K televizoru s 1080p vstupem (např. malinou) je toto zbytečné.

Balíček si můžete stáhnout v příloze do vašeho vlastního serveru, případně hostuji zde na GitHubu identickou kopii.


### Použití v Tvheadend

Balíček ikon je je připravený pro použití v Tvheadendu a ikony jsou pojmenované podle schéma satelitních kanálů.

- Stačí jít do záložky Configuration -> General -> Base -> Picon

- Channel icon path udává cestu ke složce, ve které se nachází ikony. Pokud se nachází ikony na lokálním disku, je cesta v následujícím formátu: file:// + cesta ke složce /%C.png (za %C se dosadí vygenerovaný název)
  - např. file:///home/user/icons/%C.png (3 lomítka na začátku, protože třetí je root / )

- Channel icon scheme nastavit na Service name picons a uložte změny

- Jděte do Configuration -> Channel/EPG. Zde si zobrazte všechny kanály (vpravo dole Show All)
- Stiskem CTRL+A všechny kanály označte a stiskněte Reset icon.
- Změny uložte a tím se pro každý kanál nově vygeneruje cesta k piconám podle nového nastavení.
- Hotovo.

<img src="http://marhycz.github.io/picons/docs/images/tvheadendconf.png" width="384"><img src="http://marhycz.github.io/picons/docs/images/tvheadendconf2.png" height="378">
