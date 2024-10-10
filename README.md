#Pràctica Android
Aquesta pràctica té una carpeta que tindra un projecte per a fer en Android Studio el qual es un comptador,i l'objectiu és fer botons de decrementar i de tornar a 0, i aquest es divideix en 3 blocs:
1. Bloc 1. Activitats sobre el comptador.
  - Anàlisi de l'estructura del projecte.
  - Activitats sobre el cicle de vida i la pèrdua d'estat.
  - Intents entre activitats.
2. Bloc 2. Comptador amb MVVM
3. Bloc 3. Comptador amb Compose
## Bloc 1 
  ### Activitats sobre el comptador
  Aquest projecte de Android és una Activitat buida la qual té la següent estructura i les carpetes obertes són les més importants:
  ![Foto de exemple](https://github.com/user-attachments/assets/0d53ac47-5088-47ef-ae0b-27f58b7cb4ec)
    - kotlin+java/com.pmdm.ieseljust.comptador.
        Ací està el main i el mainActivity, els principals per a fer la aplicació.
    - res/layout
        Ací estan la interfaç de la aplicació.
  ### Activitats sobre el cicle de vida i la pèrdua d'estat
  En el projecte hi ha un problema en el comptador, i es que al hora de girar la pantalla el comptador independentment que
  si has tocat el botó de rest o no el comptador torna a 0 i la solució està en el procés de OnSaveInstance i OnRestoreInstance,
  el que has de fer és guardar el valor actual en OnSaveInstance quan tanques la aplicació o quan gires la pantalla i carregar-lo en OnRestoreInstance
  quan obris l'aplicació o quan gire la pantalla
  ### Intents entre activitats
  En "activity_main.xml" ens fixem en el següent per a posar el botó:
  ![Foto per al botó](https://github.com/user-attachments/assets/f0b4784a-e8b7-4b5f-8f27-a432cf505c52)
  
  i els arrastrem a la interfaç on nosaltres vullgam.
## Bloc 2
   En aquest bloc anirem al main i posarem les funcions dels botons(El nom de les funcions tenen que ser iguals als que hem posat als botons ex:Si li posem al botó bot0 la funció es tindra que dir bot0) 
   i el que és fa és amb la funció actualtzarem el comptador per a que o disminuisca o es pose a 0 in per últim usar el toString() per a que el número es mostre en pantalla.
  ## Bloc 3
  En aquest bloc posarem els botons per a que queden en la mateixa direcció, i és fa amb:
  ![Layout botons](https://github.com/user-attachments/assets/914e4b46-f299-4292-bd8c-9d950e0395f0)
  i
  ![Botons units](https://github.com/user-attachments/assets/7ef17b5b-2638-41fd-874c-1e948fd0258d)
  En la segona imatge posem les fletxes indicades per cercles per dalt i per baix al botó + per a que és quede centrat respecte al botó del +
  i corregim imperfeccions cambiant els valors en el layout de la primera imatge
+  
