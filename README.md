Στόχος
Στόχος της παρούσας εργασίας είναι η ανάπτυξη ενός συστήματος πληθοποριστικών δεδομένων, που
αφορούν στην επισκεψιμότητα σημείων ενδιαφέροντος και τη διαχείριση πιθανής επαφής με κρούσμα
COVID-19.
Λειτουργικές Προδιαγραφές
Η διαχείριση της πανδημίας από την COVID-19 και των συνεπειών της αποτελεί πρόκληση σε πολλές χώρες
του κόσμου. Για τον έλεγχο της πιθανής διασποράς μπορούν να χρησιμοποιηθούν πληθοποριστικά
δεδομένα επισκεψιμότητας που ήδη συλλέγονται από παρόχους, όπως η Google και αφορούν στην
πυκνότητα επισκέψεων σε γεωγραφικά σημεία ενδιαφέροντος (POIs), όπως καταστήματα, εστιατόρια,
υπηρεσίες κατά τη διάρκεια της ημέρας και της εβδομάδας (popular times).
Η πυκνότητα επισκέψεων μπορεί να λειτουργήσει ως δείκτης της δημοφιλίας ενός μέρους, αλλά και ως
παράγοντας κινδύνου για πιθανή διασπορά COVID-19. Παράλληλα, αποτελεί μόνο εκτίμηση με βάση τα
δεδομένα γεωγραφικού εντοπισμού και δεν εξαρτάται από τον πραγματικό αριθμό επισκεπτών σε ένα
χώρο. Θα ήταν επομένως χρήσιμο να δίνεται η δυνατότητα σε έναν επισκέπτη να συνεισφέρει την
προσωπική του εκτίμηση για τον πραγματικό αριθμό των επισκεπτών.
Διατηρώντας με ανώνυμο τρόπο την πληροφορία των επισκέψεων, μπορεί να γίνει συνδυασμός με
καταχώρηση πιθανού κρούσματος, ώστε να υπάρχει ενημέρωση σε άλλους χρήστες αν βρέθηκαν στον ίδιο
χώρο με δηλωμένο κρούσμα. Έτσι, σκοπός της εργασίας είναι να κατασκευαστεί ένα σύστημα
πληθοποριστικής συλλογής δεδομένων επισκεψιμότητας και δήλωσης πιθανού κρούσματος με σκοπό την
παροχή πληροφοριών επισκεψιμότητας σε σημεία ενδιαφέροντος, αλλά και την ενημέρωση για πιθανή
επαφή με δηλωμένο κρούσμα, ως μέσο για έλεγχο της διασποράς. Στο σύστημα υπάρχουν δύο τύποι
χρηστών: Διαχειριστής και Χρήστης.
Χρήστης
Η αλληλεπίδραση με το χρήστη γίνεται μέσω προσαρμοστικού ιστοτόπου που επιτρέπει την πρόσβαση
μέσω σταθερού υπολογιστή ή κινητού τηλεφώνου, και έχει τις εξής δυνατότητες:
1) Εγγραφή στο σύστημα. Ο χρηστής εγγράφεται και αποκτά πρόσβαση στο σύστημα επιλέγοντας
κάποιο username & password της αρεσκείας του, και παρέχοντας το email του. Το password πρέπει
να είναι τουλάχιστον 8 χαρακτήρες και να περιέχει τουλάχιστον ένα κεφαλαίο γράμμα, ένα αριθμό
και κάποιο σύμβολο (π.χ. #$*&@).
2) Αρχική απεικόνιση χάρτη. Στον χρήστη εμφανίζεται ένας χάρτης με επίκεντρο τη γεωγραφική θέση
που βρίσκεται τη στιγμή της πρόσβασης. Η θέση του χρήστη εμφανίζεται με κατάλληλη οπτική
ένδειξη στο χάρτη. Ο χάρτης πρέπει να έχει κατάλληλο επίπεδο οπτικής μεγέθυνσης ώστε να
καλύπτει μια περιοχή ακτίνας όχι μικρότερης από 5χλμ από τη θέση του χρήστη. Στον χάρτη δεν
εμφανίζονται κατά την αρχική πρόσβαση markers που αντιστοιχούν σε POIs της βάσης δεδομένων.
3) Αναζήτηση σημείων ενδιαφέροντος. Μέσω πλαισίου ελεύθερης αναζήτησης μπορεί να αναζητήσει
σημείο ενδιαφέροντος (POI) από τη βάση δεδομένων του συστήματος, και το οποίο να είναι εντός
του ορατού εύρους του χάρτη για πιθανή επίσκεψη (εστιατόριο, καφέ, υπηρεσία κλπ). Tα
αποτελέσματα της αναζήτησης αυτής εμφανίζονται ως markers. Κάνοντας κλικ σε έναν marker
εμφανίζεται σε αναδυόμενο pop-up εκτίμηση της επισκεψιμότητας στο μέρος αυτό με βάση τα
δεδομένα που συλλέχθηκαν, για τις επόμενες 2 ώρες από την τρέχουσα. Επίσης εμφανίζεται ο μέσος
αριθμός των επισκεπτών με βάση τις καταχωρήσεις άλλων χρηστών, αν υπάρχουν ως και 2 ώρες
πριν την τρέχουσα χρονική στιγμή (βλ. επόμενο σημείο). Οι markers θα πρέπει να έχουν κατάλληλη
χρωματική ένδειξη ανάλογα με την εκτιμώμενη επισκεψιμότητα (0-32% Πράσινο, 33-65%
Πορτοκαλί, 66%+ Κόκκινο).
4) Καταχώρηση επίσκεψης. Για τα POIs που βρίσκονται εντός 20 μέτρων από την τοποθεσία του
χρήστη, εμφανίζεται, στο ίδιο pop-up με το (2), η επιλογή καταχώρησης της επίσκεψης του χρήστη.
Εφόσον ο χρήστης συναινέσει, αποθηκεύεται στη ΒΔ του συστήματος (server) η επίσκεψή του στο
συγκεκριμένο σημείο με τρέχον timestamp. Παράλληλα, έχει τη δυνατότητα να καταχωρήσει μια
εκτίμησή του για τον αριθμό των ατόμων στο σημείο (ακέραιος αριθμός).
5) Δήλωση κρούσματος. Ο χρήστης έχει τη δυνατότητα να δηλώσει στην εφαρμογή αν ο ίδιος αποτελεί
κρούσμα COVID-19 και πότε διαγνώστηκε (ημερομηνία). Εκ νέου δήλωση του ίδιου χρήστη δεν έχει
αποτέλεσμα, εκτός αν έχουν παρέλθει 14 ημέρες από την αρχική ημερομηνία διάγνωσης.
6) Πιθανή επαφή με κρούσμα. Ο χρήστης μπορεί να δει αν έχει έρθει σε επαφή με κρούσμα τις
τελευταίες 7 μέρες. Εμφανίζεται λίστα με τα σημεία ενδιαφέροντος που ο χρήστης επισκέφτηκε,
συμπεριλαμβανομένης ημερομηνίας και ώρας, και για τα οποία έχει καταγραφεί κρούσμα που: α)
βρισκόταν στο ίδιο σημείο με το χρήστη σε ένα εύρος +-2 ωρών και β) έχει διαγνωσθεί ως κρούσμα
εντός 7 ημερών από την επίσκεψη.
7) Επεξεργασία προφίλ. Ο χρήστης μπορεί να αλλάξει το username/password και να δει το αναλυτικό
ιστορικό των επισκέψεών του και δηλώσεων κρούσματος που έχει κάνει.
Διαχειριστής
Ο Διαχειριστής αποκτά πρόσβαση στο σύστημα με σταθερό υπολογιστή, μέσω κατάλληλου μηχανισμού
username / password. Ο διαχειριστής δεν εγγράφεται στο σύστημα αλλά δημιουργείται ως οντότητα
απευθείας στην σχετική βάση δεδομένων. Κατά την είσοδό του στο σύστημα έχει τις εξής δυνατότητες:
1) Ανέβασμα, ενημέρωση και διαγραφή δεδομένων. Ο διαχειριστής έχει τη δυνατότητα να φορτώσει
δεδομένα σημείων ενδιαφέροντος (POIs) και της επισκεψιμότητάς τους που πληρούν τις
προϋποθέσεις συμμόρφωσης με το πρότυπο δίνεται (JSON). Τα οποία αποθηκεύονται στη ΒΔ.
Μπορεί επίσης να επικαιροποιήσει τα δεδομένα αυτά, χωρίς όμως να δημιουργούνται
διπλοεγγραφές. Μπορείτε να θεωρήσετε ως ημερομηνία άντλησης των δεδομένων την ημερομηνία
τελευταίας τροποποίησης του αρχείου στο δίσκο. Επίσης μπορεί να επιλέξει τη διαγραφή όλων των
δεδομένων.
2) Απεικόνιση Στατιστικών. Ο διαχειριστής βλέπει σε μία σελίδα κατάλληλη πληροφορία, σε πίνακες
ή/και γραφήματα τα οποία απεικονίζουν:
a. Συνολικός αριθμός επισκέψεων που έχουν καταγραφεί.
b. Συνολικός αριθμός κρουσμάτων που έχουν δηλωθεί.
c. Συνολικός αριθμός επισκέψεων από ενεργά κρούσματα: Η επίσκεψη θα πρέπει να έχει γίνει
έως και 7 ημέρες πριν την ημερομηνία διάγνωσης κρούσματος και μέχρι 14 ημέρες μετά.
d. Κατάταξη των κατηγοριών σημείων ενδιαφέροντος που υπάρχουν στη ΒΔ του συστήματος,
με βάση το συνολικό πλήθος των επισκέψεων, όπως καταχωρείται από τους χρήστες.
e. Κατάταξη των κατηγοριών σημείων ενδιαφέροντος που υπάρχουν στη ΒΔ του συστήματος,
με βάση τον αριθμό κρουσμάτων που είχαν προσέλθει σε αυτά, έως και 7 ημέρες πριν την
ημερομηνία διάγνωσης κρούσματος και μέχρι 14 ημέρες μετά.
f. Εμφάνιση διαγράμματος ανά ημέρα, όπου:
i. Επιλέγεται ένα προκαθορισμένο εύρος (συγκεκριμένη εβδομάδα ή συγκεκριμένος
μήνας).
ii. Επιλέγεται με φίλτρο η δυνατότητα εμφάνισης ενός ή περισσότερων από τα
παρακάτω:
1. Το πλήθος των επισκέψεων που δηλώνουν οι χρήστες για κάθε ημέρα.
2. Το πλήθος των επισκέψεων από διαγνωσμένα κρούσματα για κάθε ημέρα
g. Εμφάνιση διαγράμματος ανά ώρα, όπου:
i. Επιλέγεται μια συγκεκριμένη ημερομηνία.
ii. Επιλέγεται με φίλτρο η δυνατότητα εμφάνισης ενός ή περισσότερων από τα
παρακάτω:
1. Η μεταβολή του αριθμού επισκέψεων ανά ώρα.
2. Η μεταβολή του αριθμού επισκέψεων από δηλωμένο κρούσμα ανά ώρα.
