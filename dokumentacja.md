### Zadanie 1 

****


** Utworzenie clusterip servicu dla deploymentu oraz 'dopasowanie' podow**
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/07a316cf-5690-4cb9-b8eb-6c58ecd34c23" />
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/776086f4-64b5-45b9-b9b5-7e88f5447ff9" />


### Zadanie 2

**instalacja longhorna**
<img width="1919" height="1037" alt="image" src="https://github.com/user-attachments/assets/f86dfef3-15b7-4058-93ee-269ced76b7d4" />

**Utworzenie deploymentu z danymi prezesa (nazwa utworzona aby oszukać hakerów żeby nie wiedzieli że są to dane prezesa)**
<img width="1263" height="908" alt="image" src="https://github.com/user-attachments/assets/8c8a6052-4acc-4a37-8cf0-b73bb3fbb563" />


**Następnie dodanie persisten volume claima do poda i podlaczenie dla prezesa**
<img width="1254" height="911" alt="image" src="https://github.com/user-attachments/assets/368f097f-f80e-45eb-bb9a-99b7b7f57dde" />

<img width="1242" height="904" alt="image" src="https://github.com/user-attachments/assets/4bbe8653-031e-4a86-8f2d-1444170fed45" />

### Zadanie 3
** Poprawka httpdd na httpd **
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/f51c6012-3b8e-435a-9e7f-c9241d5a9503" />
** Poprawka target portu z 8080 na 80**
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/26aae94b-9cbd-4169-9e4a-81581dfdcd24" />

** poprawka na ksiegowy-app **
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/f90aa929-4c07-4eb7-9fa9-c2e2df1ec502" />


** aktywny system premii **
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/b5c023e8-8349-46a7-9676-196a70fdb04d" />


### Zadanie 5

** Przeskalowanie do 5 replik **
<img width="1258" height="907" alt="image" src="https://github.com/user-attachments/assets/a5514815-9875-4edd-92a3-badf32657387" />
** Ustawienie limitów dla ns ksiegowosc-prod **
<img width="1905" height="908" alt="image" src="https://github.com/user-attachments/assets/ec233dec-6cb5-48f2-a892-a584a19ff271" />

### zadanie 6

** ustawienie init container z komenda pobierajaca index.html**
<img width="1241" height="908" alt="image" src="https://github.com/user-attachments/assets/4d496a66-006c-4576-b422-b6fcaf337f43" />


** Strona z adresem https **
<img width="1914" height="984" alt="image" src="https://github.com/user-attachments/assets/e68d995d-4bf4-4858-8480-0d2e97eec66f" />

### Zadanie 8

<img width="947" height="243" alt="image" src="https://github.com/user-attachments/assets/a4ab3b6a-50ac-4728-8cc6-b9a182a1ef91" />

RBAC: Dodałem ClusterRoleBinding. Bez tego initContainer wyrzuciał błąd: Forbidden (403): nodes is forbidden.
Zmieniłem ścieżkę z /healthz na / inaczej trzeba by bylo zmieniac konfig nginxa.

Timery Probea: ustawienie periodSeconds: 2 i initialDelaySeconds: 2 skutkuje tym ze jak kontener zostanie zlagowany to kubernetes moze go zabic.

