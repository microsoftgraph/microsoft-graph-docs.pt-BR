---
title: Usar a API do Microsoft Graph para acessar as notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira Configurar notificações para alterações nos dados de usuário.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: d8f8c8450f568917e5211048c164e02ad503e869
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108190"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para acessar as notificações de alteração

Namespace: microsoft.graph

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira [Configurar notificações para alterações nos dados de usuário](/graph/webhooks).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

| **Recurso** | **Trajetórias dos recursos com suporte** | **Os dados do recurso podem ser incluídos nas notificações**                  |
|:----------------|:------------|:-----------------------------------------|
| [Mensagem][] do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário: <br>`/users/{id}/messages`<br>Alterações em todas as mensagens na caixa de entrada de um usuário:<br>`/users/{id}/mailFolders('inbox')/messages` | Não |
| [Evento][] do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário:<br>`/users/{id}/events` | Não |
| [Contato][] pessoal do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário:<br>`/users/{id}/contacts` | Não |
| [Usuário][] | Alterações em todos os usuários:<br>`/users` <br>Alterações em um usuário específico:<br>`/users/{id}`| Não |
| [Grupo][] | Alterações em todos os grupos:<br>`/groups` <br>Alterações em um grupo específico:<br>`/groups/{id}` | Não |
| [Conversa][] em grupo do Office 365 | Alterações nas conversas de um grupo:<br>`groups/{id}/conversations` | Não |
| [driveItem][] no OneDrive (pessoal) | Alterações no conteúdo da hierarquia de _qualquer pasta_:<br>`/users/{id}/drive/root` | Não |
| [driveItem][] no OneDrive for Business | Alterações no conteúdo da hierarquia de _qualquer pasta_:<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | Não |
| [lista][] em um [site][] do SharePoint | Alterações no conteúdo da _lista_: <br>`/sites/{id}/lists/{id}` | Não |
| [Alerta][] de segurança | Alterações em um alerta específico:<br>`/security/alerts/{id}` <br>Alterações em alertas filtrados:<br> `/security/alerts/?$filter`| Não |
| Equipes [chatmessage](/graph/api/resources/subscription?view=graph-rest-v1.0) | Alterações nas mensagens de chat em todos os canais de todas as equipes:<br>`/teams/allMessages` <br>Alterações nas mensagens de um chat específico:<br>`/teams/{id}/channels/{id}/messages`<br>Alterações nas mensagens de todos os chats:<br>`/chats/allMessages` <br>Alterações nas mensagens de um chat específico:<br>`/chats/{id}/messages` | Sim |

> **Observação**: qualquer trajetória de recurso que comece com o `/users/{id}` também pode aceitar `/me` referenciar o usuário conectado.

## <a name="permissions"></a>Permissions

Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.

| Tipo de permissão                        | Tipos de recurso com suporte                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegado - conta corporativa ou de estudante     | [alerta][], [contato][], [conversa][], [driveItem][], [lista][], [evento][], [grupo][], [mensagem][], [usuário][]|
| Delegado - conta pessoal da Microsoft | [contato][], [driveItem][], [lista][], [evento][], [mensagem][]                                        |
| Aplicativo                            | [alerta][], [contato][], [lista][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][]|


## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](./subscription.md)
- [Listar de assinaturas](../api/subscription-list.md)
- [Obter assinatura](../api/subscription-get.md)
- [Criar assinatura](../api/subscription-post-subscriptions.md)
- [Atualizar assinatura](../api/subscription-update.md)
- [Excluir assinatura](../api/subscription-delete.md)

[contato]: ./contact.md
[conversa]: ./conversation.md
[driveItem]: ./driveitem.md
[list]: ./list.md
[site]: ./site.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
