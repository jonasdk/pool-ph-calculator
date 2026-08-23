# Pool pH

Version 1.1

Læg alle filer i samme mappe på en webserver med HTTPS (fx GitHub Pages).
Åbn siden i Safari på iPhone → Del → "Føj til hjemmeskærm". Herefter virker appen offline.

Filer: index.html, manifest.webmanifest, sw.js, icon-180.png, icon-192.png, icon-512.png

Beregning: karbonat-buffer (K1 = 10^-6,35, K2 = 10^-10,33) ud fra alkalinitet og aktuel pH.
Produktkoncentration kan ændres i appen og huskes.

## Version

Versionsnummeret staar oeverst i appen og skal matche CACHE-navnet i sw.js.
Ved hver aendring: ret baade `<span class="ver">` i index.html og `const CACHE` i sw.js.
Ellers henter en installeret app ikke den nye version.
