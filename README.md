# ertekeloRendszer

A DB-t leképezendő létre kell hozni a modeleket a következő paranccsal (VS -> tools -> Nuget Package Menager -> Package Menager Console-ból adjuk ki):
Scaffold-DbContext "server=localhost;database=ertekelo-rendszer;user=root;password=;ssl mode=none;" mysql.entityframeworkcore -outputdir Models -f
Figyeljünk a helyes DB-hozzáférés beállításaira valamint <b>production-ben</b> hozzunk létre SZIGORÚAN olyan usert, akinek kellő hozzáférése van,
ugyanakkor figyeljünk oda, hogy drop table / drop database hozzáférése ne legyen!
