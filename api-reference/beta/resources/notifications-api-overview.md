---
title: Usar a API REST de notificações no Microsoft Graph (preterido)
description: Você pode usar a API de notificações do Microsoft Graph para enviar notificações por push para um usuário. .
ms.localizationpriority: high
ms.prod: notifications
doc_type: conceptualPageType
author: merzink
ms.openlocfilehash: 2c235bfa383238897efa5d55f58f4a97865e3e56
ms.sourcegitcommit: 7a0f9f1a535795c6f77c80e02fd97581c36f1273
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/27/2021
ms.locfileid: "61609029"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph-deprecated"></a>Usar a API REST de notificações no Microsoft Graph (preterido)

> [!IMPORTANT]
> A API de notificações do Microsoft Graph está preterida e deixará de retornar dados no final de janeiro de 2022. Para uma experiência de notificação alternativa, confira os [Hubs de Notificações do Microsoft Azure](/azure/notification-hubs) e [veja esta postagem no blog](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/) para obter mais informações.  

Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. Basta publicar uma notificação para o usuário de destino e a plataforma entregará a notificação a todos os pontos de extremidade de dispositivos registrados para aquele usuário. O fluxo de alto nível ocorre da seguinte forma:

1. O usuário entra no aplicativo, o que cria uma assinatura com o serviço de notificação do Microsoft Graph. Uma ID de assinatura de notificação de usuário específica ou UNSID é retornada para o aplicativo de chamada.
2. O aplicativo envia essa UNSID para o serviço do aplicativo.
3. Quando a notificação estiver pronta para envio, o serviço de aplicativo a [autenticará em uma plataforma de identidade da Microsoft](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) e a publicará por meio do serviço de notificação do Microsoft Graph, fornecendo o token de autenticação, a UNSID do usuário de destino e o conteúdo da notificação.
4. O serviço de notificação do Microsoft Graph distribui as notificações para todos os pontos de extremidade do usuário que tenham uma assinatura ativa.

Esse tipo de notificação centrada no usuário é representado pelo recurso [notificação](../resources/projectrome-notification.md) e armazenado no serviço de notificação do Microsoft Graph. Pode ser acessado e gerenciado pelo aplicativo do cliente por meio das [APIs do SDK do lado do cliente](https://aka.ms/GNSDK). Se você não conhece o serviço de notificação do Microsoft Graph, confira a seção [visão geral da notificação](/graph/notifications-concept-overview) para saber mais.

## <a name="next-steps"></a>Próximas etapas

- Confira o [recurso notification](../resources/projectrome-notification.md) e crie notificações para interagir com os usuários.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Comece com a integração com o cliente seguindo as etapas descritas no tópico [visão geral da integração](/graph/notifications-integration-e2e-overview).