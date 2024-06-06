# Interactive system for generating chords
Acest sistem de tip MIDI Effect este realizat din doua efecte MIDI: un device ce converteste miscarile realizate la camera web in note, respectiv un device de generare de acorduri ce converteste notele muzicale individuale generate prin camera video in acordurile corespunzatoare intr-o scala selectata. Notele acordului pot fi, de asemenea, “ciupite” ca la o chitară, în loc să fie cântate toate simultan. Generatorul de acorduri include 7 moduri, multe tipuri de acorduri suplimentare, opțiuni de inversiune și de articulare a acordurilor, precum și o randomizare îmbunătățită a notelor “ciupite”. Ambele dispositive sunt realizate in MaxforLive din Ableton 12.

#### **Mențiune**

Deoarece nu pot incarca direct prin GitHub foldere cu mai mult de 100Mb, am lasat mai jos un link ce contine un proiect demo realizat cu sistemul in Ableton Live 12:

- [Demo](https://we.tl/t-rtwEWWMdZH);

## (Instalare)
Cele doua dispozitive pot fi descarcate din acest repo. Pentru a putea fi utilizate in Ableton Live 12, cele doua dispozitive trebuie incluse in folderul director: 

- pentru Windows: \Users\[username]\Documents\Ableton\User Library

- pentru MacOS: Macintosh HD/Users/[username]/Music/Ableton/User Library.


## (Utilizare)
Sistemul poate fi folosit in doua moduri: fie prin separarea fiecarui dispozitiv, fie prin folosirea lor impreuna. Prin folosirea celor doua dispozitive impreuna, trebuie sa se respecte o anumita ordine astfel: prima oara se deschide Video Motion Sounds by Hiei and V-217, iar apoi V-217 Chord Generator, dupa care se poate deschide orice instrument doreste utilizatorul pentru a putea crea o progresie de acorduri pentru cantecul pe care il compune intr-un mod interactiv.

![Untitled.png](https://github.com/VictorDucuGhioca/PCON-proiect-final/blob/main/assets/Untitled.png)

Pentru generarea de acorduri, se va deschide V-217 Chord Generator intr-un track nou MIDI in Ableton, se va alege gama pe care vrem sa o folosim (de la C la B), tipul acordului (major, minor, dorian, etc.), precum si felul lui (triad, shell, 11th, sus2, etc.). Notele colorate in verde ce se pot observa in kslider indica notele gamei pe care utilizatorul doreste sa o utilizeze.

![V-217 Chord Generator Interface.png](https://github.com/VictorDucuGhioca/PCON-proiect-final/blob/main/assets/V-217%20Chord%20Generator%20Interface.png)

Utilizatorul va crea o linie de bass in acel track MIDI (fie inregistrand notele de bass, fie introducand un fisier MIDI in track-ul respectiv), dupa care se va crea un nou track MIDI, se va face send din al doilea track la primul ce contine generatorul si astfel in cel de-al doilea track va apararea un fisier MIDI ce contine progresia de acorduri creata de utilizator. 

![testare generator.png](https://github.com/VictorDucuGhioca/PCON-proiect-final/blob/main/assets/testare%20generator.png)


Dispozitivul care utilizeaza camera video are reprezentate in partea de sus a camerei video 12 linii reprezentand cele 12 note muzicale. Atunci cand utilizatorul se misca in dreptul lor, acestea transmit informatia MIDI catre sintetizator, care genereaza notele muzicale. De asemenea, camera poate fi pornita sau oprita la alegerea utilizatorului prin apasarea butoanelor close si open. In plus, daca utilizatorul are mai multe camere web atasata calculatorului, atunci el poate alege ce camera sa foloseasca din prima lista afisata in interfata dispozitivului Max.

![Video Motion Sounds by Hiei and V-217.png](https://github.com/VictorDucuGhioca/PCON-proiect-final/blob/main/assets/Video%20Motion%20Sounds%20by%20Hiei%20and%20V-217.png)

## (Istoric)

(13.05) ...

(3.06) ...

(X.06) ...

## (Link-uri)
Pentru realizarea sistemului, m-am inspirat dupa urmatoarele link-uri:

- https://maxforlive.com/library/device/9921/181-motion-harp;

- https://maxforlive.com/;

- https://maxforlive.com/library/device/6333/chorb;

- https://maxforlive.com/library/device/3920/nylon-chord-generator;

- https://maxforlive.com/library/device/917/chord-generator;

- https://maxforlive.com/library/device/2189/xeno-chord-explorer.

# Dezvoltarea proiectului

Pentru început:

1. Creează-ți cont pe Github
2. Download și install [Github Desktop](https://desktop.github.com/)
3. Citește [acest ghid](https://charlesmartin.com.au/blog/2020/08/09/student-project-repository) și ține la îndemână [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet).

Apoi, procesul este următorul (inspirat de [aici](https://cs.anu.edu.au/courses/comp1720/deliverables/05-major-project/#submission-process)):

1. *fork* al acestui template către propriul tău cont de Github

![](assets/fork.gif)

_(dacă preferi cumva ca repo-ul să nu fie vizibil de către public, îl poți seta ca Private din Settings - "Change visibility". Atunci trebuie să mă adaugi drept colaborator, ca eu să am acces.)_

2. *clone* al repo-ului din Github Desktop pentru a-l downloada local

![](assets/clone.gif)

3. *commit* și *push* pe măsură ce lucrezi la proiect. Ultima versiune push-ată pe server înainte de deadline va conta pentru evaluare.

![](assets/commit.gif)

## Elemente obligatorii

1. Acest readme completat. Titlu, descriere, mod de utilizare, istoric, link-uri utile.

   Poți include și imagini și chiar [gif-uri animate](https://www.screentogif.com/), sau link-uri către materiale audio/video.
   
   Vezi [aici](https://charlesmartin.com.au/blog/2020/08/09/student-project-repository) mai multe sugestii.

2. [Declarația de originalitate](statement-of-originality.yml) completată. Tot ce nu este inclus acolo va fi considerat 100% contribuție proprie.

    *(formatul este adaptat de [aici](https://gitlab.cecs.anu.edu.au/comp1720/2018/comp1720-2018-major-project/-/blob/master/statement-of-originality.yml). Da, este un pic ironic să refolosim un doc [de altundeva](https://cs.anu.edu.au/courses/comp1720/resources/faq/#how-do-i-fill-out-my-statement-of-originality), dar menționăm sursa deci nu este plagiat!)*

3. Proiectul în sine. Tot codul trebuie să fie prezent, proiectul trebuie să poată rula conform instrucțiunilor din readme. Dacă e nevoie de asset-uri mari (sunete, video etc), [folosește Git LFS](https://git-lfs.github.com/) sau include link de download în instrucțiunile de instalare.

