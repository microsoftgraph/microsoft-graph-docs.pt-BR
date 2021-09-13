---
title: 'Integração das notificações com o Microsoft Graph '
description: 'As notificações são uma das maneiras mais eficazes de se envolver novamente com os usuários do seu aplicativo. Os aplicativos podem ser integrados as notificações do Microsoft Graph em algumas etapas simples.  '
ms.localizationpriority: high
ms.prod: notifications
author: merzink
ms.openlocfilehash: 8d3e2fe8d7c208cd2c4f0c7f55ba68a79a3d3713
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59066902"
---
# <a name="integrate-with-microsoft-graph-notifications"></a>Integração das notificações com o Microsoft Graph

Os aplicativos podem ser integrados às notificações do Microsoft Graph em algumas etapas simples, como mostrado no seguinte diagrama.

![Imagem mostrando as etapas para integrar notificações: registro, integração entre dispositivos, integração com o servidor e integração com o cliente](images/notifications-integration-e2e-overview.png)

1.  [Registre](notifications-integration-app-registration.md) seu aplicativo no portal do Microsoft Azure.

2. [Integre](notifications-integration-cross-device-experiences-onboarding.md) ao Partner Center/Centro de Desenvolvimento do Windows para identidade e credenciais de notificação por push multiplataforma para Windows, iOS e Android.

3.  [Configure o servidor do aplicativo](notifications-integrating-app-server.md) para enviar notificações por meio do Microsoft Graph.

4.  [Integre](notifications-integrating-with-windows.md) as novas [notificações SDK do cliente](https://aka.ms/GNSDK) para que seus clientes web, Windows, Android ou iOS recebam e gerenciem as notificações.

> [!NOTE]
> Recomendamos usar o novo [SDK de notificação](https://aka.ms/GNSDK), mais simples e avançado, em vez de usar o [SDK do Project Rome](https://github.com/microsoft/project-rome).
