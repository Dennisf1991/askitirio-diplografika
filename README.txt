ΑΣΚΗΤΗΡΙΟ ΔΙΠΛΟΓΡΑΦΙΚΩΝ - ΟΔΗΓΟΣ DEPLOY
=========================================

ΤΡΟΠΟΣ Α - RENDER (δωρεαν, δημοσιο link, ~3 λεπτα)
--------------------------------------------------
1. Φτιαξε ενα GitHub repo και ανεβασε ολα τα αρχεια αυτου του φακελου
   (server.js, package.json, render.yaml, public/index.html).
2. Πηγαινε render.com -> New -> Web Service -> συνδεσε το repo.
3. Το Render διαβαζει το render.yaml και στηνει τα παντα μονο του.
   (Runtime: Node, Build: npm install, Start: npm start)
4. Σε λιγα λεπτα παιρνεις link της μορφης:
   https://askitirio-diplografika.onrender.com
   Αυτο το link το δινεις σε οποιον θελεις.

Σημ: Στο δωρεαν πλανο, ο server "κοιμαται" μετα απο αδρανεια και
ξυπναει στην πρωτη επισκεψη (10-30 δευτ. καθυστερηση). Για συνεχη
λειτουργια, αναβαθμιση σε πληρωμενο πλανο.

ΤΡΟΠΟΣ Β - SYNOLOGY NAS (δικος σου server)
-------------------------------------------
Δεν χρειαζεσαι καν το Node. Απλα:
1. Package Center -> εγκατεστησε "Web Station".
2. Αντεγραψε το public/index.html στον φακελο web (π.χ. /web/askitirio/).
3. Ανοιξε: http://<IP-του-NAS>/askitirio/
Για προσβαση απο εξω, ενεργοποιησε QuickConnect ή reverse proxy.

ΤΡΟΠΟΣ Γ - NETLIFY (πιο απλο, δωρεαν)
--------------------------------------
1. Πηγαινε app.netlify.com/drop
2. Συρε ΜΟΝΟ το αρχειο public/index.html (μετονομασε το σε index.html).
3. Παιρνεις αμεσα δημοσιο link.

ΤΡΟΠΟΣ Δ - ΤΟΠΙΚΑ (δοκιμη στον υπολογιστη σου)
-----------------------------------------------
Με Node εγκατεστημενο:  npm install  &&  npm start
Ανοιξε: http://localhost:3000
