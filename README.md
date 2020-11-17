
# Harjoitus 3 
 
Aloitaan tehtävän tekeminen tekemällä Githubiin uuden repon. Kloonataan uusi repo "git o$
Syötetään myös käyttäjätiedot, jotta systeemi toimisi oikein. Git config --global user.e$
git config --global user.name"
git config --global credential.helper "cache--timeout=3600"

 Tästä siirrytään repon kansioon ja luodaan sinne tiedoston "harjoitus3.md".
 Tallennan tämän tiedoston ja siirrän sen repoon komennolla "git add . && git commit; git pull && git push". Näin tiedostot siirtyvät tietokoneeltani suoraan GitHubiin

# B) 

Git log: Komento näyttää repoon tehdyt muutokset ja commitit. Näistä näkyy commit token, commitin aika, ajaja ja ajanankommentit.

commit 1db38bdf8b200d16a996814fc4fe8b511d602476 Author: Koisedi <bgg337@myy.haaga-helia.fi> Date:   Tue Nov 17 10:58:00 2020 +0200 

Git Diff: Komento kertoo mitä muutoksia on tehty, mikä on paikallisen hakemiston ja reposition ero. Kyseisessä tapauksessa loin muutoksen Readme tiedostoon. 

edi@edi-VirtualBox:~/LinuxBox$ git diff diff --git a/README.md b/README.md index 4b598dd..467132e 100644 --- a/README.md +++ b/README.md @@ -13,6 +13,8 @@ git config --global credential.helper "cache--timeout=3600"

Git Blame: Komento kertoo kuka on tehnyt muutokset mihinkin tiedostoon ja kellonajan. 

64a58b62 (Koisedi           2020-11-17 11:25:14 +0200 20) Git Blame: Komento kertoo kuka on tehnyt muutokset mihinkin tiedostoon ja kellonajan. 10baefe7 (Koisedi           2020-11-17 10:27:06 +0200 21)

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
