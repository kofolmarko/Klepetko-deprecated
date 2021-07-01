Igra Klepetko se izvaja v HTML5 Canvas elementu ter je zgrajena s pomočjo programskega ogrodja Phaser. Element Canvas je namenjen dinamičnemu prikazovanju programabilnih oblik, teksta, slik in podobnega. Ogrodje Phaser nam delo olajša, saj prinaša bogato knjižnico z že vnaprej pripravljenimi funkcijami, ki so na primer uporabljene pri premikanju karakterja.

Ker je igra večigralska, potebuje tudi strežnik, ki deluje v okolju Node.js. Iz strani uporabnika se ob vsaki spremembi pošiljajo podatki na strežnik, ki jih obdela, obdrži uporabne ter razdeli med ostale igralce tiste, ki so jim namenjeni. Za povezavo na strežnik, pošiljanje in prejemanje podatkov v realnem času skrbi modul Socket.IO.

Primer delovanja klient-strežnik: eden izmed igralcev na strežnik pošlje koordinate svojega karakterja, strežnik nato prejete koordinate pošlje ostalim igralcem, ki so v isti sobi. Vsak izmed igralcev sprejme podatke in ustrezno posodobi izris ostalih igralcev v svojem Canvas elementu.
