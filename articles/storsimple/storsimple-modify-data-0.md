---
title: "Modifier les paramètres DATA 0 sur un appareil StorSimple | Microsoft Docs"
description: "Découvrez comment utiliser Windows PowerShell for StorSimple pour reconfigurer l&quot;interface réseau DATA 0 sur votre appareil StorSimple."
services: storsimple
documentationcenter: 
author: alkohli
manager: carmonm
editor: 
ms.assetid: 58e3d509-f425-4a7f-b650-d496a7c85193
ms.service: storsimple
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 08/17/2016
ms.author: alkohli
translationtype: Human Translation
ms.sourcegitcommit: 2ea002938d69ad34aff421fa0eb753e449724a8f
ms.openlocfilehash: 3a47ff1eed220cede820e8698c3384300e94688d


---
# <a name="modify-the-data-0-network-interface-settings-on-your-storsimple-device"></a>Modification des paramètres de l’interface réseau DATA 0 sur votre périphérique StorSimple
## <a name="overview"></a>Vue d'ensemble
Votre appareil Microsoft Azure StorSimple dispose de six interfaces réseau, de DATA 0 à DATA 5. L’interface DATA 0 est toujours configurée via l'interface Windows PowerShell ou la console série, et elle est automatiquement activée pour le cloud. Vous ne pouvez pas configurer l’interface réseau DATA 0 via le portail Azure Classic. 

L’interface DATA 0 est d'abord configuré via l’Assistant Installation lors du déploiement initial de l’appareil StorSimple. Si l’appareil est en cours d’exécution, vous devrez peut-être reconfigurer les paramètres DATA 0. Ce didacticiel fournit deux méthodes permettant de modifier les paramètres de réseau DATA 0 via Windows PowerShell for StorSimple.

Après avoir lu ce didacticiel, vous pourrez :

* Modification des paramètres réseau de DATA 0 via l'Assistant Installation
* Modifier les paramètres réseau DATA 0 via l’applet de commande `Set-HcsNetInterface`

## <a name="modify-data-0-network-settings-through-setup-wizard"></a>Modification des paramètres réseau de DATA 0 via l’Assistant Installation
Vous pouvez reconfigurer les paramètres réseau de DATA 0 en vous connectant à l'interface Windows PowerShell de votre appareil StorSimple et en ouvrant une session de l'Assistant Installation. Pour modifier les paramètres de DATA 0, procédez comme suit :

#### <a name="to-modify-data-0-network-settings-through-setup-wizard"></a>Pour modifier les paramètres réseau de DATA 0 via l’Assistant Installation
1. Dans le menu de la console série, sélectionnez l’option 1, **Ouvrir une session avec un accès total**. Lorsque vous y êtes invité, fournissez le **mot de passe administrateur de l’appareil**. Le mot de passe par défaut est `Password1`.
2.  À l’invite de commandes, tapez :
   
    `Invoke-HcsSetupWizard`
3. Un Assistant Installation s’affiche pour vous aider à configurer l’interface DATA 0 de votre appareil. Indiquez les nouvelles valeurs de l'adresse IP, de la passerelle et du masque réseau.

> [!NOTE]
> Les contrôleurs d’adresses IP fixes devront être reconfigurés via la page **Configurer** de l’appareil StorSimple dans le portail Azure Classic. Pour plus d'informations, consultez la rubrique [Modification des interfaces réseau](storsimple-modify-device-config.md#modify-network-interfaces).
> 
> 

## <a name="modify-data-0-network-settings-through-set-hcsnetinterface-cmdlet"></a>Modification des paramètres réseau de DATA 0 via l’applet de commande Set-HcsNetInterface
Vous pouvez également reconfigurer l’interface réseau DATA 0 via l’applet de commande `Set-HcsNetInterface`. L’applet de commande est exécutée à partir de l’interface Windows PowerShell de votre appareil StorSimple. Lorsque vous utilisez cette procédure, les adresses IP fixes du contrôleur peuvent également être configurées. Pour modifier les paramètres de DATA 0, procédez comme suit : 

#### <a name="to-modify-data-0-network-settings-through-the-set-hcsnetinterface-cmdlet"></a>Pour modifier les paramètres réseau de DATA 0 via l’applet de commande Set-HcsNetInterface
1. Dans le menu de la console série, sélectionnez l’option 1, **Ouvrir une session avec un accès total**. Lorsque vous y êtes invité, fournissez le mot de passe administrateur de l’appareil. Le mot de passe par défaut est `Password1`.
2.  À l’invite de commandes, tapez :
   
    `Set-HCSNetInterface -InterfaceAlias Data0 -IPv4Address <> -IPv4Netmask <> -IPv4Gateway <> -Controller0IPv4Address <> -Controller1IPv4Address <> -IsiScsiEnabled 1 -IsCloudEnabled 1`
   
    Entrez, entre crochets, les valeurs suivantes de DATA 0 :
   
   * Adresse IPv4
   * Passerelle IPv4
   * Masque de sous-réseau IPv4
   * Adresse IPv4 fixe du contrôleur 0
   * Adresse IPv4 fixe du contrôleur 1
     
     Pour plus d’informations sur l’utilisation de cette applet de commande, consultez le [document de référence sur les applets de commande Windows PowerShell pour StorSimple](https://technet.microsoft.com/library/dn688161.aspx).

## <a name="next-steps"></a>Étapes suivantes
* Pour configurer les interfaces réseau autres que DATA 0, utilisez la [page Configurer du portail Azure Classic](storsimple-modify-device-config.md). 
* Si vous rencontrez des problèmes lors de la configuration de vos interfaces réseau, consultez la page [Résolution des problèmes de déploiement](storsimple-troubleshoot-deployment.md).




<!--HONumber=Nov16_HO3-->


