---
title: "Azure Active Directory Domain Services : mettre à jour les paramètres DNS pour le réseau virtuel Azure | Microsoft Docs"
description: Prise en main des services de domaine Azure Active Directory
services: active-directory-ds
documentationcenter: 
author: mahesh-unnikrishnan
manager: stevenpo
editor: curtand
ms.assetid: d4f3e82c-6807-4690-b298-4eabad2b7927
ms.service: active-directory-ds
ms.workload: identity
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: get-started-article
ms.date: 06/27/2017
ms.author: maheshu
ms.translationtype: Human Translation
ms.sourcegitcommit: 1500c02fa1e6876b47e3896c40c7f3356f8f1eed
ms.openlocfilehash: c704ee189072ce8ed196d1ef0a23edd528a10025
ms.contentlocale: fr-fr
ms.lasthandoff: 06/30/2017


---
<a id="enable-azure-active-directory-domain-services-preview" class="xliff"></a>

# Activer Azure Active Directory Domain Services (préversion)

<a id="task-4-update-dns-settings-for-the-azure-virtual-network" class="xliff"></a>

## Tâche 4 : Mettre à jour les paramètres DNS pour le réseau virtuel Azure
Dans les tâches de configuration précédentes, vous avez activé Azure Active Directory Domain Services pour votre répertoire. La tâche suivante consiste à s’assurer que les ordinateurs du réseau virtuel peuvent se connecter et utiliser ces services. Dans cet article, vous mettez à jour les paramètres de serveur DNS de votre réseau virtuel afin qu’il pointe vers les deux adresses IP pour lesquelles Azure Active Directory Domain Services est disponible sur le réseau virtuel.

Afin de mettre à jour le paramètre de serveur DNS pour le réseau virtuel sur lequel vous avez activé Azure Active Directory Domain Services, procédez comme suit :

1. L’onglet **Vue d’ensemble** répertorie un ensemble d’**étapes de configuration requises** à effectuer une fois que votre domaine managé est entièrement configuré. La première étape de configuration est **Mettre à jour les paramètres du serveur de noms de domaine pour votre réseau virtuel**.

    ![Domain Services - Onglet Vue d’ensemble une fois la configuration terminée](./media/getting-started/domain-services-provisioned-overview.png)

2. Lorsque votre domaine est entièrement configuré, deux adresses IP s’affichent dans cette vignette. Chacune de ces adresses IP représente un contrôleur de domaine pour votre domaine managé.

3. Pour copier la première adresse IP dans le Presse-papiers, cliquez sur le bouton Copier situé en regard. Cliquez ensuite sur le bouton **Configurer des serveurs DNS**.

4. Collez la première adresse IP dans la zone de texte **Ajouter un serveur DNS** du panneau **Serveurs DNS**. Faites défiler l’écran vers la gauche pour copier la seconde adresse IP et collez-la dans la zone de texte **Ajouter un serveur DNS**.

    ![Domain Services - Mettre à jour le DNS](./media/getting-started/domain-services-update-dns.png)

5. Cliquez sur **Enregistrer** lorsque vous avez fini de mettre à jour les serveurs DNS pour le réseau virtuel.

> [!NOTE]
> Les machines virtuelles du réseau n’obtiendront les nouveaux paramètres DNS qu’après un redémarrage. Si vous avez besoin qu’elles obtiennent les paramètres DNS mis à jour immédiatement, déclenchez un redémarrage via le portail, PowerShell ou l’interface CLI.
>
>

<a id="next-step" class="xliff"></a>

## Étape suivante
[Tâche 5 : Activer la synchronisation du mot de passe pour Azure Active Directory Domain Services](active-directory-ds-getting-started-password-sync.md)

