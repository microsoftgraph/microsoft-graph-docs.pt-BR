---
title: Usar a API do Microsoft Graph para obter notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Os aplicativos cliente usam notificações para atualizar seu estado nas alterações. Para obter mais detalhes, incluindo como inscrever-se e lidar com notificações de entrada, confira set up Notifications for Changes in User Data.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 1d7a3d868ffc640f7659623942ac102575fb94fc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151489"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para obter notificações de alteração

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Os aplicativos cliente usam notificações para atualizar seu estado nas alterações. Para obter mais detalhes, incluindo como inscrever-se e lidar com notificações de entrada, confira [set up Notifications for Changes in User Data](/graph/webhooks).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

- [Mensagem][] do Outlook
- [Evento][] do Outlook
- [Contato][] pessoal do Outlook
- [usuário][]
- [group][]
- [Conversa][] em grupo do Office 365
- Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário
- Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business
- [Alerta][] de segurança

## <a name="permissions"></a>Permissões

Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.

| Tipo de permissão                        | Tipos de recurso suportados                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegado - conta corporativa ou de estudante     | [alerta][], [contato][], [conversa][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][]|
| Delegado - conta pessoal da Microsoft | [contato][], [driveItem][], [evento][], [mensagem][]                                        |
| Aplicativo                            | [alerta][], [contato][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][]|

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](subscription.md)
- [Listar assinaturas](../api/subscription-list.md)
- [Obter assinatura](../api/subscription-get.md)
- [Criar assinatura](../api/subscription-post-subscriptions.md)
- [Atualizar assinatura](../api/subscription-update.md)
- [Excluir assinatura](../api/subscription-delete.md)

[contato]: ./contact.md
[conversa]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
