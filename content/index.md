---
title: Σημειώσεις Αλγορίθμων
---

Στα άμεσα προβλήματα ο αλγόριθμος δεν γνωρίζει εξ αρχής όλα τα δεδομένα εισόδου. Θα εξετάσουμε τις εξής κατηγορίες προβλημάτων:

1. [[Άμεσοι Αλγόριθμοι]]: Η είσοδος παρουσίαζεται σταδιακά. Ο αλγόριθμος θα καλείται να παίρνει αποφάσεις με τα τωρινά δεδομένα χωρίς να γνωρίζει το μέλλον
2. [[Άμεση Εκμάθηση (Online Learning)]]: Εδώ θα συναντήσουμε αλγορίθμους πρόβλεψης. Γνωρίζοντας τις k πρώτες εισόδους, θα πρέπει να προβλέψουμε τι θα συμβεί στην k+1 είσοδο
3. Optimal Stopping (Στοχαστικές Είσοδοι): Στα προβλήματα αυτά έχουμε κάποια πληροφόρηση για τις τιμές εισόδου(με τη μορφή κάποια κατανομής). Τέτοιων τύπων προβλήματα είναι:
	-  [[Το πρόβλημα του γραμματέα]]
	- [[Προφητικές ανισότητες(prophet inequalities)]]

Στα άμεσα προβλήματα η δυσκολία είναι η έλλειψη πληροφορίας και όχι η έλλειψη υπολογιστικών πόρων. Ακόμα και εκθετικοί αλγόριθμοι πολλές φορές είναι ικανοποιητικοί
\
Συχνά σε όλες τις αναλύσεις που θα δούμε χρησιμοποιείται τo concept του competitive analysis(ανταγωνιστική ανάλυση). 