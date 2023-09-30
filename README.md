# Hesla

Generujte bezpečná i nebezpečná hesla.
Vytvořte si repozitář ze šablony cviceni-hesla se stránkou, která obsahuje tři různé funkce na generování hesel. Každá funkce vygeneruje heslo zadané délky s určitou bezpečnostní silou. Kód funkcí zkoumat nemusíte, obsahuje věci, které jsme zatím neprobírali.

Příklad samostatného použití jednotlivých funkcí:

weakPassword(5); // → '01234'
mediumPassword(8); // → '48140525'
strongPassword(6); // → 'azc7mw'
Napište funkci createAccount, která se bude tvářit, že zakládá nový uživatelský účet. Funkce bude mít dva parametry user a generatePassword. První bude uživatelské jméno a druhý bude funkce, pomocí které se má vygenerovat heslo pro tento účet. Funkce createAccount vrátí řetězec, který bude obsahovat jméno uživatele a heslo vygenerované voláním funkce generatePassword. Funkci generatePassword při volání předejte číslo 9 jako délku hesla.

Na konci javascriptového kódu vyzkoušejte založit více různých účtů s různými typy hesel. Například:

document.body.innerHTML += `	<p>${createAccount('Míša', weakPassword)}</p>
	<p>${createAccount('Řízek', mediumPassword)}</p>
	<p>${createAccount('Mápodčepicí', strongPassword)}</p>`;
by mělo vepsat do stránky něco jako:

Uživatel Míša s heslem 012345678
Uživatel Řízek s heslem 074031827
Uživatel Mápodčepicí s heslem mwwf9epts
