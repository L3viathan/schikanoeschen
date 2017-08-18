# Liga-Regeln

Diese Liga-Regeln betreffen die Liga eines bestimmten `#schika`-Kanals eines
bestimmten Slack-Teams, das ungenannt bleibt.

## Mitgliedschaft und Ligaspiele

Durch das Spielen eines Ligaspiels gegen ein aktives Mitglied der Liga wird ein
Nicht-Mitglied zu einem Mitglied der Liga. Neue Mitglieder fangen mit dem Rang
1000 an. Wenn ein Mitglied inaktiv wird (indem es acht Wochen lang keine
Ligaspiele spielt, oder es explizit erwünscht), wird es als solches markiert
und nicht mehr in der offiziellen Rangliste aufgeführt, ihr Rang jedoch bleibt
gespeichert. Wenn es wünscht, wieder aktiv zu werden, oder durch das Spielen
eines Ligaspiels gegen ein aktives Mitglied wird ein inaktives Mitglied wieder
aktiv.

Spiele zwischen zwei aktiven Spielerinnen sind Ligaspiele, außer beide
Spielerinnen werden sich vor dem Spiel darüber einig, dass es kein Ligaspiel
sein soll.

Alle Ligaspiele werden nach den offiziellen Spielregeln gespielt. Wenn beide
Spielerinnen sich vor dem Spiel über modifizierte Regeln einig sind, können sie
auch ein Ligaspiel mit diesen modifizierten Regeln spielen, aber dies muss vor
jedem solchem Spiel explizit geschehen.

## Ränge und das ELO-System

Die Rangliste basiert auf dem
[ELO-System](https://en.wikipedia.org/wiki/Elo_rating_system).

Nachdem eine Spielerin ein Spiel gespielt hat, wird ihr neuer Rang nach der
folgenden Formel berechnet.

    k = 16
    S = 1 wenn du gewinnst, 0 wenn du verlierst, 0.5 bei Unentschieden
    r(jemand) = alter Rang
    R(jemand) = 10**(r(jemand)/400)
    Neuer Rang = round(r(du) + k*(S-R(du)/(R(du)+R(Gegner))))

@l3viathan ist für die technische Umsetzung von Speicherung und Berechnung der
Ränge verantwortlich.

## Aktivitätsstrafen

Inaktivität über einen längeren Zeitraum wird durch Punktabzug bestraft. Diese
Strafe betrifft nur aktive Mitglieder. Außerdem gibt es eine feste Strafe für
das inaktiv werden.

- Wenn ein Mitglied inaktiv wird (außer dies geschieht durch die achtwöchige
  Frist), wird seine Punktzahl um 10 reduziert. Dies wird nicht nachträglich
  auf bereits inaktive Mitglieder angewendet.
- Wenn ein Mitglied in x aufeinanderfolgenden Wochen (eine Woche in diesem
  Sinne ist das Intervall von Montag, 0:00 bis Sonntag, 24:00) keine
  Ligaspiele gespielt hat, wird seine Punktzahl um x^2 (1, 4, 9, 16, ...)
  reduziert. Nachdem die Punktzahl um 64 reduziert wurde (für die achte
  aufeinanderfolgende Woche), wird es automatisch als inaktiv markiert und
  verliert keine weiteren Punkte durch Inaktivität.

@l3viathan ist für die Einhaltung dieser Regeln verantwortlich, umsetzbar
entweder durch manuelle Anpassung der Punkte, oder die Automatisierung der
Aufgabe.

## Änderung der Spielregeln

Änderungen der Spielregeln können nach dem folgenden Wahlsystem vollzogen
werden. Es ist nicht geheim.

1. Dieses Repository forken, die vorgeschlagene Änderung in den Spielregeln
   machen (am besten in beiden Sprachen).
2. Einen Pull-Request zu diesem Repository machen.
3. Den Antrag in `#schika` ankündigen, selbst wenn dies schon automatisch
   geschah, inklusive einer Frist, die nicht weniger als eine Woche vom
   Zeitpunkt der Ankündigung sein darf.
4. Wenn jede aktive Spielerin den neuen Regeln zustimmt (mit Emoji-Reaktionen)
   bevor die Frist abgelaufen ist, gilt der Vorschlag als angenommen.
5. Wenn die Frist abgelaufen ist, und noch nicht jede aktive Spielerin den
   Änderungen zugestimmt hat, wird jede Enthaltung in eine Zustimmung
   verwandelt. Wenn nach dieser Anpassung mehr Stimmen für als gegen die
   Änderung eingegangen sind, gilt der Vorschlag als angenommen. Im Fall einer
   Stimmengleichheit gilt der Vorschlag als abgelehnt.
6. Wenn der Vorschlag abgelehnt wurde, wird der Pull-Request geschlossen.
7. Wenn der Vorschlag angenommen wurde, wird der Pull-Request gemerged und die
   neuen Regeln sind in Kraft.

## Änderug der Liga-Regeln

Änderungen der Liga-Regeln können nach dem folgenden Wahlsystem vollzogen
werden. Es ist nicht geheim.

1. Dieses Repository forken, die vorgeschlagene Änderung in den Liga-Regeln
   machen (am besten in beiden Sprachen).
2. Einen Pull-Request zu diesem Repository machen.
3. Den Antrag in `#schika` ankündigen, selbst wenn dies schon automatisch
   geschah, inklusive einer Frist, die nicht weniger als eine Woche vom
   Zeitpunkt der Ankündigung sein darf.
4. Wenn jede aktive Spielerin den neuen Regeln zustimmt (mit Emoji-Reaktionen)
   bevor die Frist abgelaufen ist, gilt der Vorschlag als angenommen.
5. Wenn die Frist abgelaufen ist, und noch nicht jede aktive Spielerin den
   Änderungen zugestimmt hat, wird jede Enthaltung in eine Zustimmung
   verwandelt. Wenn nach dieser Anpassung mehr Stimmen für als gegen die
   Änderung eingegangen sind, gilt der Vorschlag als angenommen. Im Fall einer
   Stimmengleichheit gilt der Vorschlag als abgelehnt.
6. Wenn der Vorschlag abgelehnt wurde, wird der Pull-Request geschlossen.
7. Wenn der Vorschlag angenommen wurde, wird der Pull-Request gemerged und die
   neuen Regeln sind in Kraft.
