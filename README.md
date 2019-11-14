# QuizBash program


Ezen programom alkalmas diákok vizsgáztatására, amennyiben nem adunk nekik read jogosultságot a prop mappára, hogy ne tudják látni a kérdéseket és az azokhoz tartozó helyes válaszokat.

# Konfiguráció
A prop/config fájlban be lehet állítani, hogy az egyes érdemjegyekhez minimum hány százalékot kell elérni, valamint be lehet állítani, hogy az egyes kérdés típusokból hányra kelljen válaszolniuk a diákoknak. 
# *VIGYÁZAT!!!*
A konfigurációs fájlban ne adjon meg nagyobb értéket az egyes kérdések beállításánál, mint ahány kérdés az adott típusból rendelkezésre áll a database.txt fájlban! Ellenőrizheti, hogy az egyes fajta kérdésekből hány darab áll rendelkezésre, ha elindítja a programot és a "0"-ás számú opciót választja.
# Kérdés hozzáadás
A kérdés hozzáadásához a prop/database.txt fájlt kell megnyitni.

`KERD_KOZEPES2Hany ujja van az embernek?%K_V`
`-5`
`-4`
`-8`
`-9`
`+10%`

Felépítése egy kérdésnek és a hozzá adott válaszoknak:
KERD_KONNY (KOZEPES, NEHEZ vegződések egyéb esetben) - a kérdés nehézségi besorolása
1, 2 - Egyes azon kérdés, amire szöveges választ várunk, begépelve, 2 pedig a feleletválasztós kérdéseket jelöli
[ kérdés szövege ]%K_V - A kérdés szövege után meg kell adni egy százalékjelet és a K_V megjelolést.
-- Jelekkel jeloljuk a hibás kérdéseket (csakis 2-es típusú kérdés esetén)
++ Jelekkel jeloljuk a helyes választ, csak egy helyes válasz lehet!
A válaszok megadása után szintén kötelező egy *százalékjelet* kiírni!
