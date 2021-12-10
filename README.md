# vaja4_interupt_tipka_LED

V Pinout % Configuraton pogledu glede na vašo razvojno ploščico ugotovite, ali lahko uporabite modro tipko za digitalni vhod kot interrupt (GPIO_EXT…). Če da, kateri pin je to? PA0

Zapišite naslov izhodnih pinov za zeleno in modro LED:
PC9 (LD3 - Green Led)  PC8 (LD4 - Blue Led)

Znotraj te funkcije zapišite ukaz za vklop/izklop zelene LED:
HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_9);

Koliko znaša (v mili sekundah) zapisana zakasnitev, ki jo proizvede zanka for?
10000

V user code begin 3 - zanka while(1) - zapišite ukaz za utripanje modre LED:
HAL_GPIO_TogglePin(GPIOC, GPIO_PIN_8);

V to zanko dodajte ukaz za zakasnitev z funkcijo Delay iz knjižnice HAL, in sicer pol sekunde:
HAL_Delay(500);

Opazujte delovanje (utripanje modre LED). Kaj se zgodi, ko pritisnemo na modro tipko na STM32L1? Zelena LED se prižge

Ali pritisk na modro tipko vpliva na utripanje modre LED in zakaj? Ne upliva, ker je modra LED nastavljena tako, da vedno utripa

Komentar:
