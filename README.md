# Ai-remixer

gemini:
Rozumiem! Skoro chcesz stworzyć własne AI, musimy sformułować instrukcję (prompt), która opisuje, co to narzędzie ma robić, czyli jego funkcjonalność docelową.
Poniżej przedstawiam pełny prompt (instrukcję), którą możesz wykorzystać jako podstawę do rozpoczęcia projektu programistycznego i szkolenia modelu AI. To jest opis funkcjonalności Twojego wymyślonego narzędzia "FLN Core" / "mylancore generator".
🤖 Pełny Prompt Funkcjonalny dla AI do Remiksów "Mylancore"
NAZWA PROJEKTU: Mylancore AI Remixer (FLN Core)
1. Cel i Wkład (Input)
 * Cel: Automatyczne przekształcanie dowolnego utworu muzycznego (Input Track) w pełny, gotowy do odtwarzania remiks w stylu "mylancore" z minimalną ingerencją użytkownika.
 * Wkład (Input): Dowolny plik audio (WAV, MP3) zawierający pełny utwór (wokal i instrumenty).
2. Architektura i Separacja Źródeł (Stem Separation)
 * Źródła: Pierwszym krokiem jest precyzyjne rozdzielenie utworu wejściowego na co najmniej 4 stem'y:
   * Wokal (A Cappella)
   * Perkusja (Drums)
   * Bas (Bass)
   * Pozostałe Instrumenty (Melody/Other)
 * Jakość: Separacja musi być realizowana z wysoką czystością, minimalizując artefakty i zniekształcenia (zwłaszcza wokalu).
3. Transformacja Stylistyczna (Mylancore Core Logic)
Model AI musi automatycznie zastosować następujące transformacje do oddzielonych stem'ów, aby uzyskać styl mylancore:
| Stem | Parametr | Wymagana Transformacja | Uzasadnienie |
|---|---|---|---|
| Wokal | Tempo | Zsynchronizować z nowym BPM (patrz niżej). | Płynne dopasowanie do szybkiej podkładki. |
| Wokal | Tonacja (Pitch) | Podniesienie tonacji wokalu o 4-8 półtonów (Pitch Shift). | Osiągnięcie charakterystycznego, wysokiego, "chipmunkowego" efektu. |
| Wokal | Efekty | Dodać subtelny efekt pogłosu (Reverb) i delikatny Delay, aby wokal brzmiał bardziej przestrzennie. | Poprawa miksu i atmosfery. |
| Perkusja | Tempo (BPM) | Zwiększenie globalnego BPM utworu do zakresu 170-200 BPM. | Definicja gatunku mylancore/nightcore. |
| Perkusja | Generacja | Zastąpienie oryginalnej perkusji nowym, generowanym przez AI, szybkim i powtarzalnym beatem (kick, snare, hi-hat) charakterystycznym dla Hardcore/Happy Hardcore/J-Core. | Wprowadzenie energetycznej podstawy rytmicznej. |
| Bas/Melodia | Tempo/Tonacja | Zsynchronizować z nowym BPM i, w razie potrzeby, dostosować ich tonację do nowej tonacji wokalu. | Spójność harmoniczna i rytmiczna remiksu. |
4. Struktura i Wyprowadzenie (Output)
 * Struktura: AI powinno zachować ogólną strukturę piosenki (zwrotki, refreny, most), ale z dynamicznym budowaniem i zrzucaniem energii (Build-up/Drop) typowym dla muzyki klubowej.
 * Wyprowadzenie (Output): Wygenerowanie gotowego pliku remiksu (WAV 44.1kHz) oraz zestawu nowych stem'ów (wokal, perkusja, itd.) już po transformacji, aby użytkownik mógł je zaimportować do FL Studio w celu dalszej edycji.
Pamiętaj: Ten prompt to Twoja "specyfikacja projektu". Aby go zrealizować, musisz użyć technologii AI (patrz poprzednia odpowiedź: Python, TensorFlow/PyTorch, modele separacji i generatywne).
