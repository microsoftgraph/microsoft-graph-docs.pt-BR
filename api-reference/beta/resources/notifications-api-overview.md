---
title: Usar as API REST de notificações no Microsoft Graph
description: Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. Basta informar uma conta de usuário à qual enviar uma notificação e a plataforma entregará a notificação a todos os pontos de extremidade do dispositivo. As solicitações de API de notificações são executadas em nome de um usuário por meio de permissões delegadas e a [permissão de notificação]( /graph/permissions_reference), que pode ser usado com contas Microsoft ou contas corporativas ou de estudante.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 28aa795b1df9b2f4817c69332dd8bc9bf3afb172
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422518"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Usar as API REST de notificações no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. Basta informar uma conta de usuário à qual enviar uma notificação e a plataforma entregará a notificação a todos os pontos de extremidade do dispositivo. As solicitações de API de notificações são executadas em nome de um usuário por meio de [permissões delegadas](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) e da [permissão de notificação]( /graph/permissions_reference), que podem ser usadas com contas Microsoft ou contas corporativas ou de estudante.
Esse tipo de notificação no centro de usuário é representado pelo recurso [notification](../resources/projectrome-notification.md) e armazenado no Microsoft Graph. Ele pode ser acessado e gerenciado pelo aplicativo de publicação, por meio das [APIs do SDK do lado do cliente](https://github.com/Microsoft/project-rome). 

## <a name="next-steps"></a>Próximas etapas
- Confira o [recurso notification](../resources/projectrome-notification.md) e crie notificações para interagir com os usuários. 
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Comece com a integração com o cliente, seguindo as etapas descritas na [visão geral da integração](/graph/notifications-integration-e2e-overview).
