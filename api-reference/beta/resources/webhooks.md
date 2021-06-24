---
title: Usar a API do Microsoft Graph para acessar as notificações de alteração
description: Fornecer notificações de alteração aos clientes.
localization_priority: Normal
author: Jumaodhiss
doc_type: conceptualPageType
ms.prod: change-notifications
ms.openlocfilehash: 59bcc9f45b34508197494da7bc807cadbf214deb
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107750"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para acessar as notificações de alteração

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira [Configurar notificações para alterações nos dados de usuário](/graph/webhooks).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

| **Recurso** | **Trajetórias dos recursos com suporte** | **Os dados do recurso podem ser incluídos nas notificações**                  |
|:----------------|:------------|:-----------------------------------------|
| Impressão na nuvem [printer][] | Alterações quando um trabalho de impressão está pronto para ser baixado (evento JobFetchable):<br>`/print/printers/{id}/jobs` | Não |
| Impressão na nuvem [printTaskDefinition][] | Alterações quando há um trabalho válido na fila (evento JobStarted) :<br>`/print/printtaskdefinition/{id}/tasks` | Não |
| [driveItem][] no OneDrive for Business | Alterações no conteúdo da hierarquia de _qualquer pasta_:<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | Não |
| [driveItem][] no OneDrive (pessoal) | Alterações no conteúdo da hierarquia de _qualquer pasta_:<br>`/users/{id}/drive/root` | Não |
| [Grupo][] | Alterações em todos os grupos:<br>`/groups` <br>Alterações em um grupo específico:<br>`/groups/{id}`<br>Mudanças nos proprietários de um grupo específico:<br>`/groups/{id}/owners`<br>Mudanças em membros de um grupo específico:<br>`/groups/{id}/members` | Não |
| [lista][] em um [site][] do SharePoint | `/sites/{id}/lists/{id}` | Não |
| Grupo Microsoft 365 [conversação][] | Alterações nas conversas de um grupo:<br>`groups/{id}/conversations` | Não |
| [Evento][] do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário:<br>`/users/{id}/events` | Não |
| [Mensagem][] do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário: <br>`/users/{id}/messages`<br>Alterações em todas as mensagens na caixa de entrada de um usuário:<br>`/users/{id}/mailFolders('inbox')/messages` | Não |
| [Contato][] pessoal do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário:<br>`/users/{id}/contacts` | Não |
| [Alerta][] de segurança | Alterações em um alerta específico:<br>`/security/alerts/{id}` <br>Alterações em alertas filtrados:<br> `/security/alerts/?$filter`| Não |
| Teams [callRecord][] | Mudanças para _todos os_ registros de chamadas: `/communications/callRecords` | Não |
| [Canal][] do Teams | Alterações nos canais em todas as equipes:<br>`/teams/getAllChannels` <br>Alterações no canal em uma equipe específica:<br>`/teams/{id}/channels` | Sim |
| Equipes [chatmessage][] | Alterações nas mensagens de chat em todos os canais de todas as equipes:<br>`/teams/getAllMessages` <br>Alterações nas mensagens de um chat específico:<br>`/teams/{id}/channels/{id}/messages`<br>Alterações nas mensagens de todos os chats:<br>`/chats/getAllMessages` <br>Alterações nas mensagens de um chat específico:<br>`/chats/{id}/messages` | Sim |
| [conversationMember][] do Teams | Alterações na associação em uma equipe específica:<br>`/teams/{id}/members` | Sim |
| Teams [presença][] | Alterações na presença de um único usuário: `/communications/presences/{id}` <br> Alterações em várias presenças de usuário:<br> `/communications/presences?$filter=id in ({id},{id}...)` | Sim |
| Equipe do [Teams][] | Alterações em qualquer equipe no locatário:<br>`/teams` <br>Alterações em uma equipe específica:<br>`/teams/{id}` | Sim |
| [todoTask][] | Alterações em todas as tarefas em uma lista de tarefas específica:<br>`/me/todo/lists/{todoTaskListId}/tasks` | Não |
| [Usuário][] | Alterações em todos os usuários:<br>`/users` <br>Alterações em um usuário específico:<br>`/users/{id}`| Não |


> **Observação**: qualquer trajetória de recurso que comece com o `/users/{id}` também pode aceitar `/me` referenciar o usuário conectado.

## <a name="permissions"></a>Permissions

Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.

| Tipo de permissão                        | Tipos de recurso com suporte                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegado - conta corporativa ou de estudante     | [alert][], channel , contact , [conversation][], [conversationMember][], [driveItem][], [list][], [event][] [,][] [group][] [,][]message , [user][], [presence][], [chatMessage][] (preview), [team][], [todoTask][] [][] |
| Delegado - conta pessoal da Microsoft | [contact][], [driveItem][], [list][], [event][], [message][],[todoTask][]                                     |
| Aplicativo                            | [alert][], [channel][], [contact][], [driveItem][], [list][] [,][]event , [group][], [message][], [user][], [callRecord][], [chatMessage][], [conversationMember][], [printer][], [printTaskDefinition][], [team][] |

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
[conversationMember]: ./conversationmember.md
[channel]: ./channel.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[usuário]: ./user.md
[callRecord]: ./callrecords-callrecord.md
[alerta]: ./alert.md
[presence]: ./presence.md
[impressora]: ./printer.md
[printTaskDefinition]: ./printtaskdefinition.md
[team]: ./team.md
[todoTask]: ./todoTask.md

