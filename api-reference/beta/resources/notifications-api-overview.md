---
title: Usar as API REST de notificações no Microsoft Graph
description: Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. Basta informar uma conta de usuário à qual enviar uma notificação e a plataforma entregará a notificação a todos os pontos de extremidade do dispositivo. As solicitações de API de notificações são executadas em nome de um usuário por meio de permissões delegadas e a [permissão de notificação]( /graph/permissions_reference), que pode ser usado com contas Microsoft ou contas corporativas ou de estudante.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 2a4c23955e348159d2e17514d6041260f13cffba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458786"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Usar as API REST de notificações no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. Basta informar uma conta de usuário à qual enviar uma notificação e a plataforma entregará a notificação a todos os pontos de extremidade do dispositivo. As solicitações de API de notificações são executadas em nome de um usuário por meio de [permissões delegadas](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) e da [permissão de notificação]( /graph/permissions_reference), que podem ser usadas com contas Microsoft ou contas corporativas ou de estudante.
Esse tipo de notificação no centro de usuário é representado pelo recurso [notification](../resources/projectrome-notification.md) e armazenado no Microsoft Graph. Ele pode ser acessado e gerenciado pelo aplicativo de publicação por meio das [APIs de SDK do Projeto Rome ](https://github.com/Microsoft/project-rome). 

## <a name="next-steps"></a>Próximas etapas
- Confira o [recurso notification](../resources/projectrome-notification.md) e crie notificações para interagir com os usuários. 
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/notifications-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
