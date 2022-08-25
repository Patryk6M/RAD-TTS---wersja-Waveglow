# TTS z solidnym uczeniem się dopasowania, zróżnicowaną syntezą, generatywnym modelowaniem i drobiazgową kontrolą niskowymiarowych atrybutów mowy (F0 i energia).
To repozytorium zawiera kod źródłowy i kilka punktów kontrolnych dla naszej pracy opartej na RADTTS. RADTTS jest opartym na normalizacji przepływie szkieletem TTS z najnowocześniejszą wiernością akustyczną i wysoce odpornym modułem wyrównania audio-transkrypcji. Stronę naszego projektu i kilka próbek można znaleźć [tutaj](https://nv-adlr.github.io/RADTTS), z odpowiednimi pracami wymienionymi [tutaj](#relevant-papers).

To repozytorium może być użyte do trenowania następujących modeli:

- Normalizująca architektura dwudzielna do mapowania tekstu do spektrogramów melowych.
- Wariant powyższego, uwarunkowany na F0 i energię
- Modele przepływu normalizującego dla wyraźnego modelowania czasu trwania fonemów, częstotliwości podstawowej (F0) i energii.
- Samodzielny moduł wyrównania do uczenia się bez nadzoru wyrównania tekst-słuch, niezbędnego do treningu TTS.


## LICENCJA
Jeśli nie określono inaczej, kod źródłowy w tym repozytorium jest dostarczany na licencji
[MIT License](LICENSE)

## Podziękowania
Kod w tym repozytorium jest mocno inspirowany lub wykorzystuje kod źródłowy z następujących prac:

- Implementacja Tacotronu od [Keith Ito](https://github.com/keithito/tacotron/)
- Kod STFT od [Prem Seetharaman](https://github.com/pseeth/pytorch-stft)
- [Masked Autoregressive Flows](https://arxiv.org/abs/1705.07057)
- [Flowtron](https://arxiv.org/abs/2005.05957)
- Źródło funkcji neural spline użytych w tej pracy: https://github.com/ndeutschmann/zunis 
- Oryginalne źródło funkcji neuronowych splajnów: https://github.com/bayesiains/nsf 
- Architektura dwudzielna oparta na kodzie z [WaveGlow](https://github.com/NVIDIA/waveglow) 
- [HiFi-GAN](https://github.com/jik876/hifi-gan) 
- [Glow-TTS](https://github.com/jaywalnut310/glow-tts) 

## Autorzy

Rohan Badlani, Adrian Łańcucki, Kevin J. Shih, Rafael Valle, Wei Ping, Bryan Catanzaro. <br/>[One TTS Alignment to Rule Them All.](https://ieeexplore.ieee.org/abstract/document/9747707) ICASSP 2022
<br/><br/>
Kevin J Shih, Rafael Valle, Rohan Badlani, Adrian Lancucki, Wei Ping, Bryan Catanzaro. <br/>[RAD-TTS: Parallel flow-based TTS with robust alignment learning and diverse synthesis.](https://openreview.net/pdf?id=0NQwnnwAORi)<br/> ICML Workshop on Invertible Neural Networks, Normalizing Flows, and Explicit Likelihood Models 2021
<br/><br/>
Kevin J Shih, Rafael Valle, Rohan Badlani, João Felipe Santos, Bryan Catanzaro.<br/>[Generative Modeling for Low Dimensional Speech Attributes with Neural Spline Flows.](https://arxiv.org/pdf/2203.01786) Technical Report
