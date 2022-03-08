---
title: Usar a API do Microsoft Graph para acessar as notificações de alteração
description: Fornecer notificações de alteração aos clientes.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: conceptualPageType
ms.prod: change-notifications
ms.openlocfilehash: 9812aeca1d2a8a057389aaec5183b42032b64674
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335959"
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
| [Evento][] do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário:<br>`/users/{id}/events` | Sim |
| [Mensagem][] do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário: <br>`/users/{id}/messages`<br>Alterações em todas as mensagens na caixa de entrada de um usuário:<br>`/users/{id}/mailFolders('inbox')/messages` | Sim |
| [Contato][] pessoal do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário:<br>`/users/{id}/contacts` | Sim |
| [Alerta][] de segurança | Alterações em um alerta específico:<br>`/security/alerts/{id}` <br>Alterações em alertas filtrados:<br> `/security/alerts/?$filter`| Não |
| Teams [callRecord][] | Mudanças para _todos os_ registros de chamadas: `/communications/callRecords` | Não |
| [Canal][] do Teams | Alterações nos canais em todas as equipes:<br>`/teams/getAllChannels` <br>Alterações no canal em uma equipe específica:<br>`/teams/{id}/channels` | Sim |
| [Chat][] do Teams | Alterações em qualquer chat no locatário:<br>`/chats` <br>Alterações em um chat específico:<br>`/chats/{id}` | Sim |
| Equipes [chatmessage][] | Alterações nas mensagens de chat em todos os canais de todas as equipes:<br>`/teams/getAllMessages` <br>Alterações nas mensagens de um chat específico:<br>`/teams/{id}/channels/{id}/messages`<br>Alterações nas mensagens de todos os chats:<br>`/chats/getAllMessages` <br>Alterações nas mensagens de um chat específico:<br>`/chats/{id}/messages`<br>Alterações nas mensagens de chat em todos os chats de que um usuário específico faz parte:<br>`/users/{id}/chats/getAllMessages` | Sim |
| [conversationMember][] do Teams | Alterações na associação em uma equipe específica:<br>`/teams/{id}/members` <br> Alterações na associação em um chat específico:<br>`/chats/{id}/members` <br> Alterações na associação em todos os chats:<br>`/chats/getAllMembers` <br> Alterações na associação em todos os canais em uma equipe específica:<br>`teams/{id}/channels/getAllMembers` | Sim |
| Teams [presença][] | Alterações na presença de um único usuário: `/communications/presences/{id}` <br> Alterações em várias presenças de usuário:<br> `/communications/presences?$filter=id in ({id},{id}...)` | Sim |
| Equipe do [Teams][] | Alterações em qualquer equipe no locatário:<br>`/teams` <br>Alterações em uma equipe específica:<br>`/teams/{id}` | Sim |
| [baseTask][] | Alterações em todas as tarefas em uma lista de tarefas específica:<br>`/me/tasks/lists/{baseTaskListId}/tasks`<br>Alterações em todas as tarefas:<br>`/me/tasks/lists/alltasks` | Não |
| [Usuário][] | Alterações em todos os usuários:<br>`/users` <br>Alterações em um usuário específico:<br>`/users/{id}`| Não |


> **Observação**: qualquer trajetória de recurso que comece com o `/users/{id}` também pode aceitar `/me` referenciar o usuário conectado.

## <a name="permissions"></a>Permissions

Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.

| Tipo de permissão                        | Tipos de recurso com suporte                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegado - conta corporativa ou de estudante     | [alert][], [channel][], [chat][], [contact][], [conversation][], [conversationMember][], [driveItem][], [list][], [event][], [group][], [message][][, user][], [presence][], [chatMessage][] (visualização), [team][], [baseTask][] |
| Delegado - conta pessoal da Microsoft | [contact][], [driveItem][], [list][], [event][], [message][], [baseTask][]                                     |
| Aplicativo                            | [alert][], [channel][], [chat][], [contact][], [driveItem][], [list][], [][]event, [group][], [message][], [user][], [callRecord][], [chatMessage][], [conversationMember][], [printer][], [printTaskDefinition][], [team][] |

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](subscription.md)
- [Listar de assinaturas](../api/subscription-list.md)
- [Obter assinatura](../api/subscription-get.md)
- [Criar assinatura](../api/subscription-post-subscriptions.md)
- [Atualizar assinatura](../api/subscription-update.md)
- [Excluir assinatura](../api/subscription-delete.md)

[chat]: ./chat.md
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
[baseTask]: ./baseTask.md

