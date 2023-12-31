# ASR_and_science_podcasts

Herzlich Willkommen auf diesem GitHub Repository, 
auf dem ich die Ergebnisse und Skripte meiner Bachelorarbeit "Transkription wissenschaftlicher Podcasts unter Verwendung von automatischen Spracherkennungssystemen" präsentiere. Zusätzlich biete ich Ihnen hier die Möglichkeit, auf die Datengrundlage zuzugreifen, die im Rahmen meiner Forschung verwendet wurde. Über die bereitgestellten Links finden Sie weitere Informationen zu den Daten und können diese dort herunterladen beziehungsweise anfordern.

## Abstract
Der digitale Wandel, getrieben durch die Evolution von "New Media mit ihren interaktiven, multimedialen Merkmalen und globaler Zugänglichkeit, hat nachhaltige Auswirkungen auf die Bereiche Journalismus, Unterhaltung und Wissenschaftskommunikation hinterlassen. Innerhalb dieses Rahmens dienen Podcasts als zugängliche, offene Plattform zur Verbreitung wissenschaftlicher Informationen und zur Förderung interdisziplinärer Diskussionen, wobei Herausforderungen im Hinblick auf die auditiven Eigenschaften und die Notwendigkeit evidenzbasierter Kommunikation bestehen. Das Hauptziel dieser Studie besteht darin, die jüngsten Fortschritte in KI-gesteuerten Transkriptionsverfahren zu nutzen, um effiziente und hochwertige Transkriptionen zu realisieren. Darüber hinaus werden neue Ansätze zur Steigerung der Auffindbarkeit, Zugänglichkeit und Verbreitung wissenschaftlicher Inhalte diskutiert. Für diese Studie wurden Audio-Daten aus dem bilingualen Common Voice-Datensatz und dem englischsprachigen GigaSpeech-Datensatz verwendet, um automatisierte Transkriptionen zu erstellen. Die Transkriptionen wurden anschließend mithilfe von Metriken wie der Wortfehlerrate und des Jaro-Winkler-Ähnlichkeitsmaß bewertet. Die Ergebnisse dieser Untersuchung verdeutlichen, dass die Genauigkeit des ASR-Modells "Whisper" von OpenAI von verschiedenen Faktoren abhängig ist. Hierzu zählen die Sprache, verschiedene Dialekte, Akzente, Altersgruppen und Themengebiete. Im Gesamten betrachtet konnte die Transkription von englischen im Vergleich zu deutschen Daten präziser durchgeführt werden. Trotz gelegentlicher Fehler zeigten die durch ASR generierten Transkriptionen eine signifikante Ähnlichkeit zur Ground Truth, was auf ihr Potenzial für die Transkription von Podcasts hinweist. Ein Vergleich verschiedener Modellgrößen ergab, dass größere Modelle eine überlegene Leistung erbrachten. Diese robusten Ergebnisse legen nahe, dass Transkriptionen eine sinnvolle Ergänzung zu den vorhandenen Metadaten von Podcasts darstellen und zur Verbesserung von Retrieval-Anwendungen genutzt werden können. Des Weiteren bieten Transkriptionen eine solide Grundlage für die Anwendung fortgeschrittener Methoden des NLP zur Extraktion entscheidender Informationen, wie beispielsweise Verweise und Entitäten, welche in ein vernetztes System, wie Knowledge Graphs, integriert werden können, um Podcast-Inhalte auf effiziente Weise zu strukturieren und Verknüpfungen zu anderen Wissensquellen herzustellen.

## Inhalt

- **Common_voice:** Enthält die Ergebnisse die auf den Daten des Common Voice Datensatzes erzielt wurden. 

- **GigaSpeech:** Enthält die Ergebnisse die auf den Daten des GigaSpeech Datensatzes erzielt wurden.

- **summary:** Enthält Übersichten der wichtigsten Parameter, sowie des Modellvergleichs und die erstellten Plots

- **Skripte:** Dieser Ordner enthält die Python-Skripte, die zur Erstellung der in der Arbeit präsentierten Ergebnisse verwendet wurden.

## Ergebnisse

Es wurde die Anwendbarkeit des ASR-Modells Whisper auf die Transkription von wissenschaftlichen Podcasts untersucht. Als Grundlage dafür dienten Auszüge aus dem bilingualen Common Voice Datensatz von Mozilla und dem englischsprachigen GigaSpeech Datensatz.
Zur Transkription wurde das kleinste Whisper-Modell verwendet. Die Ergebnisse zeigen, dass die WER abhängig von der Sprache und dem verwendeten Datensatz variiert. Es wurde deutlich, dass englische Daten besser verarbeitet wurden als deutsche. Zusätzlich zur WER wurde das Jaro-Winkler-Ähnlichkeitsmaß verwendet. Trotz hoher WER wurde festgestellt, dass die Transkripte eine hohe Ähnlichkeit zur Ground Truth aufwiesen. Dies deutet darauf hin, dass es sich meist um kleinere Orthographiefehler, Wortdreher, Löschungen und Einfügungen handelt, die im Gesamteindruck jedoch wenig ins Gewicht fallen. Im Bezug auf Altersgruppen des Common Voice Datensatzes zeigte sich, dass es eine scheinbare positive Korrelation zwischen Altersgruppen und WER gab. Diese Beziehung erwies sich nach Unterteilung der Daten in englisch- und deutschsprachige Sprecher jedoch als nicht eindeutig. Bei der Unterteilung in Akzentgruppen konnte die Vermutung, dass Akzente und Dialekte tendenziell schwerer zu transkribieren sind, bestätigt werden. Die Untersuchung des Gigaspeech Datensatzes ergab, dass Podcasts besser transkribiert wurden als Audiobooks oder Auszüge von YouTube-Videos. Insbesondere in der Kategorie "Science and Technology" schnitten Podcasts im Vergleich zu YouTube-Videos gut ab, mit einer hohen Ähnlichkeit zur Ground Truth und einer niedrigen WER von 7,8%. In einem direkten Modellvergleich zeigte sich, dass die WER mit zunehmender Modellgröße abnahm. Dies zeigt, dass die Leistung des ASR-Modells mit mehr Ressourcen und Trainingsdaten verbessert werden kann. Schlussendlich wurden Nomen, Verben, Eigennamen, Adjektive und Adverben als häufigste Fehlerquelle identifiziert.

## Skripte

Die Ergebnisse können unter Verwendung der bereitgestellten Daten und Skripte repliziert werden. Hierzu wird das Skript "BA_ASR_and_science_podcasts.ipynb" benötigt, sowie die .tsv-Dateien, welche sich in den Ordnern 'Common_voice', 'GigaSpeech' und 'summary'befinden. Stellen Sie sicher, dass alle verwendeten Bibliotheken, die zu Beginn des Skripts importiert werden, installiert sind. Des Weiteren benötigen Sie eine Installation von FFmpeg zur Ausführung von Whisper. Die nötigen Links sind ebenfalls im Skript eingebunden.

## Weiterführende Links

- [Common Voice](https://github.com/common-voice/common-voice)
- [GigaSpeech](https://github.com/SpeechColab/GigaSpeech)
- [Open Science Radio](https://www.openscienceradio.org/)
