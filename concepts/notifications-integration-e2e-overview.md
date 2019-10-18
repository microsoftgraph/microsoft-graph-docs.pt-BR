---
title: 'Integração das notificações com o Microsoft Graph '
description: 'As notificações são uma das maneiras mais eficazes de se envolver novamente com os usuários do seu aplicativo. Os aplicativos podem ser integrados as notificações do Microsoft Graph em algumas etapas simples.  '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: 2f3a126ade92ff1615848f9f4db846aebb62d5f7
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063227"
---
# <a name="integrate-with-microsoft-graph-notifications"></a><span data-ttu-id="a8652-104">Integração das notificações com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a8652-104">Integrate with Microsoft Graph notifications</span></span>

<span data-ttu-id="a8652-105">Os aplicativos podem ser integrados às notificações do Microsoft Graph em algumas etapas simples, como mostrado no seguinte diagrama.</span><span class="sxs-lookup"><span data-stu-id="a8652-105">You can integrate your apps with Microsoft Graph notifications with a few simple steps, as shown in the following diagram.</span></span>

![Imagem mostrando as etapas para integrar notificações: registro, integração entre dispositivos, integração com o servidor e integração com o cliente](images/notifications-integration-e2e-overview.png)

1.  <span data-ttu-id="a8652-107">[Registre](notifications-integration-app-registration.md) seu aplicativo no portal do Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="a8652-107"> Register a new application in the Azure portal</span></span>

2.  <span data-ttu-id="a8652-108">[Integre](notifications-integration-cross-device-experiences-onboarding.md) ao Partner Center/Centro de Desenvolvimento do Windows para identidade e credenciais de notificação por push multiplataforma.</span><span class="sxs-lookup"><span data-stu-id="a8652-108">[Onboard](notifications-integration-cross-device-experiences-onboarding.md) to Partner Center/Windows Dev Center for cross-platform application identity and push notification credentials.</span></span>

3.  <span data-ttu-id="a8652-109">[Configure o servidor do aplicativo](notifications-integrating-app-server.md) para enviar notificações por meio do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a8652-109">[Set up your app server](notifications-integrating-app-server.md) to send notifications via Microsoft Graph.</span></span>

4.  <span data-ttu-id="a8652-110">[Integre](notifications-integrating-with-windows.md) as [notificações SDK do cliente do Microsoft Graph](https://github.com/microsoft/project-rome) para que seus clientes do aplicativo no Windows, Android ou iOS recebam e gerenciem as notificações.</span><span class="sxs-lookup"><span data-stu-id="a8652-110">[Integrate](notifications-integrating-with-windows.md) the [Microsoft Graph notifications client SDK](https://github.com/microsoft/project-rome) into your Windows, Android, or iOS app clients to receive and manage notifications.</span></span>
