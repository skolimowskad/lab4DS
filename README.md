# Laboratorium4 - sprawozdanie
<h3>Przestrzen nazw</h3>
Do utworzenia przestrzeni nazw "lab4" stworzony zostal plik o nnazwie <i>lab4-namespace.yaml</i>. Niniejszy plik YAML tworzy przestrzeń nazw "lab4" z dodatkowymi etykietami, które określają dostępne ograniczenia CPU i pamięci. Aby utworzyć przestrzeń nazw "lab4" z tymi ograniczeniami, wykonaj następującą komendę:
<br /><i>kubectl apply -f lab4-namespace.yaml</i>
<h3>Deployment</h3>
Deployment "restrictednginx" rowniez zostal stworzony dzieki plikowi YAML (<i>lab4_deployment.yaml</i>). Aby utworzyć Deployment "restrictednginx" w przestrzeni nazw "lab4" z podanymi ograniczeniami CPU i pamięci, wykonaj następującą komendę:
<br /><i>kubectl apply -f lab4-deployment.yaml</i>
<h3>Sprawdzenie poprawnosci</h3>
sprawdzenie stanu przestrzeni nazw "lab4":  <i>kubectl get namespace lab4</i>
<br />sprawdzenie stanu deploymentu w przestrzeni nazw "lab4": <i>kubectl get deployment restrictednginx -n lab4</i>
<br />sprawdzenie stanu podow w deploymencie: <i>kubectl get pods -n lab4</i>
