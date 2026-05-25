
# Zbadać aktualny stan wiedzy (3 punkty): Należy krótko opisać istniejące podejścia i rozwiązania dla podobnych problemów

## 1. Ogólny wpływ AI na rozwój akademicki

**Źródło:** [Vieriu, A. M., & Petrea, G. (2025). The Impact of Artificial Intelligence (AI) on Students' Academic Development](https://www.mdpi.com/2227-7102/15/3/343)

**Treść:** Badanie przeprowadzone zostało na grupie 85 studentów kierunków inżynieryjnych. Z analizy wynika, że korzystanie z narzędzi AI stało się powszechną, codzienną praktyką – aż 95,6% studentów deklaruje ich używanie, opierając się głównie na wirtualnych asystentach (takich jak ChatGPT, Siri lub Google Assistant) oraz platformach adaptacyjnych (Coursera, Duolingo, etc.).

**Proponowane podejścia i rozwiązania:**

* organizację systemowych szkoleń dla studentów i wykładowców z zakresu prompt engineeringu i krytycznej oceny źródeł,
* stworzenie oficjalnych uczelnianych protokołów weryfikacji prac (zamiast zawodnych detektorów AI),
* oraz wdrożenie sztywnych polityk prywatności chroniących dane studentów wprowadzane do modeli komercyjnych.

**Dlaczego pasuje do tematu:** Artykuł ten bezpośrednio uzasadnia strukturę i spodziewany rozkład cech w naszym zbiorze danych. Wykazany przez autorów masowy odsetek studentów korzystających z AI pozwala nam założyć, że zmienna `Weekly_GenAI_Hours` w większości obserwacji będzie przybierać wartości niezerowe, co czyni z niej kluczowy predyktor w modelu. Ponadto badanie skupiające się na studentach kierunków inżynieryjnych dostarcza tła do analizy zmiennej `Major_Category`. Pozwala nam to zweryfikować, czy studenci kierunków technicznych wykazują inne wzorce zachowań, takie jak wyższe `Tool_Diversity` czy specyficzne `Primary_Use_Case` oraz jak te profile korelują z ostatecznym poziomem `Burnout_Risk_Level`.

## 2. Interakcja i zaangażowanie w środowisku cyfrowym

**Źródło:** [Seo, K., Tang, J., Roll, I., Fels, S., & Yoon, D. (2021). The impact of artificial intelligence on learner-instructor interaction in online learning.](https://link.springer.com/article/10.1186/s41239-021-00292-9?src_trk=em6718a9d972d857.274398601191650753)

**Treść:** Badanie analizuje, jak systemy AI zmieniają dynamikę i oczekiwania w relacjach między studentami a wykładowcami. Przeniesienie ciężaru pozyskiwania wiedzy i wsparcia na narzędzia AI może osłabiać tradycyjne interakcje, ograniczać bezpośredni feedback od prowadzących oraz wpływać na poczucie osamotnienia w procesie edukacyjnym.

**Proponowane podejścia i rozwiązania:**

* projektowanie narzędzi AI w sposób, który wspiera i stymuluje (a nie zastępuje) bezpośrednią komunikację człowiek-człowiek,
* wyraźne określenie granic roli wirtualnych asystentów jako wsparcia technicznego, a nie mentorskiego,
* wdrażanie strategii dydaktycznych przeciwdziałających cyfrowej izolacji studentów.

**Dlaczego pasuje do tematu:** Choć nasz zbiór danych nie mierzy bezpośrednio liczby interakcji międzyludzkich, artykuł ten dostarcza kluczowego tła teoretycznego do interpretacji zmiennych takich jak `Weekly_GenAI_Hours`, `Perceived_AI_Dependency` oraz `Primary_Use_Case`. Pozwala on wysnuć przypuszczenie, że studenci spędzający nieproporcjonalnie dużo czasu z AI kosztem tradycyjnej nauki `Traditional_Study_Hours`, potencjalnie izolują się od środowiska akademickiego. Publikacja Seo et al. sugeruje, że to właśnie ten ukryty mechanizm cyfrowej izolacji i braku ludzkiego wsparcia może być główną przyczyną wzrostu wskaźników `Anxiety_Level` oraz `Burnout_Risk_Level`.

## 3. Negatywne skutki i ryzyka poznawcze

**Źródło:** [Basha, J. Y. (2024). The Negative Impacts of AI Tools on Students in Academic and Real-Life Performance.](https://nsfjournals.com/article-files/pdf/WyWmemNe8hyG6vgiQoPO-1723214664.pdf)

**Treść:** Artykuł koncentruje się na negatywnych skutkach nadmiernego polegania na narzędziach AI, analizując ich wpływ zarówno na wyniki akademickie, jak i na codzienne funkcjonowanie studentów. Literatura wskazuje, że bezkrytyczne korzystanie z AI prowadzi do tzw. zjawiska „lenistwa intelektualnego”, osłabienia zdolności zapamiętywania, zaniku umiejętności samodzielnego podejmowania decyzji oraz uzależnienia od gotowych rozwiązań technologicznych.

**Proponowane podejścia i rozwiązania:**

* promowanie zrównoważonego podejścia i higieny cyfrowej wśród studentów,
* transformacja metod oceniania przez wykładowców – przesunięcie punktu ciężkości z testowania suchej wiedzy na zadania wymagające unikalnych ludzkich kompetencji, takich jak krytyczna analiza, myślenie projektowe i rozwiązywanie problemów w czasie rzeczywistym,
* edukacja w zakresie etyki AI i rozwijanie świadomości dotyczącej długofalowych skutków poznawczych nadmiernego wyręczania się algorytmami.

**Dlaczego pasuje do tematu:** Opisane przez autora zjawiska „lenistwa intelektualnego” i uzależnienia od gotowych rozwiązań znajdują swoje bezpośrednie odzwierciedlenie w kolumnach `Perceived_AI_Dependency` oraz `Skill_Retention_Score`. Artykuł ten pozwala nam sformułować logiczną ścieżkę dla modelu predykcyjnego: wysoki poziom zależności od AI może powodować obniżenie realnych zdolności poznawczych, co w obliczu tradycyjnych wymagań akademickich generuje frustrację, podnosi `Anxiety_Level` i w konsekwencji staje się bezpośrednim katalizatorem dla `Burnout_Risk_Level`.
