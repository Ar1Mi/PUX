# Laboratorium 4 – UX Writing: komunikaty i mikrocopy

📄 Raport: [PDF](PUX_lab04_raport.pdf) · [DOCX](PUX_lab04_raport.docx)
📁 Makiety: [`makiety/makiety.html`](makiety/makiety.html) (przed / po) · [`makiety/zakreslacz.html`](makiety/zakreslacz.html) (test zakreślacza)

Projekt: **„Seans na dziś”**, aplikacja mobilna do szybkiego wyboru filmu na wieczór (kontynuacja lab1).
Audyt objął **27 komunikatów** w 5 grupach: CTA, błędy i toasty, formularze, puste stany i onboarding, dialogi. Przypadki A–D i scenariusze 1–3 z materiałów przeniesiono do kontekstu aplikacji.

---

## 1. Audyt – co było nie tak w wersji v0

| Problem | Przykłady |
|---|---|
| Żargon i kody błędów | `auth_fail_0x892`, `ERR_NO_PROVIDERS`, „Błąd 503” |
| Anglicyzmy z API | Dashboard, Mood, Providers, Watchlist, Network error |
| Ogólne przyciski | Dalej, OK, Przejdź, Wyślij formularz |
| Brak kroku zaradczego | „Nie znaleziono wyników dla podanych kryteriów.” |
| Lęk / obwinianie | „błąd krytyczny”, „nieprawidłowy”, „musisz” |
| Dark patterns | confirmshaming przy anulowaniu Premium i usuwaniu konta |

## 2. Voice & Tone

**Głos:** znajomy kinoman, czyli życzliwy, konkretny, swobodny (na „Ty”), uczciwy i kompetentny.

| Sytuacja | Emocja | Ton | Humor | Entuzjazm | Formalność |
|---|---|---|:-:|:-:|:-:|
| Propozycje gotowe | ekscytacja | lekki | ●●○ | ●●● | ○○○ |
| Drobny sukces | zadowolenie | krótki | ●○○ | ●○○ | ○○○ |
| Brak wyników | rozczarowanie | pomocny | ●○○ | ●○○ | ○○○ |
| Błąd sieci | frustracja | spokojny, bez żartów | ○○○ | ○○○ | ●○○ |
| Płatności | nieufność | neutralny, przejrzysty | ○○○ | ○○○ | ●●○ |
| Usunięcie konta | stres | poważny, jednoznaczny | ○○○ | ○○○ | ●●○ |

Pełna matryca (9 sytuacji) i zasady stylu są w raporcie, w punkcie 3.

## 3. Mikrocopy – przed i po

Pomarańczowe znaczniki (C1, E4…) to identyfikatory zmian z tabel w raporcie.

| CTA i kontekst | Onboarding |
|---|---|
| ![](screenshots/pair-today.png) | ![](screenshots/pair-onboarding.png) |

| Błąd logowania (Przypadek B) | Brak filmu na platformach |
|---|---|
| ![](screenshots/pair-login.png) | ![](screenshots/pair-title.png) |

| Formularz (Przypadek C, Scenariusz 1) | Pusty stan + toast (Scenariusz 3) |
|---|---|
| ![](screenshots/pair-form.png) | ![](screenshots/pair-empty.png) |

| Anulowanie Premium (Scenariusz 2) | Usuwanie konta (Przypadek D) |
|---|---|
| ![](screenshots/pair-premium.png) | ![](screenshots/pair-delete.png) |

| Usuwanie z listy (Przypadek A) | Brak sieci / brak wyników |
|---|---|
| ![](screenshots/pair-remove.png) | ![](screenshots/pair-errors.png) |

## 4. Testy

**Test zakreślacza:** 🟩 wartość/instrukcja, 🟥 zbędne lub budzące wątpliwości. Wszystkie wersje v0 dostały werdykt „przepisać”, a wszystkie wersje końcowe „OK”. D2 przeszedł dwie iteracje.

![](screenshots/zakreslacz-1.png)
![](screenshots/zakreslacz-2.png)

**A/B etykiet:** 7 par oceniono według 5 kryteriów (czasownik, obiekt, przewidywalny skutek, ≤ 24 znaki, brak dwuznaczności). Za każdym razem wygrał wariant precyzyjny, np. „Anuluj subskrypcję” (5/5) zamiast „Anuluj” (2/5).

**Czytelność FOG-PL** (obliczenia własne, wyrazy trudne = 4 sylaby i więcej):

| Grupa | Przed | Po |
|---|:-:|:-:|
| Błędy i powiadomienia | 11,9 | 6,1 |
| Formularze | 5,7 | 4,3 |
| Puste stany i onboarding | 17,1 | 4,5 |
| Dialogi | 4,8 | 4,7 |
| **Razem** | **9,0** | **4,9** |

W dialogach FOG się nie zmienił, bo ich problemem była manipulacja, a nie mglistość tekstu. Dlatego wskaźnik trzeba łączyć z oceną jakościową.

---

Makiety wygenerowano z HTML/CSS (mid-fi). Zrzuty ekranu odtworzysz, otwierając `makiety/makiety.html` w przeglądarce.
