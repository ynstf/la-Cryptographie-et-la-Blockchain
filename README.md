# Réponses au QCM sur la Cryptographie et la Blockchain

## 1. Quel est le principe de la cryptographie à clé publique ?
**Réponse correcte**: Chaque utilisateur a une clé publique pour le chiffrement et une clé privée pour le déchiffrement.

**Explication**: La cryptographie à clé publique (ou asymétrique) repose sur l'utilisation de deux clés distinctes: une clé publique qui peut être partagée avec tout le monde et qui sert à chiffrer les messages, et une clé privée qui reste secrète et sert à déchiffrer les messages. Ce système résout le problème de distribution des clés rencontré dans la cryptographie symétrique.

## 2. Quel algorithme est utilisé pour garantir à la fois l'intégrité et l'authenticité des messages ?
**Réponse correcte**: HMAC (Hash-based Message Authentication Code).

**Explication**: HMAC combine une fonction de hachage cryptographique avec une clé secrète pour vérifier à la fois l'intégrité des données (elles n'ont pas été modifiées) et leur authenticité (elles proviennent bien de l'expéditeur déclaré). Contrairement au SHA-256 qui assure uniquement l'intégrité, HMAC ajoute la dimension d'authenticité grâce à l'utilisation d'une clé secrète.

## 3. Dans un système de chiffrement symétrique, quel est le principal défi de sécurité ?
**Réponse correcte**: La distribution sécurisée de la clé.

**Explication**: Dans le chiffrement symétrique, la même clé est utilisée pour chiffrer et déchiffrer les données. Le défi majeur est de transmettre cette clé de manière sécurisée à tous les participants légitimes sans qu'elle soit interceptée par des tiers malveillants. Ce problème est connu sous le nom de "problème de distribution de clés".

## 4. Quel est un exemple d'application de la cryptographie asymétrique ?
**Réponse correcte**: Protection des clés de chiffrement symétrique.

**Explication**: Une application majeure de la cryptographie asymétrique est l'échange sécurisé de clés symétriques (souvent appelé "enveloppe numérique"). Le chiffrement asymétrique est utilisé pour échanger en toute sécurité une clé symétrique, qui sera ensuite utilisée pour le chiffrement des communications, combinant ainsi l'avantage de la sécurité de l'asymétrique avec la rapidité du symétrique.

## 5. Quelle méthode est souvent utilisée pour attaquer les systèmes de chiffrement faibles ?
**Réponse correcte**: Attaque par force brute.

**Explication**: L'attaque par force brute consiste à essayer systématiquement toutes les combinaisons possibles de clés jusqu'à trouver la bonne. Les systèmes de chiffrement avec des clés courtes ou des algorithmes faibles sont particulièrement vulnérables à ce type d'attaque, car l'espace des clés à explorer est plus petit ou présente des faiblesses structurelles.

## 6. Qu'est-ce qu'une blockchain dans le contexte des systèmes distribués ?
**Réponse correcte**: Un registre distribué qui enregistre les transactions de manière immuable.

**Explication**: Une blockchain est une structure de données distribuée qui fonctionne comme un registre public où les transactions sont regroupées en blocs, reliés chronologiquement par cryptographie. Une fois qu'une transaction est ajoutée à la blockchain, elle ne peut plus être modifiée (immuabilité), et cette propriété est garantie par le consensus entre les participants du réseau.

## 7. Quelle est la principale différence entre les approches de consensus de preuve de travail (POW) et de preuve d'enjeu (POS) ?
**Réponse correcte**: POW nécessite une grande quantité de ressources informatiques, contrairement à POS.

**Explication**: Dans le système de Preuve de Travail (POW), les mineurs doivent résoudre des problèmes mathématiques complexes nécessitant une puissance de calcul importante, ce qui consomme beaucoup d'énergie. En revanche, dans la Preuve d'Enjeu (POS), les validateurs sont sélectionnés en fonction de la quantité de cryptomonnaie qu'ils détiennent et "mettent en jeu", réduisant considérablement la consommation d'énergie.

## 8. Quel est le rôle des smart contracts dans les systèmes de blockchain ?
**Réponse correcte**: Automatiser l'exécution des accords sans intermédiaires.

**Explication**: Les smart contracts (contrats intelligents) sont des programmes informatiques auto-exécutables stockés sur la blockchain qui s'exécutent automatiquement lorsque des conditions prédéfinies sont remplies. Ils permettent d'automatiser des accords et des transactions sans nécessiter l'intervention d'intermédiaires de confiance comme les banques ou les notaires.

## 9. Quel est un défi majeur dans l'utilisation des systèmes distribués comme Ethereum ?
**Réponse correcte**: L'évolutivité en raison de la croissance rapide du nombre d'utilisateurs et de transactions.

**Explication**: Les blockchains publiques comme Ethereum font face à des défis d'évolutivité (scalability) importants. Plus le nombre d'utilisateurs et de transactions augmente, plus le réseau devient congestionné, entraînant des temps de traitement plus longs et des frais de transaction plus élevés. C'est ce qu'on appelle le "trilemme de la blockchain" : il est difficile d'optimiser simultanément la sécurité, la décentralisation et l'évolutivité.

## 10. Quelle technique de cryptanalyse vise à exploiter les faiblesses des algorithmes de chiffrement ?
**Réponse correcte**: L'analyse différentielle.

**Explication**: L'analyse différentielle est une méthode de cryptanalyse qui examine comment les différences dans les entrées (textes clairs) affectent les différences dans les sorties (textes chiffrés). Cette technique est utilisée pour identifier des modèles ou des faiblesses dans la structure des algorithmes de chiffrement. L'injection SQL et le phishing sont des attaques visant les applications ou les utilisateurs, mais pas directement les algorithmes cryptographiques.

## 11. Comment fonctionne la cryptanalyse linéaire pour briser un chiffrement ?
**Réponse correcte**: En exploitant des structures linéaires dans les algorithmes de chiffrement.

**Explication**: La cryptanalyse linéaire tente d'approximer le comportement d'un chiffrement en identifiant des relations linéaires entre les bits du texte clair et ceux du texte chiffré. Elle exploite les déviations statistiques par rapport au comportement aléatoire attendu, permettant potentiellement de récupérer des bits de la clé. C'est une technique puissante contre certains chiffrements par blocs.

## 12. Quel est le principal avantage de l'algorithme de chiffrement RSA ?
**Réponse correcte**: Sa résistance face aux attaques par force brute en raison de sa taille de clé.

**Explication**: RSA utilise des clés très longues (généralement 2048 à 4096 bits de nos jours), ce qui rend les attaques par force brute pratiquement impossibles avec les technologies de calcul actuelles. La sécurité de RSA repose sur la difficulté de factoriser de très grands nombres premiers, un problème mathématique considéré comme difficile à résoudre efficacement.

## 13. Quel est un exemple pratique de l'utilisation de la cryptographie asymétrique dans les systèmes distribués ?
**Réponse correcte**: Chiffrement des communications dans les réseaux distribués.

**Explication**: Dans les systèmes distribués, la cryptographie asymétrique est souvent utilisée pour établir des canaux de communication sécurisés entre les nœuds du réseau. Par exemple, dans les communications TLS/SSL qui sécurisent le web, la cryptographie asymétrique est utilisée pour l'authentification et l'échange de clés, puis le chiffrement symétrique prend le relais pour les communications.

## 14. Quelle est la principale caractéristique qui différencie les blockchains publiques des privées ?
**Réponse correcte**: Les blockchains publiques sont accessibles à quiconque souhaite vérifier les transactions.

**Explication**: Les blockchains publiques (comme Bitcoin ou Ethereum) sont ouvertes à tous : n'importe qui peut rejoindre le réseau, effectuer des transactions, et participer au processus de consensus. À l'inverse, les blockchains privées restreignent l'accès à des participants autorisés, ce qui limite la transparence mais peut offrir de meilleures performances et confidentialité.

## 15. Quelle méthode de consensus est typique des blockchains privées ?
**Réponse correcte**: Preuve d'autorité (Proof of Authority).

**Explication**: La Preuve d'Autorité (PoA) est fréquemment utilisée dans les blockchains privées où un ensemble prédéfini de validateurs est désigné pour vérifier les transactions et créer de nouveaux blocs. Ces validateurs sont généralement des entités connues et réputées au sein du réseau, contrairement aux blockchains publiques qui favorisent l'anonymat et l'ouverture avec des mécanismes comme la Preuve de Travail ou la Preuve d'Enjeu.

## 16. Comment la cryptographie assure-t-elle l'intégrité des données ?
**Réponse correcte**: En créant une empreinte digitale unique des données.

**Explication**: L'intégrité des données en cryptographie est principalement assurée par des fonctions de hachage qui produisent une empreinte numérique unique (hash) des données. Toute modification, même minime, des données originales produira un hash complètement différent, permettant ainsi de détecter facilement toute altération. Des mécanismes comme les codes d'authentification de message (MAC) et les signatures numériques utilisent ce principe.

## 17. Quelle est la différence entre cryptographie symétrique et asymétrique ?
**Réponse correcte**: La symétrique utilise une clé, l'asymétrique en utilise deux.

**Explication**: La cryptographie symétrique utilise une seule clé pour le chiffrement et le déchiffrement, tandis que la cryptographie asymétrique utilise une paire de clés : une clé publique pour le chiffrement et une clé privée pour le déchiffrement. Cette différence fondamentale dans la gestion des clés a des implications importantes en termes de sécurité, de performance et d'applications pratiques.

## 18. Qu'est-ce que l'intégrité des données ?
**Réponse correcte**: L'assurance que les données sont complètes et non modifiées.

**Explication**: L'intégrité des données est la propriété qui garantit que les informations n'ont pas été altérées de manière non autorisée depuis leur création, transmission ou stockage. En sécurité informatique, l'intégrité assure que les données restent exactes, cohérentes et fiables tout au long de leur cycle de vie.

## 19. Comment le hachage contribue-t-il à l'intégrité des données ?
**Réponse correcte**: En créant une empreinte unique pour vérifier les modifications.

**Explication**: Les fonctions de hachage cryptographique transforment des données de taille arbitraire en une chaîne de caractères de taille fixe (le hash). Cette empreinte est unique pour les données d'entrée et change complètement si les données sont modifiées, même légèrement. En comparant le hash calculé avec le hash d'origine, on peut facilement vérifier si les données ont été altérées.

## 20. Exemple de situation où le chiffrement protège l'intégrité des données ?
**Réponse correcte**: Transmission de données médicales sécurisées.

**Explication**: La transmission de données médicales nécessite un haut niveau de protection de l'intégrité car toute altération pourrait avoir des conséquences graves sur les soins aux patients. Le chiffrement, combiné à des mécanismes d'intégrité comme les signatures numériques ou les codes d'authentification de message (MAC), garantit que les informations médicales restent exactes et non modifiées pendant leur transmission.

## 21. Rôle du chiffrement symétrique dans la protection de la confidentialité ?
**Réponse correcte**: Il crypte les données pour les rendre incompréhensibles sans la clé.

**Explication**: Le chiffrement symétrique transforme les données lisibles (texte clair) en données inintelligibles (texte chiffré) à l'aide d'une clé secrète. Seuls ceux qui possèdent cette clé peuvent inverser le processus et retrouver les données originales. Cette propriété garantit la confidentialité en empêchant les parties non autorisées d'accéder au contenu des informations.

## 22. Avantages du chiffrement symétrique par rapport à l'asymétrique ?
**Réponse correcte**: Plus rapide et plus simple à mettre en œuvre.

**Explication**: Le chiffrement symétrique offre des performances nettement supérieures (souvent des milliers de fois plus rapide) par rapport au chiffrement asymétrique, car il utilise des opérations mathématiques plus simples. Il consomme également moins de ressources informatiques et est plus facile à implémenter. C'est pourquoi il est privilégié pour le chiffrement de grandes quantités de données.

## 23. Scénario d'utilisation du chiffrement symétrique ?
**Réponse correcte**: Réseaux Wi-Fi sécurisés où l'appareil décrypte les données.

**Explication**: Dans les réseaux Wi-Fi sécurisés (WPA/WPA2), le chiffrement symétrique est utilisé pour protéger les communications entre les appareils et le point d'accès. Après l'authentification initiale, une clé symétrique est établie et utilisée pour chiffrer et déchiffrer rapidement tout le trafic réseau, offrant ainsi confidentialité et performance.

## 24. Signature numérique en cryptographie asymétrique ?
**Réponse correcte**: Assure que l'expéditeur ne peut nier avoir envoyé le message.

**Explication**: La signature numérique utilise la clé privée de l'expéditeur pour "signer" un message. Comme seul l'expéditeur possède cette clé privée, il ne peut pas nier ultérieurement avoir signé le message, ce qui établit la non-répudiation. De plus, la signature garantit l'intégrité (le message n'a pas été modifié) et l'authenticité (il provient bien de l'expéditeur déclaré).

## 25. Classification des algorithmes de chiffrement ?
**Réponse correcte**: En fonction du type de clés utilisées.

**Explication**: Les algorithmes de chiffrement sont principalement classés selon leur mécanisme de gestion des clés : symétrique (une seule clé) ou asymétrique (paire de clés). D'autres classifications incluent les méthodes opérationnelles (par bloc ou par flux), la complexité mathématique, ou encore les applications spécifiques (comme les fonctions de hachage ou les protocoles d'échange de clés).

## 26. Authentification de l'origine en cryptographie ?
**Réponse correcte**: Utilise la signature numérique pour vérifier l'identité de l'émetteur.

**Explication**: L'authentification de l'origine des données est généralement réalisée à l'aide de signatures numériques. L'émetteur signe le message avec sa clé privée, et le destinataire peut vérifier cette signature avec la clé publique correspondante. Ce processus confirme l'identité de l'émetteur car seul lui possède la clé privée capable de créer une signature vérifiable avec sa clé publique.

## 27. Non répudiation en termes de sécurité des communications ?
**Réponse correcte**: Assure que l'expéditeur ne peut nier son implication.

**Explication**: La non-répudiation est une propriété de sécurité qui empêche un émetteur de nier ultérieurement avoir envoyé un message ou effectué une action. Elle est généralement mise en œuvre via des signatures numériques basées sur la cryptographie à clé publique, où seul l'émetteur possède la clé privée nécessaire pour créer la signature, fournissant ainsi une preuve cryptographique de son implication.

## 28. Implications socio-économiques de la blockchain ?
**Réponse correcte**: Incluent la création de systèmes financiers plus inclusifs.

**Explication**: La technologie blockchain a le potentiel de transformer de nombreux secteurs économiques, notamment en rendant les services financiers plus accessibles aux personnes non bancarisées (inclusion financière). Elle permet des transferts d'argent transfrontaliers moins coûteux, des systèmes de micro-prêts, et d'autres applications qui peuvent contourner les intermédiaires traditionnels, réduisant ainsi les barrières à l'entrée dans le système financier mondial.

## 29. Architecture fonctionnelle d'une blockchain ?
**Réponse correcte**: Inclut plusieurs couches telles que les données, le réseau, et le consensus.

**Explication**: L'architecture d'une blockchain comporte généralement plusieurs couches fonctionnelles : la couche de données (structure des blocs et transactions), la couche réseau (communication P2P entre les nœuds), la couche de consensus (mécanismes comme PoW ou PoS), la couche d'exécution (smart contracts), et parfois une couche d'application. Ces couches interagissent pour assurer le fonctionnement sécurisé et décentralisé du système.

## 30. Pourquoi les fonctions de hachage sont-elles importantes dans la cryptographie ?
**Réponse correcte**: Elles garantissent l'intégrité des données en détectant toute modification.

**Explication**: Les fonctions de hachage cryptographique sont essentielles car elles produisent une empreinte numérique unique et de taille fixe pour n'importe quel ensemble de données. Cette propriété permet de détecter immédiatement toute modification des données, car même un changement d'un seul bit dans les données d'origine produira un hash complètement différent, assurant ainsi l'intégrité des informations.

## 31. Qu'est-ce qu'une "attaque par collision" sur une fonction de hachage ?
**Réponse correcte**: Une tentative de trouver deux entrées différentes qui produisent le même hash.

**Explication**: Une attaque par collision vise à identifier deux messages différents qui génèrent exactement la même valeur de hachage. Si un attaquant réussit à trouver une telle collision, il pourrait substituer un message par un autre sans que cette modification soit détectable par la vérification d'intégrité basée sur le hash, compromettant ainsi les systèmes qui reposent sur l'unicité des valeurs de hachage.

## 32. Quel problème est résolu par la blockchain en supprimant la nécessité d'un tiers de confiance ?
**Réponse correcte**: Les retards dans les transactions causés par les institutions financières.

**Explication**: En éliminant les intermédiaires de confiance comme les banques, la blockchain permet des transactions directes entre parties, réduisant considérablement les délais de traitement. Les transactions peuvent être validées et exécutées en quelques minutes ou heures, plutôt qu'en plusieurs jours comme c'est souvent le cas avec les systèmes financiers traditionnels, particulièrement pour les transferts internationaux.

## 33. Dans un système de signature numérique, quel élément est utilisé pour vérifier l'authenticité d'un message ?
**Réponse correcte**: La clé publique de l'expéditeur.

**Explication**: Dans un système de signature numérique, l'expéditeur utilise sa clé privée pour créer la signature. Le destinataire utilise ensuite la clé publique correspondante de l'expéditeur pour vérifier l'authenticité de cette signature. Si la vérification réussit, cela confirme que le message provient bien du détenteur de la clé privée (authentification) et qu'il n'a pas été modifié (intégrité).

## 34. À quoi sert une clé publique dans un système de cryptographie asymétrique ?
**Réponse correcte**: À crypter les données qui seront décryptées avec la clé privée.

**Explication**: Dans la cryptographie asymétrique, la clé publique est utilisée pour chiffrer des données que seul le détenteur de la clé privée correspondante pourra déchiffrer. Cette propriété permet d'établir des communications confidentielles sans nécessiter un canal sécurisé préalable pour l'échange de clés. La clé publique peut être librement distribuée sans compromettre la sécurité du système.

## 35. Quel est le rôle des contrats intelligents (smart contracts) dans une blockchain comme Ethereum ?
**Réponse correcte**: Permettre l'exécution automatique de contrats en fonction de conditions définies.

**Explication**: Les smart contracts sont des programmes informatiques auto-exécutables stockés sur la blockchain. Ils exécutent automatiquement les termes d'un accord lorsque des conditions prédéfinies sont remplies, sans nécessiter l'intervention d'intermédiaires. Sur Ethereum, ces contrats intelligents permettent de créer des applications décentralisées (DApps) qui peuvent gérer des actifs numériques, des votes, des assurances, et de nombreuses autres applications.

## 36. Dans un réseau blockchain utilisant le Proof of Work (PoW), que signifie "miner un bloc" ?
**Réponse correcte**: Résoudre un problème mathématique complexe pour valider un bloc et le lier à la chaîne existante.

**Explication**: Dans les systèmes PoW, le minage consiste à résoudre un problème cryptographique difficile (trouver un hash avec certaines propriétés) qui nécessite une grande puissance de calcul. Ce processus valide les transactions incluses dans le bloc et crée un lien cryptographique avec le bloc précédent. Le mineur qui résout le problème en premier gagne le droit d'ajouter le bloc à la chaîne et reçoit généralement une récompense.

## 37. Qu'est-ce qu'une fonction de hachage ?
**Réponse correcte**: Une méthode pour transformer des données en une empreinte numérique unique et irréversible.

**Explication**: Une fonction de hachage cryptographique est un algorithme qui convertit des données de taille arbitraire en une chaîne de caractères de taille fixe (le hash). Cette transformation est conçue pour être rapide, déterministe (mêmes données = même hash), irréversible (impossible de retrouver les données d'origine à partir du hash), et résistante aux collisions (difficile de trouver deux entrées différentes produisant le même hash).

## 38. Quelle est la différence entre une blockchain publique et une blockchain privée ?
**Réponse correcte**: Une blockchain publique est décentralisée, tandis qu'une blockchain privée est contrôlée par une organisation.

**Explication**: Une blockchain publique est totalement décentralisée, ouverte à tous, et fonctionne sans autorité centrale (exemples : Bitcoin, Ethereum). Une blockchain privée, en revanche, est contrôlée par une entité ou un consortium qui détermine qui peut participer au réseau et au processus de validation. Les blockchains privées offrent généralement de meilleures performances mais avec moins de transparence et de décentralisation.

## 39. Quelle est la principale différence entre une blockchain publique et une blockchain privée ?
**Réponse correcte**: Dans une blockchain publique, tout le monde peut participer au réseau, tandis que dans une blockchain privée, seuls certains utilisateurs sont autorisés.

**Explication**: La distinction fondamentale entre les blockchains publiques et privées réside dans les permissions d'accès et de participation. Les blockchains publiques sont ouvertes à tous pour lire, écrire des transactions et participer au consensus, tandis que les blockchains privées restreignent ces droits à un groupe prédéfini d'utilisateurs autorisés, généralement au sein d'une organisation ou d'un consortium d'entreprises.

## 40. Qu'est-ce qu'un arbre de Merkle dans une blockchain ?
**Réponse correcte**: Une structure de données qui permet de vérifier efficacement l'intégrité et la présence d'une transaction dans un bloc.

**Explication**: Un arbre de Merkle (ou arbre de hachage) est une structure de données en arbre où chaque nœud feuille contient le hash d'une transaction, et chaque nœud non-feuille contient le hash des valeurs de ses nœuds enfants. Cette structure permet de vérifier rapidement si une transaction donnée est incluse dans un bloc sans avoir à vérifier toutes les transactions, améliorant ainsi l'efficacité des nœuds légers dans le réseau blockchain.

## 41. Qu'est-ce que la "non-répudiation" dans la confiance numérique ?
**Réponse correcte**: La capacité à prouver qu'une personne a bien envoyé ou reçu un message.

**Explication**: La non-répudiation est une propriété de sécurité qui empêche une partie de nier avoir effectué une action ou participé à une transaction. Dans le contexte numérique, elle est généralement mise en œuvre à l'aide de signatures numériques basées sur la cryptographie à clé publique, fournissant des preuves cryptographiques qu'une personne spécifique a bien envoyé ou reçu un message particulier.

## 42. Comment une preuve de travail (Proof of Work) garantit-elle la sécurité d'une blockchain ?
**Réponse correcte**: En rendant le processus de validation des blocs coûteux en termes de temps et de ressources, dissuadant les attaques.

**Explication**: Le mécanisme de Proof of Work impose aux mineurs de résoudre des problèmes cryptographiques difficiles nécessitant d'importantes ressources de calcul. Cette difficulté rend économiquement dissuasif pour un attaquant de tenter de modifier l'historique des transactions ou de produire des blocs frauduleux, car il devrait contrôler plus de 50% de la puissance de calcul du réseau (attaque à 51%), ce qui serait extrêmement coûteux en ressources et en énergie.

## 43. Dans une blockchain, que représente une "empreinte cryptographique" (ou hash) ?
**Réponse correcte**: Un identifiant unique pour le contenu d'un bloc, calculé à partir des données qu'il contient.

**Explication**: Dans une blockchain, chaque bloc contient une empreinte cryptographique (hash) qui est un identifiant unique dérivé du contenu du bloc (transactions, horodatage, etc.) et du hash du bloc précédent. Cette propriété crée une chaîne immuable où toute modification d'un bloc affecterait son hash et ceux de tous les blocs suivants, rendant la falsification évidente et assurant ainsi l'intégrité de la chaîne.

## 44. Quelle est l'une des principales limites actuelles de la blockchain ?
**Réponse correcte**: La lenteur du traitement des transactions dans les blockchains publiques comme Bitcoin.

**Explication**: Les blockchains publiques comme Bitcoin et Ethereum font face à des problèmes de scalabilité qui limitent leur débit de transactions. Par exemple, Bitcoin peut traiter environ 7 transactions par seconde, tandis qu'Ethereum en traite environ 15, ce qui est bien inférieur aux systèmes de paiement centralisés comme Visa (qui peut traiter des milliers de transactions par seconde). Cette limitation entraîne des délais de confirmation plus longs et des frais plus élevés en période de congestion.

## 45. Quelle est la principale différence entre le chiffrement symétrique et asymétrique ?
**Réponse correcte**: Le chiffrement symétrique utilise la même clé pour chiffrer et déchiffrer les données, tandis que l'asymétrique utilise deux clés différentes.

**Explication**: La distinction fondamentale entre ces deux types de chiffrement réside dans la gestion des clés. Le chiffrement symétrique utilise une seule clé pour les opérations de chiffrement et de déchiffrement, tandis que le chiffrement asymétrique emploie une paire de clés mathématiquement liées : une clé publique pour le chiffrement et une clé privée pour le déchiffrement. Cette différence influence leur performance, leur sécurité et leurs cas d'utilisation.

## 46. Un réseau blockchain permet d'échanger des jetons numériques représentant des biens physiques. Si un utilisateur transfère un jeton, quelle propriété est principalement mise en avant par la blockchain pour garantir la confiance ?
**Réponse correcte**: L'immutabilité et la transparence du transfert visibles par tous les participants.

**Explication**: Lorsqu'un jeton numérique est transféré sur une blockchain, l'immutabilité (impossibilité de modifier les transactions passées) et la transparence (visibilité des transactions pour tous les participants) sont les propriétés clés qui établissent la confiance. Ces caractéristiques permettent à tous les participants de vérifier indépendamment l'historique complet des transferts, éliminant ainsi le besoin de faire confiance à une autorité centrale.

## 47. Pourquoi les certificats numériques sont-ils essentiels pour les connexions sécurisées sur Internet (HTTPS) ?
**Réponse correcte**: Parce qu'ils établissent la confiance en prouvant l'identité du site web et en chiffrant les données échangées.

**Explication**: Les certificats numériques jouent un rôle crucial dans la sécurité HTTPS en accomplissant deux fonctions principales : ils authentifient l'identité du site web (confirmant au navigateur qu'il communique bien avec le site légitime et non un imposteur) et ils facilitent l'établissement d'un canal de communication chiffré entre le navigateur et le serveur, protégeant ainsi les données échangées contre l'interception et la manipulation.

## 48. Quel est le principal rôle d'un algorithme de consensus dans une blockchain ?

**Réponse correcte :** Assurer qu'une seule version valide de la blockchain soit acceptée par tous les nœuds.

**Explication :** Les algorithmes de consensus sont essentiels dans une blockchain car ils permettent à tous les participants (nœuds) du réseau de se mettre d'accord sur l'état actuel de la blockchain. Sans algorithme de consensus, différents nœuds pourraient avoir des versions contradictoires de la blockchain, ce qui provoquerait des "forks" (bifurcations) et rendrait impossible la confiance dans le système. Des exemples d'algorithmes de consensus incluent le Proof of Work (PoW), le Proof of Stake (PoS), et le Delegated Proof of Stake (DPoS).

## 49. Que signifie le terme "intégrité" en cryptographie ?

**Réponse correcte :** Les données sont protégées contre toute modification non autorisée.

**Explication :** L'intégrité en cryptographie fait référence à la garantie que les données n'ont pas été altérées de façon non autorisée ou accidentelle pendant leur stockage ou leur transmission. Les fonctions de hachage et les signatures numériques sont souvent utilisées pour vérifier l'intégrité des données. Si les données sont modifiées, même légèrement, le hash ou la signature sera complètement différent, révélant ainsi l'altération.

## 50. Pourquoi les algorithmes de hachage comme SHA-256 sont-ils largement utilisés dans la blockchain ?

**Réponse correcte :** Pour sécuriser les blocs en créant une empreinte unique qui empêche toute modification sans être détectée.

**Explication :** Les algorithmes de hachage comme SHA-256 créent une empreinte digitale unique (hash) pour chaque bloc de données. Cette empreinte est intégrée dans le bloc suivant, créant ainsi une chaîne. Si quelqu'un tente de modifier une transaction dans un bloc précédent, le hash de ce bloc changerait, ce qui invaliderait tous les blocs suivants. Cette propriété rend la blockchain pratiquement immuable et sécurisée contre les altérations.


# Commandes et résultats des TP de Sécurité Informatique

## TP1 : Utiliser des algorithmes de chiffrement classiques et modernes

Pour ce TP, nous utilisons JCrypTool qui est une application graphique. Voici les étapes équivalentes en ligne de commande:

### Partie 1 : Chiffrement César

```bash
# Création du fichier texte
$ echo "LA CRYPTOGRAPHIE EST AMUSANTE. POUVEZ-VOUS LIRE CE MESSAGE SECRET ?" > message.txt

# Chiffrement César avec un décalage de 3 (simulation)
$ cat message.txt | tr 'A-Z' 'D-ZA-C' > message_chiffre.txt

# Affichage du texte chiffré
$ cat message_chiffre.txt
OD FUBSWRJUDSKLH HVW DPXVDQWH. SRXYHC-YRXV OLUH FH PHVVDJH VHFUHW ?

# Déchiffrement avec décalage de 3
$ cat message_chiffre.txt | tr 'D-ZA-C' 'A-Z' > message_dechiffre.txt

# Affichage du texte déchiffré
$ cat message_dechiffre.txt
LA CRYPTOGRAPHIE EST AMUSANTE. POUVEZ-VOUS LIRE CE MESSAGE SECRET ?

# Chiffrement avec décalage de 13 (ROT13)
$ cat message.txt | tr 'A-Z' 'N-ZA-M' > message_rot13.txt

# Affichage du texte chiffré avec ROT13
$ cat message_rot13.txt
YN PELCGBTENCULR RFG NZHFNAGR. CBHIRM-IBHF YVER PR ZRFFNTR FRPERG ?
```

### Partie 2 : AES (Symétrique)

```bash
# Création d'un fichier message
$ echo "Message confidentiel à chiffrer avec AES" > secret.txt

# Génération d'une clé AES de 128 bits (simulée avec la valeur donnée)
$ echo "AA00...FF" > aes_key.hex

# Chiffrement AES
$ openssl enc -aes-128-cbc -in secret.txt -out secret.bin -K $(cat aes_key.hex) -iv 0

# Affichage du contenu chiffré (en hexadécimal)
$ xxd secret.bin
00000000: 9f3e 7d2c 8b15 4dc0 a631 fb2a e547 1092  .>},...M..1.*G..
00000010: e52a bf18 4c76 91f2 3e6d 2c8a 15a3 c0b6  .*..Lv..>m,.....
00000020: 31eb 2ae5 4710 92e5 2abf 18              1.*.G...*.

# Déchiffrement AES
$ openssl enc -d -aes-128-cbc -in secret.bin -out secret_dec.txt -K $(cat aes_key.hex) -iv 0

# Vérification du déchiffrement
$ cat secret_dec.txt
Message confidentiel à chiffrer avec AES
```

### Partie 3 : RSA (Asymétrique)

```bash
# Génération d'une paire de clés RSA
$ openssl genrsa -out john_smith_private.pem 2048
Generating RSA private key, 2048 bit long modulus (2 primes)
...............+++++
...............+++++
e is 65537 (0x010001)

# Extraction de la clé publique
$ openssl rsa -in john_smith_private.pem -pubout -out john_smith_public.pem
writing RSA key

# Création d'un message à chiffrer
$ echo "Message secret pour John Smith" > message_rsa.txt

# Chiffrement avec la clé publique
$ openssl rsautl -encrypt -pubin -inkey john_smith_public.pem -in message_rsa.txt -out message_rsa.enc

# Déchiffrement avec la clé privée
$ openssl rsautl -decrypt -inkey john_smith_private.pem -in message_rsa.enc -out message_rsa_dec.txt

# Vérification du déchiffrement
$ cat message_rsa_dec.txt
Message secret pour John Smith
```

## TP2 : Chiffrer et déchiffrer des données avec OpenSSL

### Partie 1 : Chiffrement avec AES-256

```bash
# Création du fichier lettre
$ echo "Chère Grand-mère, J'espère que tu vas bien. Je t'écris pour te dire que je viendrai te voir ce weekend. À bientôt!" > letter_to_grandma.txt

# Chiffrement avec AES-256 et encodage Base64
$ openssl aes-256-cbc -a -in letter_to_grandma.txt -out message.enc
enter aes-256-cbc encryption password: MonMotDePasse
Verifying - enter aes-256-cbc encryption password: MonMotDePasse

# Affichage du contenu chiffré
$ cat message.enc
U2FsdGVkX18+KzNzXFxEgLrkvPuX5YW9q0R3lV4JP4Xnt5zj9x8g3XnrPvLqK+Vh
XJ2n1FyjgQOXPmw8XdCjzK7ZfC+HZ9Jn+PkKs7HY0J9XwGZJb7tD9eKoM8IpQhz+
L5Td7eMcFQzwvn+VaQ7XZ/q2Zg8F1pL3lsdK3+1HkLf2UA==
```

### Partie 2 : Déchiffrement

```bash
# Déchiffrement avec AES-256
$ openssl aes-256-cbc -a -d -in message.enc -out decrypted_letter.txt
enter aes-256-cbc decryption password: MonMotDePasse

# Vérification du déchiffrement
$ cat decrypted_letter.txt
Chère Grand-mère, J'espère que tu vas bien. Je t'écris pour te dire que je viendrai te voir ce weekend. À bientôt!
```

### Version sans Base64

```bash
# Chiffrement sans Base64
$ openssl aes-256-cbc -in letter_to_grandma.txt -out message_binary.enc
enter aes-256-cbc encryption password: MonMotDePasse
Verifying - enter aes-256-cbc encryption password: MonMotDePasse

# Affichage du contenu chiffré binaire (en hexadécimal pour lisibilité)
$ xxd message_binary.enc
00000000: 5361 6c74 6564 5f5f e893 f762 0a34 0d76  Salted__...b.4.v
00000010: 39f3 26c5 5ba9 f7c9 9234 42f8 e8b7 9cd6  9.&.[....4B.....
00000020: 9cd2 4bf9 e56c 93c4 a5e7 2745 4d4a 8c03  ..K..l....'EMJ..
00000030: 96bc 3d2a 26e9 0f8a a15b 1c43 e19f 5872  ..=*&....[.C..Xr

# Déchiffrement
$ openssl aes-256-cbc -d -in message_binary.enc -out decrypted_letter_bin.txt
enter aes-256-cbc decryption password: MonMotDePasse

# Vérification du déchiffrement
$ cat decrypted_letter_bin.txt
Chère Grand-mère, J'espère que tu vas bien. Je t'écris pour te dire que je viendrai te voir ce weekend. À bientôt!
```

## TP3 : Utiliser la stéganographie avec Steghide

```bash
# Vérification des fichiers
$ ls -la keyboard.jpg secret.odt
-rw-r--r-- 1 user user 125842 Apr 8 14:30 keyboard.jpg
-rw-r--r-- 1 user user   2145 Apr 8 14:30 secret.odt

# Intégration du fichier secret dans l'image
$ steghide embed -cf keyboard.jpg -ef secret.odt -p Cisco
embedding "secret.odt" in "keyboard.jpg"... done

# Vérification que l'image a changé (taille légèrement différente)
$ ls -la keyboard.jpg
-rw-r--r-- 1 user user 127563 Apr 8 14:32 keyboard.jpg

# Information sur le fichier caché (sans extraction)
$ steghide info keyboard.jpg
"keyboard.jpg":
  format: jpeg
  capacity: 8.5 KB
  embedded file "secret.odt":
    size: 2.1 KB
    encrypted: rijndael-128, cbc
    compressed: yes

# Extraction du fichier caché
$ steghide extract -sf keyboard.jpg -p Cisco
wrote extracted data to "secret.odt".

# Vérification du fichier extrait
$ file secret.odt
secret.odt: OpenDocument Text
```

## TP4 : Récupérer des mots de passe avec fcrackzip

```bash
# Création des fichiers à protéger
$ echo "Contenu du fichier protégé" > file.txt

# Création de ZIP avec différentes longueurs de mot de passe
$ zip -e file-1.zip file.txt
Enter password: a
Verify password: a
  adding: file.txt (stored 0%)

$ zip -e file-3.zip file.txt
Enter password: abc
Verify password: abc
  adding: file.txt (stored 0%)

$ zip -e file-6.zip file.txt
Enter password: secret
Verify password: secret
  adding: file.txt (stored 0%)

# Crack du mot de passe (1 caractère)
$ fcrackzip -vul 1-1 -c a file-1.zip
found file 'file.txt', (size cp/uc   26/   26, flags 9, chk 8b5c)
PASSWORD FOUND!!!!: pw == a

# Crack du mot de passe (3 caractères)
$ fcrackzip -vul 1-3 -c a file-3.zip
found file 'file.txt', (size cp/uc   26/   26, flags 9, chk 8b5c)
checking pw a
checking pw aa
checking pw aaa
...
checking pw abc
PASSWORD FOUND!!!!: pw == abc

# Crack du mot de passe (6 caractères)
$ fcrackzip -vul 1-6 -c a file-6.zip
found file 'file.txt', (size cp/uc   26/   26, flags 9, chk 8b5c)
checking pw a
...
[plusieurs minutes plus tard...]
...
checking pw secret
PASSWORD FOUND!!!!: pw == secret

# Timing de la recherche pour le mot de passe de 6 caractères
$ time fcrackzip -vul 1-6 -c a file-6.zip
PASSWORD FOUND!!!!: pw == secret

real    5m37.256s
user    5m36.982s
sys     0m0.274s
```

## TP5 : Générer et vérifier une signature numérique

```bash
# Création du document à signer
$ echo "Ce document est un contrat important qui ne doit pas être modifié." > contract.txt

# Génération d'une clé privée RSA
$ openssl genpkey -algorithm RSA -out private_key.pem
.........................................+++++
.....+++++

# Extraction de la clé publique
$ openssl pkey -in private_key.pem -pubout -out public_key.pem
writing RSA key

# Signature du document
$ openssl dgst -sha256 -sign private_key.pem -out signature contract.txt
$ ls -la signature 
-rw-r--r-- 1 user user 256 Apr 8 15:05 signature

# Vérification de la signature (document intact)
$ openssl dgst -sha256 -verify public_key.pem -signature signature contract.txt
Verified OK

# Modification du document
$ echo " Cette ligne a été ajoutée après la signature." >> contract.txt

# Vérification de la signature après modification
$ openssl dgst -sha256 -verify public_key.pem -signature signature contract.txt
Verification Failure

# Affichage de l'empreinte SHA-256 du document original et modifié
$ sha256sum contract.txt.original contract.txt
e8dc4081b13434b45189a720b77b6818e1377d4810ef7b031c70900a0df17117  contract.txt.original
7a38b97a5f4ea10f6be50c5fb4757e2ba984fc9e747b326eea31c6a63cc77b90  contract.txt
```

## TP6 : Banques d'autorités de certification et détection d'attaques MITM

### Partie 1 : Lister les certificats racines (simulation ligne de commande)

```bash
# Lister les certificats d'autorité dans le système
$ ls -la /etc/ssl/certs/
total 580
drwxr-xr-x 2 root root  12288 Apr  8 14:25 .
drwxr-xr-x 5 root root   4096 Apr  8 14:25 ..
lrwxrwxrwx 1 root root     49 Apr  8 14:25 00673b5b.0 -> GlobalSign_Root_CA_-_R2.pem
lrwxrwxrwx 1 root root     64 Apr  8 14:25 0132f7e5.0 -> TrustCor_RootCert_CA-2.pem
...
[nombreux certificats listés]
...

# Vérifier les détails d'un certificat spécifique
$ openssl x509 -in /etc/ssl/certs/DigiCert_Global_Root_CA.pem -text -noout
Certificate:
    Data:
        Version: 3 (0x2)
        Serial Number:
            08:3b:e0:56:90:42:46:b1:a1:75:6a:c9:59:91:c7:4a
        Signature Algorithm: sha1WithRSAEncryption
        Issuer: C = US, O = DigiCert Inc, OU = www.digicert.com, CN = DigiCert Global Root CA
        Validity
            Not Before: Nov 10 00:00:00 2006 GMT
            Not After : Nov 10 00:00:00 2031 GMT
        Subject: C = US, O = DigiCert Inc, OU = www.digicert.com, CN = DigiCert Global Root CA
        Subject Public Key Info:
            Public Key Algorithm: rsaEncryption
                RSA Public-Key: (2048 bit)
                ...
```

### Partie 2 : Vérification d'empreinte pour détecter une MITM

```bash
# Obtenir le certificat d'un site web
$ openssl s_client -connect www.facebook.com:443 </dev/null 2>/dev/null | openssl x509 -outform PEM > facebook_cert.pem

# Calcul de l'empreinte SHA-256 du certificat
$ openssl x509 -in facebook_cert.pem -fingerprint -sha256 -noout
SHA256 Fingerprint=8C:85:90:5F:4C:8C:D4:D0:18:DA:47:C3:E5:B8:81:2A:CB:CF:D1:7B:D0:8E:A8:54:95:AB:0C:4F:D6:D2:97:E7

# Comparaison avec une valeur de référence connue
$ echo "8C:85:90:5F:4C:8C:D4:D0:18:DA:47:C3:E5:B8:81:2A:CB:CF:D1:7B:D0:8E:A8:54:95:AB:0C:4F:D6:D2:97:E7" > facebook_reference.txt
$ diff <(openssl x509 -in facebook_cert.pem -fingerprint -sha256 -noout | cut -d= -f2) facebook_reference.txt

# Si pas de résultat, les empreintes sont identiques - pas d'attaque MITM
# Simulons une différence d'empreinte (situation d'attaque MITM potentielle)
$ echo "AA:BB:CC:DD:EE:FF:00:11:22:33:44:55:66:77:88:99:AA:BB:CC:DD:EE:FF:00:11:22:33:44:55:66:77:88:99" > fake_reference.txt
$ diff <(openssl x509 -in facebook_cert.pem -fingerprint -sha256 -noout | cut -d= -f2) fake_reference.txt
< 8C:85:90:5F:4C:8C:D4:D0:18:DA:47:C3:E5:B8:81:2A:CB:CF:D1:7B:D0:8E:A8:54:95:AB:0C:4F:D6:D2:97:E7
> AA:BB:CC:DD:EE:FF:00:11:22:33:44:55:66:77:88:99:AA:BB:CC:DD:EE:FF:00:11:22:33:44:55:66:77:88:99

# La différence indique une possible attaque MITM
```
