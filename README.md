# Opis projekta
Template projekta je preuzet sa sajta [https://www.free-css.com/free-css-templates](https://www.free-css.com/free-css-templates)

Template služi za obnavljanje HTMLL i CSS tehnologija i prikaz dobrih praksi dizajna i stilizovanja veb sajtova
# Koraci za preuzimanje
1. Potrebno je kreirati folder na lokalnom računaru u kojem će projekat biti sačuvan
2. Otvoriti Git Bash terminal u okviru kreiranog foldera
3. Komandom `git clone` potrebno je klonirati ovaj repozitorijum\
   `git clone git@github.com:elab-development/kteh-tamara.git`

4. Kako ovaj repozitorijum već poseduje svog autora i remote lokaciju, potrebno je da podesite nove (svoje) parametre. 
Komandom `git config --local user.name [ime]` postavljate vaše ime, na primer `git config --local user.name "Petar Petrovic"`\
Komandom `git config --local user.email [email]` postavljate vaš email, na primer `git config --local user.email petar.petrovic@gmail.com`\
Primetite da se za ime koriste navodnici `" "`, dok za email to nije potrebno.\
Komandom `git remote -v` možemo proveriti trenutnu remote lokacije repozitorijuma, dok komandom `git remote remove [lokacija]` brišemo konkretnu lokaciju, na primer `git remote remove origin`
5. Nakon postavljanja lokalne konfiguracije i brisanja remote lokacije, potrebno je kreirati novi repozitorijum na GitHub nalogu koji će biti nova remote lokacija za ovaj projekat
6. Komandom `git remote add [ime_lokacije] [adresa_lokacije]` dodajemo novu remote lokaciju.\
   Na primer `git remote add origin git@github.com:tamara-naumovic/test.git` \
   Vodimo računa do koristimo **SSH** povezivanje a ne ~~HTTPS~~
7. Da bi ovaj remote repozitorijum povezali sa lokalnim potrebno je dodati SSH ključ u okviru lokalnog repozitorijuma na računaru, pod uslovom da je SSH ključ generisan, ako nije potrebno je generisati nove ključeve i povezati sa GitHub nalogom.\
   Ključ se povezuje sledećim komandama \
   `eval ssh-agent -s` \
   `ssh-add [adresa_kljuca]` na primer `ssh-add c:/users/student/.ssh/id_rsa` - nakon čega je potrebno uneti šifru ključa
8. Kada je ključ uspešno dodat moguće je uraditi push-ovanje promena na remote repozitorijum komandom `git push origin master`
   

