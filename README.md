# My AI Idea / Proiect

## Rezumat
Proiectul reprezinta un sistem de recomandare personalizat pentru filme si carti. Acesta analizeaza evaluarile si preferintele anterioare ale unui utilizator pentru a sugera continut nou pe care este foarte probabil sa il aprecieze, utilizand metrici de similitudine din invatarea automata.

## Context
Avand in vedere milioanele de carti si filme disponibile online, utilizatorii sufera de o supraincarcare de optiuni. Acest proiect rezolva problema prin filtrarea automata a continutului. Este important deoarece economiseste timp pentru utilizatori si creste implicarea pe platforma pentru furnizorii de continut.

## Date utilizate
Sistemul necesita doua tipuri de date: metadate despre continut (genuri, autori, regizori, ani de lansare) si date privind comportamentul utilizatorilor (evaluari de la 1 la 5, istoricul de vizionare sau lectura). Aceste date pot fi preluate din seturi de date deschise precum MovieLens sau prin API-ul Goodreads.

## Algoritm
Motorul principal foloseste algoritmul K-Nearest Neighbors (K-NN) bazat pe Filtrare Colaborativa. Acesta calculeaza distanta euclidiana sau similitudinea cosinus intre utilizatori. Daca Utilizatorul A si Utilizatorul B au o distanta foarte mica (similitudine mare) in evaluarile lor, sistemul recomanda filme care i-au placut Utilizatorului B, dar pe care Utilizatorul A nu le-a vazut inca.

## Impact estimat
Proiectul va oferi sugestii automate cu o precizie ridicata. Utilizatorii vor descoperi carti si filme de nisa pe care altfel nu le-ar fi gasit cu usurinta. Pentru companii, acest sistem poate creste direct rata de retentie a utilizatorilor si timpul petrecut zilnic pe aplicatie.

## Limitari
Principala limitare este problema Cold Start (Pornirea la rece): sistemul nu poate oferi recomandari bune utilizatorilor complet noi, care nu au evaluat inca niciun continut. In plus, poate crea o bula de filtrare, recomandand in mod repetat aceleasi genuri si blocand diversitatea continutului.
