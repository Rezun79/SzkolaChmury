# TYDZIEN4.1
„Przeanalizuj proszę Azure Security i zainstaluj Endpoint protection na wcześniej utworzonych Vmkach. Przejrzyj usługę Azure Security Center oraz poszukaj opcję rekomendacji pod względem spełniania regulacji - Regulatory Compliance PCI DSS. W miarę możliwości postaraj się wdrożyć dane rekomendacje i podziel się swoimi wnioskami!”

## Endpoint protection:

Zainstalowany \
![Installed Endpoint protection](https://github.com/Rezun79/SzkolaChmury/blob/master/homework/week_4/Images/Endpoint_protection.jpg)

## Compliance

Bardzo szczegółowy raport, z jasnymi wskazówkami co do eliminacji niezgodności.
Udało się "testowo" wdrożyć kilka rekomendacji

\+ Pozwala lepiej zrozumieć wymagania regulatorów
\+ Daje Możliwość dokumentowania zgodności infrastruktury z wykogami regulatorów (np. generowanie raportów)


# TYDZIEN4.2
„Poprzez Azure Monitor zacznij monitorować dyski, CPU, Memory, a następnie podłącz maszyny do Log Analytics. Zacznij zbierać dane takie jak eventy z logu Apliacation oraz System. Postaraj się utworzyć własne dashboardy, w których pokazywane będą zbierane dane ze zdarzeń oraz danych performansowych (zachęcamy też do popatrzenia na inne dane i tego co da się osiągnąć dzięki Log Analytics w kwestii bezpieczeństwa. Proszę podziel się swoimi wnioskami!)

## Custom dasboard

Zbieranie metryk włączone, przygotowany dashboard"
![Dashboard](https://github.com/Rezun79/SzkolaChmury/blob/master/homework/week_4/Images/Dashboard.jpg)

## Events

Zbieranie zdarzeń włączone, przygotowany dashboard:
![Events](https://github.com/Rezun79/SzkolaChmury/blob/master/homework/week_4/Images/Events.jpg)

\+ Możliwość podłączenia alertów do Logs query


# TYDZIEN4.3
„Włącz dla maszyn Just-in-time (JIT) i zweryfikuj jakie zmiany nastąpiły na NSG oraz jak możesz zarządzać dostępem do maszyn. Dla utworzonych wcześniej maszyn wdróż usługę Azure Bastion, powyłączaj na VMkach Public IP. Podłącz się za pomocą Azure Basion do VM, opowiedz o plusach i minusach usługi”


## JIT
Po włączeniu JIT, z Azure Security Center, do NSG dodawane jest reguła blokująca połączenia (domyślnie dla 22,3389,5985,5986).

![JIT NSG](https://github.com/Rezun79/SzkolaChmury/blob/master/homework/week_4/Images/JIT.jpg)

W odpowiedzi na żądanie dostępu dodawana jest reguła odblokowująca ruch dla hosta/podsieci.

![JIT NSG Allow](https://github.com/Rezun79/SzkolaChmury/blob/master/homework/week_4/Images/JIT_Allow.jpg)


## Azure Bastion
Usługa włączona .. działa.

\+ wygodny sposób połączenia do VM \
\- konieczność wdrażania per VirtualNetwork \
\- cena (ok 130Euro\\miesiąc \
\- zauważalnie gorsza responsywność VM niż przy połączeniu RDP \
