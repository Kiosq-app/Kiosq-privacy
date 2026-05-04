# Politique de confidentialité — Kiosq

**Dernière mise à jour : 4 mai 2026**

Cette politique décrit comment l'application **Kiosq** (« l'Application »,
éditée par [Gaïalabx]) gère vos données. En utilisant
Kiosq, vous acceptez les pratiques décrites ci-dessous.

Notre principe : **vos données vous appartiennent**. Kiosq fonctionne
majoritairement hors ligne, sans publicité, sans pistage, et sans envoi
de votre comportement de lecture à des tiers.

## 1. Données stockées localement sur votre appareil

L'Application stocke localement (base Hive chiffrée par Android) :

- Vos flux RSS / chaînes vidéo / podcasts configurés
- Vos catégories, sujets (mots-clés d'alerte) et favoris
- L'historique des articles téléchargés (purgé selon votre réglage,
  30 jours par défaut)
- Vos préférences d'affichage et de lecture
- Vos statistiques de lecture (articles lus, série quotidienne)
- La progression de lecture des podcasts
- Les images et contenus mis en cache pour la lecture hors ligne

Ces données ne quittent **jamais** votre appareil sauf si vous activez
explicitement la sauvegarde cloud (cf. section 2).

## 2. Sauvegarde cloud Google Drive (optionnel)

Si vous activez la sauvegarde cloud, l'Application :

- Authentifie votre compte Google via OAuth (jeton stocké uniquement sur
  votre appareil)
- Sauvegarde votre configuration (flux, catégories, sujets, paramètres)
  dans le **dossier réservé à Kiosq** de votre Google Drive personnel.
  Aucun autre dossier n'est lisible.
- Permet la restauration sur un nouvel appareil

Vos données ne transitent **jamais** par nos serveurs : la communication
est directe entre votre appareil et l'API Google Drive. Vous restez
propriétaire et contrôlez l'accès via votre compte Google.

Pour révoquer l'accès : Paramètres Kiosq → Synchronisation, ou via
[myaccount.google.com](https://myaccount.google.com/permissions).

## 3. Rapports de crash anonymes (Firebase Crashlytics)

Pour améliorer la stabilité, l'Application peut envoyer **automatiquement**
des rapports techniques en cas de plantage. Ces rapports contiennent :

- La trace technique du plantage (stack trace)
- La version de l'Application et la version d'Android
- Le modèle de votre appareil
- Votre langue système
- Un identifiant **anonyme et local** (UUID généré sur votre appareil,
  non lié à votre identité, votre compte ou votre numéro de téléphone)

**Aucune donnée personnelle, aucun contenu d'article ni aucun comportement
de lecture n'est envoyé.**

Ce service est fourni par Firebase Crashlytics (Google). Politique
Google : [policies.google.com/privacy](https://policies.google.com/privacy).

**Vous pouvez désactiver à tout moment** cette collecte dans
Paramètres → Général → Confidentialité → Rapports de crash.

## 4. Service de traduction d'articles (à la demande)

Lorsque vous tappez « Traduire » sur un article, le texte de cet article
est envoyé à l'API publique Google Translate
(`translate.googleapis.com`) pour traduction. Aucun identifiant utilisateur
n'est joint à la requête.

Cette communication n'a lieu **que** lors d'un tap explicite. Aucun
texte n'est envoyé en arrière-plan.

## 5. Affichage de pages web (WebView)

Pour la lecture en mode « Web » d'un article, l'Application charge la
page d'origine de l'article dans un composant WebView Android. Le site
distant peut alors poser ses propres cookies, ses analytics ou ses
publicités (pratiques propres à chaque éditeur). Ces cookies sont isolés
de votre navigateur principal et peuvent être effacés via les paramètres
système Android.

## 6. Achats intégrés (donations)

Si vous effectuez un don pour soutenir l'Application, la transaction est
gérée intégralement par Google Play Billing. Nous ne recevons **aucune
donnée bancaire**, uniquement la confirmation que la transaction a abouti.

## 7. Notifications

Les notifications (nouveaux articles, alertes Sujets) sont **générées
localement** par votre appareil. Elles ne nécessitent aucun serveur de
push externe. Vous pouvez les désactiver via Paramètres Kiosq ou les
réglages système Android.

## 8. Données que nous NE collectons PAS

L'Application **ne collecte ni ne transmet** :

- Votre localisation
- Vos contacts, votre agenda, vos SMS, vos photos, votre micro, votre caméra
- Votre identifiant publicitaire (Advertising ID)
- Votre historique de navigation
- Vos comportements de lecture (quels articles, à quelle heure, etc.)
- Votre carnet de favoris à des fins commerciales

Aucune publicité n'est affichée. Aucun pixel de pistage n'est intégré.

## 9. Permissions Android demandées

| Permission | Pourquoi |
|---|---|
| Accès Internet | Synchronisation des flux RSS |
| État du réseau | Détection Wi-Fi vs cellulaire (option « sync uniquement Wi-Fi ») |
| Notifications (Android 13+) | Alertes nouveaux articles |
| Service en avant-plan | Lecture audio podcasts |
| Wake lock | Maintenir la lecture audio active |
| Démarrage automatique | Reprise des tâches de synchronisation après redémarrage |
| Vibreur | Notifications |
| Achats intégrés | Donations |

## 10. Conservation des données

- Données locales : conservées tant que l'Application est installée.
  Suppression complète via la désinstallation ou Paramètres → Données →
  Réinitialiser.
- Sauvegarde cloud : conservée tant que vous le souhaitez. Suppression
  via Paramètres → Synchronisation → Supprimer la sauvegarde cloud.
- Rapports de crash : conservés 90 jours par Firebase Crashlytics, puis
  supprimés automatiquement.

## 11. Vos droits (RGPD)

Conformément au RGPD, vous disposez des droits suivants :

- **Accès** : toutes vos données sont visibles dans l'Application elle-même.
- **Rectification** : modifiez vos paramètres directement dans l'Application.
- **Suppression** : désinstallez l'Application, ou effacez la sauvegarde
  cloud, ou désactivez Crashlytics.
- **Portabilité** : exportez vos flux au format OPML via Paramètres →
  Données → Exporter.
- **Opposition** : désactivez Crashlytics (Paramètres → Confidentialité)
  ou la synchronisation cloud à tout moment.

Pour toute question relative à vos données : [kiosqrssatm@gmail.com].

## 12. Enfants

L'Application n'est pas destinée aux enfants de moins de 13 ans et ne
collecte sciemment aucune donnée d'enfant. Si vous êtes parent et pensez
que votre enfant a fourni des données, contactez-nous pour suppression.

## 13. Sécurité

Vos données locales sont stockées dans le sandbox de l'Application (zone
réservée à l'app par Android). Les communications réseau utilisent HTTPS.
La sauvegarde cloud transite directement entre votre appareil et Google
Drive, sans serveur intermédiaire.

Aucun système n'étant infaillible, nous ne pouvons garantir une sécurité
absolue, mais nous appliquons les pratiques standard du secteur.

## 14. Modifications de cette politique

Toute modification sera publiée à cette URL avec une date de mise à
jour. Pour les changements substantiels, nous afficherons une notification
dans l'Application au prochain démarrage.

## 15. Contact

[Gaïalabx]
Email : [kiosqrssatm@gmail.com]
Application : Kiosq (com.gaialabx.kiosq)