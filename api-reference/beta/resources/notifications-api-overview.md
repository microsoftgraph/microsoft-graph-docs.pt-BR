---
title: Usar as API REST de notificações no Microsoft Graph
description: Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. Basta informar uma conta de usuário à qual enviar uma notificação e a plataforma entregará a notificação a todos os pontos de extremidade do dispositivo. As solicitações de API de notificações são executadas em nome de um usuário por meio de permissões delegadas e a [permissão de notificação]( /graph/permissions_reference), que pode ser usado com contas Microsoft ou contas corporativas ou de estudante.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 243f412162ed1427c766272d02d58c57ba47cf42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342097"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Usar as API REST de notificações no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. Basta informar uma conta de usuário à qual enviar uma notificação e a plataforma entregará a notificação a todos os pontos de extremidade do dispositivo. As solicitações de API de notificações são executadas em nome de um usuário por meio de [permissões delegadas](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) e da [permissão de notificação]( /graph/permissions_reference), que podem ser usadas com contas Microsoft ou contas corporativas ou de estudante.
Esse tipo de notificação no centro de usuário é representado pelo recurso [notification](../resources/projectrome-notification.md) e armazenado no Microsoft Graph. Ele pode ser acessado e gerenciado pelo aplicativo de publicação por meio das [APIs de SDK do Projeto Rome ](https://github.com/Microsoft/project-rome). 

## <a name="next-steps"></a>Próximas etapas
- Confira o [recurso notification](../resources/projectrome-notification.md) e crie notificações para interagir com os usuários. 
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
