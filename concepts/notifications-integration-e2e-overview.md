---
title: 'Integração das notificações com o Microsoft Graph '
description: 'As notificações são uma das maneiras mais eficazes de se envolver novamente com os usuários do seu aplicativo. Os aplicativos podem ser integrados as notificações do Microsoft Graph em algumas etapas simples.  '
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: 8dc5ef886106ca4d966e0a94ae2915040cfb5d1f1ea66d041d136db5bb7951e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149524"
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
