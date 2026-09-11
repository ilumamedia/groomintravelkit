# Grooming Concept — Travel Kit landing

Statičan sajt, četiri samostalna HTML fajla. Nema build koraka — prebaciti ceo folder u
repozitorijum i uključiti GitHub Pages.

## Fajlovi

| Fajl | Šta je |
|---|---|
| `index.html` | Landing, desktop prikaz |
| `checkout.html` | Strana za plaćanje, desktop prikaz |
| `mobil.html` | Landing, mobilni prikaz |
| `checkout-mobil.html` | Strana za plaćanje, mobilni prikaz |

## Kako se bira prikaz

Svaka stranica na učitavanju meri širinu prozora i, ako treba, prebacuje na svoj par:

- uže od 768px → mobilni prikaz
- 768px i šire → desktop prikaz

Posetilac uvek otvara `index.html`; ostalo ide samo. Za testiranje jednog prikaza bez
prebacivanja, dodati `?nored` na kraj adrese (npr. `mobil.html?nored`).

Izbor linije i boje nesesera prenose se na checkout kroz adresu:
`checkout.html?kit=Pupper&boja=Roze`.

## Slike

Slike su privremene i ugrađene u same HTML fajlove (zato je `mobil.html` velik).
Kad stignu prave fotografije, zameniti ih i izvesti ponovo, po mogućstvu kao WebP
oko 1600px širine i kao odvojene fajlove umesto ugrađenih.

## Napomena o plaćanju

Ovo je dizajn, ne radna prodavnica. Dugme „Poruči" ne šalje porudžbinu. Strane za plaćanje
se ugrađuju u WordPress kao WooCommerce checkout template; naplatu i dalje obrađuje
Raiffeisen banka preko postojećeg podešavanja.

## Boje i fontovi

- Naslovi i dugmad: Manrope (800 za naslove, 700 za dugmad)
- Telo teksta: Karla 18px, `#6E5040`
- Zelena: `#748629`, sastojci `#4D571D`
- Terakota: `#9E5730`, `#944D27`, okvir `#DCBFA4`
- Podloge: `#FBF3EA`, kartice `#FFFDF9`, finalna CTA sekcija `#F7E9DA`
