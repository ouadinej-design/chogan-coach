════════════════════════════════════════════════════
 COACH OBJECTIONS CHOGAN — GUIDE D'INSTALLATION
════════════════════════════════════════════════════

ÉTAPE 1 — Créez votre compte EmailJS GRATUIT
─────────────────────────────────────────────
1. Allez sur https://www.emailjs.com
2. Créez un compte gratuit (200 emails/mois inclus)
3. Connectez votre Gmail :
   → Email Services > Add New Service > Gmail
   → Notez votre SERVICE ID (ex: service_abc123)
4. Créez un template email :
   → Email Templates > Create New Template
   → Collez ce contenu dans le template :

   Sujet : 🔔 Nouvelle demande d'accès - Coach Chogan

   Corps :
   Bonjour,

   Nouvelle demande d'accès à l'application Coach Objections.

   👤 Nom : {{from_name}}
   📧 Email : {{from_email}}

   ✅ CODE À LUI ENVOYER : {{access_code}}

   Envoyez ce code à l'utilisatrice si vous l'autorisez.

   → Cliquez Save > notez votre TEMPLATE ID (ex: template_xyz789)
5. Récupérez votre PUBLIC KEY :
   → Account > General > Public Key

─────────────────────────────────────────────
ÉTAPE 2 — Modifiez le fichier index.html
─────────────────────────────────────────────
Ouvrez index.html avec un éditeur de texte (Bloc-notes, TextEdit).
Trouvez la section "CONFIGURATION ADMIN" et remplacez :

  ACCESS_CODE   : "CHOGAN2025"       → Votre code secret (ex: "ROSE2025")
  ADMIN_EMAIL   : "admin@email.com"  → Votre email
  EMAILJS_PK    : "VOTRE_PUBLIC_KEY" → Votre Public Key EmailJS
  EMAILJS_SVC   : "VOTRE_SERVICE_ID" → Votre Service ID EmailJS
  EMAILJS_TPL   : "VOTRE_TEMPLATE_ID"→ Votre Template ID EmailJS

Sauvegardez le fichier.

─────────────────────────────────────────────
ÉTAPE 3 — Publiez sur Netlify (GRATUIT, 2min)
─────────────────────────────────────────────
1. Allez sur https://app.netlify.com/drop
2. Glissez-déposez le DOSSIER complet (les 5 fichiers)
3. Netlify génère une URL sécurisée en 10 secondes
   (exemple : https://chogan-coach-abc123.netlify.app)
4. ✅ Votre application est en ligne !

─────────────────────────────────────────────
ÉTAPE 4 — Installer sur l'écran d'accueil
─────────────────────────────────────────────
Sur Android (Chrome) :
  → Ouvrez l'URL dans Chrome
  → Menu ⋮ > "Ajouter à l'écran d'accueil"

Sur iPhone (Safari) :
  → Ouvrez l'URL dans Safari
  → Bouton Partager 🔗 > "Sur l'écran d'accueil"

─────────────────────────────────────────────
ÉTAPE 5 — Autoriser une consultante
─────────────────────────────────────────────
1. La consultante installe l'app et remplit le formulaire
2. Vous recevez un email avec son nom + email
3. Si vous l'autorisez → envoyez-lui le CODE par WhatsApp/SMS
4. Elle entre le code → l'app se déverrouille !

Pour révoquer l'accès :
  → Changez le ACCESS_CODE dans index.html
  → Re-uploadez sur Netlify Drop
  → Communiquez le nouveau code uniquement aux autorisées

════════════════════════════════════════════════════
 Questions ? Contactez votre développeur.
════════════════════════════════════════════════════
