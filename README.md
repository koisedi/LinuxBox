
# Harjoitus 3 
 
Aloitaan tehtävän tekeminen tekemällä Githubiin uuden repon. Kloonataan uusi repo "git o$
Syötetään myös käyttäjätiedot, jotta systeemi toimisi oikein. Git config --global user.e$
git config --global user.name"
git config --global credential.helper "cache--timeout=3600"

 Tästä siirrytään repon kansioon ja luodaan sinne tiedoston "harjoitus3.md" joka on kyseinen tiedosto jota kirjoitan.
 Tallennan tämän tiedoston ja siirrän sen repoon komennolla "git add . && git commit; git pull && git push". Näin tiedostot siirtyvät tietokoneeltani suoraan GitHubiin

# B) 

Git log: Komento näyttää repoon tehdyt muutokset ja commitit. Näistä näkyy commit token, commitin aika, ajaja ja ajanankommentit.

Git Diff: Komento kertoo mitä muutoksia on tehty, mikä on paikallisen hakemiston ja reposition ero. Kyseisessä tapauksessa loin muutoksen Readme tiedostoon. 

Git Blame: Komento kertoo kuka on tehnyt muutokset mihinkin tiedostoon ja kellonajan. 

# C) Tyhmä muutos

Muokkasin harjoitus3.md tiedostoa ja lisäsin siihen muutoksen. Tämän jälkeen se tallenttaan 
ja löydään git reset --hard komento, joka palauttaa muutokset viimeisimpään kohtaan.

# D) Tee uusi Salt-moduuli

Tehdään uusi moduuli. Aion tällä kertaa asentaa Gimp-kuvankäsittelyohjelman. 
Siirrytään Cd /srv/salt/ kansioon ja luodaan Mkdir gimp-kansio. Kyseisen kansion sisään laitetaan init.sls tiedosto johon laitetaan tarvittavat ohjeistukset saltille. Sitten helloworld pohja txt. 
Gimp:
  pkg.installed
Ajetaan komento läpi sudo salt '*' state.apply gimp. Toiminto onnistui. Ajetaan komento
vielä uudestaan. Toimii. 
