---
title: Usar a API do Microsoft Graph para acessar as notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira Configurar notificações para alterações nos dados de usuário.
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: c8a23236d312c6e4d20a6c6018ff3a77957517e6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898293"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para acessar as notificações de alteração

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira [Configurar notificações para alterações nos dados de usuário](/graph/webhooks).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

| **Recurso** | **Trajetórias dos recursos com suporte** | **Os dados do recurso podem ser incluídos nas notificações**                  |
|:----------------|:------------|:-----------------------------------------|
| [Mensagem][] do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário: <br>`/users/{id}/messages`<br>Alterações em todas as mensagens na caixa de entrada de um usuário:<br>`/users/{id}/mailFolders('inbox')/messages` | Não |
| [Evento][] do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário:<br>`/users/{id}/events` | Não |
| [Contato][] pessoal do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário:<br>`/users/{id}/contacts` | Não |
| [Usuário][] | Alterações em todos os usuários:<br>`/users` <br>Alterações em um usuário específico:<br>`/users/{id}`| Não |
| [Grupo][] | Alterações em todos os grupos:<br>`/groups` <br>Alterações em um grupo específico:<br>`/groups/{id}`<br>Alterações nos proprietários de um grupo específico:<br>`/groups/{id}/owners`<br>Alterações nos membros de um grupo específico:<br>`/groups/{id}/members` | Não |
| [Conversa][] de grupo do Microsoft 365 | Alterações nas conversas de um grupo:<br>`groups/{id}/conversations` | Não |
| [driveItem][] no OneDrive (pessoal) | Alterações no conteúdo da hierarquia de _qualquer pasta_:<br>`/users/{id}/drive/root` | Não |
| [driveItem][] no OneDrive for Business | Alterações no conteúdo da hierarquia de _qualquer pasta_:<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | Não |
| [lista][] em um [site][] do SharePoint | `/sites/{id}/lists/{id}` | Não |
| [Alerta][] de segurança | Alterações em um alerta específico:<br>`/security/alerts/{id}` <br>Alterações em alertas filtrados:<br> `/security/alerts/?$filter`| Não |
| Teams [callRecord][] | Alterações em _todos os_ registros de chamadas:`/communications/callRecords` | Não |
| Equipes [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta) | Alterações nas mensagens de chat em todos os canais de todas as equipes:<br>`/teams/allMessages` <br>Alterações nas mensagens de um chat específico:<br>`/teams/{id}/channels/{id}/messages`<br>Alterações nas mensagens de todos os chats:<br>`/chats/allMessages` <br>Alterações nas mensagens de um chat específico:<br>`/chats/{id}/messages` | Sim |

> **Observação**: qualquer trajetória de recurso que comece com o `/users/{id}` também pode aceitar `/me` referenciar o usuário conectado.

## <a name="permissions"></a>Permissions

In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.

| Tipo de permissão                        | Tipos de recurso com suporte                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegado - conta corporativa ou de estudante     | [alerta][], [contato][], [conversa][], [driveItem][], [lista][], [evento][], [grupo][], [mensagem][], [usuário][]|
| Delegado - conta pessoal da Microsoft | [contato][], [driveItem][], [lista][], [evento][], [mensagem][]                                        |
| Aplicativo                            | [alerta][], [contato][], [driveItem][], [lista][], [evento][], [grupo][], [mensagem][], [usuário][], [callRecord][], [chat][]|

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](subscription.md)
- [Listar de assinaturas](../api/subscription-list.md)
- [Obter assinatura](../api/subscription-get.md)
- [Criar assinatura](../api/subscription-post-subscriptions.md)
- [Atualizar assinatura](../api/subscription-update.md)
- [Excluir assinatura](../api/subscription-delete.md)

[chatMessage]: ./chatmessage.md
[contato]: ./contact.md
[conversa]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[callRecord]: ./callrecords-callrecord.md
[alert]: ./alert.md
