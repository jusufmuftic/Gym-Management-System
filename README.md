# AKO SE ODLUCIMO ZA OVO TREBA I README PROMIJENIT

# Gym-Management-System

Ova baza podataka sistema upravljanja teretanom dizajnirana je za efikasno upravljanje različitim aspektima teretane, uključujući pretplate za članove, trenere, opremu i osoblje.

# Tables
1. **Trainer**
   
   - Čuva informacije o trenerima u teretani.
     
2. **Subscription**

   - Upravlja članovskim pretplatama s detaljima poput datuma početka, datuma završetka, vrste paketa i cijene.

3. **Gym**

   - Sadrži informacije o lokacijama teretane.
     
4. **Worker/employes** CSV

   - Čuva podatke o radnicima u teretani, uključujući njihove plate i uloge. U sebi ima foreign key 'gym_id' koji ga povezuje sa tabelom gym one to many vezom, jer jedan worker moze da radi u samo jednoj teretani a jedna teretana moze da ima vise workers-a
     
5. **Plan**

   - Upravlja različitim članstvenim planovima koje nudi teretana, uključujući naziv plana, cijenu i broj sesija.
     
6. **Equipment**

   - Čuva detalje o opremi u teretani dostupnoj za korištenje.
     
7. **Gym_Trainer**
   
   - Uspostavlja vezu između teretana i trenera. Tabele Gym i Trainer su povezane many to many vezom jer jedan trener moze da radi u vise teretana a i u jednoj teretani moze da radi vise trenera.
     
8. **Gym_Equipment**

   - Povezuje lokacije teretane s dostupnom opremom i njihovim količinama. Tabele Gym i Equipment su povezane many to many vezom jer se jedna sprava moze nalaziti u vise teretana kao sto i jedna teretana moze imati vise sprava.
  
9. **Members**

   - Sadrži informacije o članovima teretane, uključujući njihove lične podatke, dodijeljene trenere, pretplatne planove i popuste. Ima par foreign keys:'plan_id','trainer_id','subscription_id' koji je povezuju sa tabelama redom: plan, trainer, subscription one to many vezom. jedan member moze da ima samo jedan plan a jedan plan moze da ima vise member-a, jedan trener moze da vjezba vise membera ali jedan member moze da ima samo jednog trenera, jedan member moze da bude pretplacen na samo jedan subsctiption a vise membera moze da bude pretplaceno na jedan subscription.
  
# Inserts

   - O insertima se nema reci nista specijalno, tu smo samo unijeli nekoliko nasumicnih primjera da provjerimo da li nam rade upiti.

# Contributors

1. Jusuf Muftić
2. Mustafa Gradišić
3. Ahmed Alijagić

# Version History

- 2024: Beta version
     
