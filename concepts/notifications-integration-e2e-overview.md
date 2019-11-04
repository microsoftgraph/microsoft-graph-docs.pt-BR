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
# <a name="integrate-with-microsoft-graph-notifications"></a>Integração das notificações com o Microsoft Graph

Os aplicativos podem ser integrados às notificações do Microsoft Graph em algumas etapas simples, como mostrado no seguinte diagrama.

![Imagem mostrando as etapas para integrar notificações: registro, integração entre dispositivos, integração com o servidor e integração com o cliente](images/notifications-integration-e2e-overview.png)

1.  [Registre](notifications-integration-app-registration.md) seu aplicativo no portal do Microsoft Azure.

2. [Integre](notifications-integration-cross-device-experiences-onboarding.md) ao Partner Center/Centro de Desenvolvimento do Windows para identidade e credenciais de notificação por push multiplataforma para Windows, iOS e Android.

3.  [Configure o servidor do aplicativo](notifications-integrating-app-server.md) para enviar notificações por meio do Microsoft Graph.

4.  [Integre](notifications-integrating-with-windows.md) as novas [notificações SDK do cliente](https://aka.ms/GNSDK) para que seus clientes web, Windows, Android ou iOS recebam e gerenciem as notificações.

> [!NOTE]
> Recomendamos usar o novo [SDK de notificação](https://aka.ms/GNSDK), mais simples e avançado, em vez de usar o [SDK do Project Rome](https://github.com/microsoft/project-rome).
