---
title: 'Integração das notificações com o Microsoft Graph '
description: 'As notificações são uma das maneiras mais eficazes de se envolver novamente com os usuários do seu aplicativo. Os aplicativos podem ser integrados as notificações do Microsoft Graph em algumas etapas simples.  '
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: 3cbeedfae4e47ac388b60d150505e247534ee68a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939569"
---
# <a name="integrate-with-microsoft-graph-notifications"></a><span data-ttu-id="e222e-104">Integração das notificações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e222e-104">Integrate with Microsoft Graph notifications</span></span>

<span data-ttu-id="e222e-105">Os aplicativos podem ser integrados às notificações do Microsoft Graph em algumas etapas simples, como mostrado no seguinte diagrama.</span><span class="sxs-lookup"><span data-stu-id="e222e-105">You can integrate your apps with Microsoft Graph notifications with a few simple steps, as shown in the following diagram.</span></span>

![Imagem mostrando as etapas para integrar notificações: registro, integração entre dispositivos, integração com o servidor e integração com o cliente](images/notifications-integration-e2e-overview.png)

1.  <span data-ttu-id="e222e-107">[Registre](notifications-integration-app-registration.md) seu aplicativo no portal do Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="e222e-107">[Register](notifications-integration-app-registration.md) your application in the Microsoft Azure portal.</span></span>

2. <span data-ttu-id="e222e-108">[Integre](notifications-integration-cross-device-experiences-onboarding.md) ao Partner Center/Centro de Desenvolvimento do Windows para identidade e credenciais de notificação por push multiplataforma para Windows, iOS e Android.</span><span class="sxs-lookup"><span data-stu-id="e222e-108">[Onboard](notifications-integration-cross-device-experiences-onboarding.md) to Partner Center/Windows Dev Center for cross-platform application identity and push notification credentials.</span></span>

3.  <span data-ttu-id="e222e-109">[Configure o servidor do aplicativo](notifications-integrating-app-server.md) para enviar notificações por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e222e-109">[Set up your app server](notifications-integrating-app-server.md) to send notifications via Microsoft Graph.</span></span>

4.  <span data-ttu-id="e222e-110">[Integre](notifications-integrating-with-windows.md) as novas [notificações SDK do cliente](https://aka.ms/GNSDK) para que seus clientes web, Windows, Android ou iOS recebam e gerenciem as notificações.</span><span class="sxs-lookup"><span data-stu-id="e222e-110">[Integrate](notifications-integrating-with-windows.md) the [Microsoft Graph notifications client SDK](https://aka.ms/GNSDK) into your Windows, Android, or iOS app clients to receive and manage notifications.</span></span>

> [!NOTE]
> <span data-ttu-id="e222e-111">Recomendamos usar o novo [SDK de notificação](https://aka.ms/GNSDK), mais simples e avançado, em vez de usar o [SDK do Project Rome](https://github.com/microsoft/project-rome).</span><span class="sxs-lookup"><span data-stu-id="e222e-111">We recommend using the new and improved, lightweight [notification SDK](https://aka.ms/GNSDK) instead of the cross-device [Project Rome SDK](https://github.com/microsoft/project-rome).</span></span>
