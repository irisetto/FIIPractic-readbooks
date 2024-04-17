Proiect FIIPractic CloudLab - Cohman Teodora Cristina

Am ales sa fac o aplicatie de tipul librarie online, deoarece este ceva ce imi doresc de mult timp pentru mine si vreau sa o continui ca sa o aduc in forma la care ma gandesc.
Cartile sunt preluate din API-ul Google Books si utilizate cu ajutorul librariei Scriptotek.
Am folosit tailwind si vite pentru stilizare.
# Functionalitati
In timpul pe care l-am avut am reusit sa fac:
1. cand userul nu este logat
   - meniul home care pe viitor va avea mai multa substanta
   - meniul books, initial are niste carti deja preluate dupa un query din api care sunt afisate alaturi de butonul de search la intrarea in pagina; putem cauta carti dupa un query personalizat si vor fi afisate in locul celor existente
   - la apasarea pe coperta unei carti va deschide pagina cartii unde exista mai multe informatii despre carte
   - butoanele de login si register

2. cand userul este logat
   - meniul home care e acelasi
   - meniul books unde de data asta fiecare carte ofera posibilitatea de a fi adaugata intr o anumita lista
   - meniul my books, unde avem listele userului in stanga. cand deschide pagina initial apar toate cartile userului, iar cand se apasa pe o lista anume, sunt afisate cartile doar din acea lista
   - fiecare carte din librarie are buton de delete in caz de vrem sa stergem cartea din my books

In momentul inregistrarii userului sunt create 2 liste default ("to read","finished") pentru acesta. pe viitor voi face ca userul sa poata sa isi creeze si liste personalizate
Daca cartea exista deja intr o lista, nu mai poate fi adaugata in alta (pe viitor cand vor exista mai multe liste voi modifica acest comportament)

Pentru rulare am folosit php artisan serve si npm run dev.
Cheia pentru google api se afla in env.example

# Testare

Nu am mai creat seedere, deoarece cartile exista deja in api.
- Cand nu esti logat meniul de my books si adaugarea in liste nu exista.
- Inregistrati-va ca user nou
- Logati-va
- Accesati books si adaugati in liste mai multe carti
- Dati search la niste carti
- Apasati pe o carte (pe coperta) pentru a vizualiza mai multe informatii si o adauga in lista
- Navigati la my books si vizualitati cartile in functie de lista
- Stergeti ce carte nu v-o doriti in librarie

  
- Delogati-va
