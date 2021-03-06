---
title: "Problème d’ajout d’une application hors galerie | Microsoft Docs"
description: "Comprendre les problèmes courants auxquels les utilisateurs sont confrontés lors de l’ajout d’applications hors galerie personnalisées"
services: active-directory
documentationcenter: 
author: ajamess
manager: femila
ms.assetid: 
ms.service: active-directory
ms.workload: identity
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.date: 07/11/2017
ms.author: asteen
ms.translationtype: Human Translation
ms.sourcegitcommit: cc9e81de9bf8a3312da834502fa6ca25e2b5834a
ms.openlocfilehash: 2dd8ed2cc0cd9575dcc56f489afa19a41cc9c10a
ms.contentlocale: fr-fr
ms.lasthandoff: 04/11/2017

---

<a id="problem-adding-a-non-gallery-application" class="xliff"></a>

# Problème d’ajout d’une application hors galerie

Cet article vous aide à comprendre les problèmes courants auxquels les utilisateurs sont confrontés lors de l’ajout **d’applications hors galerie personnalisées** et ce que vous pouvez faire pour les résoudre. 

<a id="i-clicked-the-add-button-and-my-application-took-a-long-time-to-appear" class="xliff"></a>

## J’ai cliqué sur le bouton « Ajouter » et l’application a mis beaucoup de temps à s’afficher

Dans certaines conditions, 1 à 2 minutes (et parfois plus) peuvent être nécessaires pour qu’une application apparaisse après avoir été ajoutée à votre annuaire. Même si ce comportement demeure anormal, vous pouvez visualiser la progression de l’ajout de l’application en cliquant sur l’icône **Notifications** (cloche) dans le coin supérieur droit du [portail](https://portal.azure.com/) et en recherchant la notification **En cours** ou **Terminé** pour le champ **Créer une application**.

Si votre application n’est jamais ajoutée, ou si vous rencontrez une erreur lorsque vous cliquez sur le bouton **Ajouter**, vous verrez une **notification** affichant l’état **Erreur**. Si vous souhaitez obtenir plus de détails sur l’erreur afin d’en savoir plus sur ou de partager ces informations avec un ingénieur du support, vous pouvez afficher plus d’informations sur l’erreur en suivant les étapes décrites dans la section [Guide pratique pour afficher les détails d’une notification du portail](#how-to-see-the-details-of-a-portal-notification).

<a id="i-clicked-the-add-button-and-my-application-didnt-appear" class="xliff"></a>

## J’ai cliqué sur le bouton « Ajouter » et mon application n’apparaît pas

En raison de problèmes temporaires, de problèmes de réseau ou d’un bogue, l’ajout d’une application peut parfois échouer. Ce problème se manifeste lorsque vous cliquez sur l’icône **Notifications** (cloche) dans le coin supérieur droit du portail Azure et qu’une icône rouge (!) apparaît en regard de votre notification **Créer une application**. Cela indique qu’une erreur est survenue lors de la création de l’application.

Si vous rencontrez une erreur lorsque vous cliquez sur le bouton **Ajouter**, vous verrez une **notification** affichant l’état **Erreur**. Si vous souhaitez obtenir plus de détails sur l’erreur afin d’en savoir plus sur ou de partager ces informations avec un ingénieur du support, vous pouvez afficher plus d’informations sur l’erreur en suivant les étapes décrites dans la section [Guide pratique pour afficher les détails d’une notification du portail](#how-to-see-the-details-of-a-portal-notification).

<a id="i-dont-know-how-to-set-up-my-application-once-ive-added-it" class="xliff"></a>

## Je ne sais pas comment configurer mon application une fois que je l’ai ajoutée

Si vous avez besoin d’aide pour en savoir plus sur les applications personnalisées, la [bibliothèque de documents Applications Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-apps-index) vous fournit plus d’informations sur l’authentification unique avec Azure AD et son fonctionnement.

<a id="how-to-see-the-details-of-a-portal-notification" class="xliff"></a>

## Guide pratique pour afficher les détails d’une notification du portail

Vous pouvez afficher les détails de toute notification du portail en suivant les étapes ci-dessous :

1.  Cliquez sur l’icône **Notifications** (cloche) dans le coin supérieur droit du portail Azure

2.  Sélectionnez n’importe quelle notification avec l’état **Erreur**, signalée par une croix rouge (!).

   >[!NOTE]
   >Vous ne pouvez pas cliquer sur les notifications affichant l’état **Réussi** ou **En cours**.
   >
   >

3.  Le volet **Détails de notification** apparaît.

4.  Utilisez ces informations pour en savoir plus sur le problème.

5.  Si vous avez encore besoin d’aide, vous pouvez également partager ces informations avec un ingénieur du support technique ou le groupe de produits qui vous aidera à résoudre votre problème.

6.  Cliquez sur l**’icône de copie** à droite de la zone de texte **Erreur de copie** pour copier tous les détails de la notification afin de les partager avec un ingénieur du support technique ou du groupe de produits.

<a id="how-to-get-help-by-sending-notification-details-to-a-support-engineer" class="xliff"></a>

## Guide pratique pour obtenir de l’aide en envoyant les détails de la notification à un ingénieur du support technique

Il est très important que vous partagiez **tous les détails ci-dessous** avec un ingénieur du support technique si vous avez besoin d’aide car il peut vous aider à résoudre rapidement le problème. Vous pouvez facilement le faire en **prenant une capture d’écran** ou en cliquant sur l**’icône d’erreur de copie** située à droite de la zone de texte **Erreur de copie**.

<a id="notification-details-explained" class="xliff"></a>

## Explication des détails de la notification

Vous trouverez ci-dessous plus d’informations sur la signification de chaque notification ainsi que des exemples de chacune d’elles.

<a id="essential-notification-items" class="xliff"></a>

### Éléments essentiels de la notification

-   **Titre** : titre descriptif de la notification
   *  Exemple : **paramètres de proxy d’application**

-   **Description** : description de ce qui s’est produit suite à l’opération

   *  Exemple : **URL interne entrée est déjà utilisée par une autre application**

-   **ID de notification** : ID unique de la notification

   *  Exemple : **clientNotification-2adbfc06-2073-4678-a69f-7eb78d96b068**

-   **ID de la demande client** : ID de la demande spécifique faite par votre navigateur

   *  Exemple : **302fd775-3329-4670-a9f3-bea37004f0bc**

-   **Horodatage UTC** : horodatage de l’affichage de la notification, au format UTC

   *  Exemple : **2017-03-23T19:50:43.7583681Z**

-   **ID de transaction interne** : ID interne nous permettant de rechercher l’erreur dans nos systèmes

   *  Exemple : **71a2f329-ca29-402f-aa72-bc00a7aca603**

-   **UPN** : utilisateur qui a effectué l’opération

   *  Exemple : **tperkins@f128.info**

-   **ID de locataire** : ID unique du locataire dont l’utilisateur qui a effectué l’opération était membre

   *  Exemple : **7918d4b5-0442-4a97-be2d-36f9f9962ece**

-   **ID de l'objet utilisateur** : ID unique de l’utilisateur qui a effectué l’opération

 *  Exemple : **17f84be4-51f8-483a-b533-383791227a99**

<a id="detailed-notification-items" class="xliff"></a>

### Éléments détaillés de la notification

-   **Nom d’affichage** : **(peut être vide)** nom d’affichage plus détaillé de l’erreur

  *  Exemple : **paramètres de proxy d’application**

-   **État** : état spécifique de la notification

   *  Exemple : **Échec**

-   **ID de l’objet** : **(peut être vide)** ID de l’objet sur lequel l’opération a été effectuée

   *  Exemple : **8e08161d-f2fd-40ad-a34a-a9632d6bb599**

-   **Détails** : description détaillée de ce qui s’est produit suite à l’opération

   *  Exemple : **l’URL interne 'http://bing.com/' n’est pas valide car elle est déjà en cours d’utilisation**

-   **Erreur de copie** : cliquez sur l**’icône de copie** à droite de la zone de texte **Erreur de copie** pour copier tous les détails de la notification afin de les partager avec un ingénieur du support technique ou du groupe de produits

   *  Exemple ```{"errorCode":"InternalUrl\_Duplicate","localizedErrorDetails":{"errorDetail":"Internal url 'http://google.com/' is invalid since it is already in use"},"operationResults":\[{"objectId":null,"displayName":null,"status":0,"details":"Internal url 'http://bing.com/' is invalid since it is already in use"}\],"timeStampUtc":"2017-03-23T19:50:26.465743Z","clientRequestId":"302fd775-3329-4670-a9f3-bea37004f0bb","internalTransactionId":"ea5b5475-03b9-4f08-8e95-bbb11289ab65","upn":"tperkins@f128.info","tenantId":"7918d4b5-0442-4a97-be2d-36f9f9962ece","userObjectId":"17f84be4-51f8-483a-b533-383791227a99"}```

<a id="next-steps" class="xliff"></a>

## Étapes suivantes
[Gestion des applications avec Azure Active Directory](active-directory-enable-sso-scenario.md)




