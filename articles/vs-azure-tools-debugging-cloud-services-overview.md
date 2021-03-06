---
title: "Options de débogage des services cloud Azure | Microsoft Docs"
description: "Débogage des services cloud Azure"
services: visual-studio-online
documentationcenter: n/a
author: kraigb
manager: ghogen
editor: 
ms.assetid: 80755da7-8350-4f5c-97ce-2962beabb36d
ms.service: visual-studio-online
ms.devlang: multiple
ms.topic: article
ms.tgt_pltfrm: multiple
ms.workload: na
ms.date: 03/18/2017
ms.author: kraigb
ms.translationtype: Human Translation
ms.sourcegitcommit: 424d8654a047a28ef6e32b73952cf98d28547f4f
ms.openlocfilehash: e79aa1db6c89ad1e382c7a70017f868fe186aa74
ms.contentlocale: fr-fr
ms.lasthandoff: 03/22/2017

---
# <a name="learn-the-various-ways-to-debug-an-azure-cloud-service"></a>Découvrez différentes méthodes de débogage d’un service cloud Azure.
Cet article fournit des liens menant vers différentes méthodes de débogage d’un service cloud Azure. 

## <a name="debugging-an-azure-cloud-service-in-visual-studio"></a>Débogage d’un service cloud Azure dans Visual Studio
L’utilisation de l’émulateur de calcul Azure pour déboguer votre service cloud sur une machine locale constitue un gain de temps et d’argent. Déboguer un service localement avant de le déployer vous permet d’améliorer la fiabilité et les performances, tout en évitant les coûts de temps de calcul. Certaines erreurs peuvent toutefois se produire quand vous exécutez un service cloud directement dans Azure. Vous pouvez déboguer les erreurs qui surviennent seulement lorsque vous exécutez un service cloud dans Azure en activant le débogage à distance lors de la publication de votre service, puis en associant le débogueur à une instance de rôle. Pour plus d’informations, consultez [Déboguer votre service cloud sur votre ordinateur local](vs-azure-tools-debug-cloud-services-virtual-machines.md#debug-your-cloud-service-on-your-local-computer).

## <a name="using-azure-diagnostics"></a>Utilisation des diagnostics Azure 
Vous pouvez utiliser les diagnostics Azure pour consigner des informations détaillées à partir du code en cours d’exécution dans des rôles, que ces derniers s’exécutent dans l’environnement de développement ou dans Azure. Pour plus d’informations, consultez la page [Activation des diagnostics Azure dans Azure Cloud Services](http://go.microsoft.com/fwlink/p/?LinkId=400450).

## <a name="using-intellitrace"></a>Utilisation d’IntelliTrace 
Si vous utilisez Visual Studio Enterprise pour écrire des rôles ciblés sur .NET Framework 4.5, vous pouvez activer IntelliTrace au moment où vous déployez un service cloud Azure depuis Visual Studio. IntelliTrace fournit un journal que vous pouvez utiliser avec Visual Studio pour déboguer votre application comme si elle s’exécutait dans Azure. Pour plus d’informations, consultez [Débogage d’un service cloud publié avec IntelliTrace et Visual Studio](http://go.microsoft.com/fwlink/p/?LinkId=623016).

## <a name="remote-debugging"></a>Débogage à distance 
Vous pouvez activer le débogage distant sur vos services cloud au moment où vous les déployez depuis Visual Studio. Si vous choisissez d’activer le débogage distant pour un déploiement, les services de débogage distant sont installés sur les machines virtuelles qui exécutent chaque instance de rôle. Ces services, tels que `msvsmon.exe`, n’affectent pas les performances et n’entraînent pas de coûts supplémentaires. Pour plus d’informations, consultez [Déboguer un service cloud dans Azure](vs-azure-tools-debug-cloud-services-virtual-machines.md#debug-a-cloud-service-in-azure).

## <a name="next-steps"></a>Étapes suivantes
- [Débogage d’un service cloud ou d’une machine virtuelle Azure dans Visual Studio](./vs-azure-tools-debug-cloud-services-virtual-machines.md) : découvrez en détail la méthode de débogage de services cloud Azure.
