---
title: Usar a API do Microsoft Graph para acessar as notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira Configurar notificações para alterações nos dados de usuário.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: aadd1cb451a5da1c8d546ce140bd8129ca9c2bf8
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162509"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para acessar as notificações de alteração

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira [Configurar notificações para alterações nos dados de usuário](/graph/webhooks).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

| **Recurso** | **Trajetórias dos recursos com suporte** | **Os dados do recurso podem ser incluídos nas notificações**                  |
|:----------------|:------------|:-----------------------------------------|
| [Mensagem][] do Outlook | `/users/{id}/messages`<br>`/users/{id}/mailFolders('inbox')/messages` | Não |
| [Evento][] do Outlook | `/users/{id}/events` | Não |
| [Contato][] pessoal do Outlook | `/users/{id}/contacts` | Não |
| [Usuário][] | `/users` (alterações a todos os usuários)<br>`/users/{id}` ( um usuário específico) | Não |
| [Grupo][] | `/groups` (alterações a todos os grupos)<br>`/groups/{id}` (a um grupo específico) | Não |
| [Conversa][] em grupo do Office 365 | `groups/{id}/conversations` | Não |
| Conteúdo dentro da hierarquia de _qualquer pasta_ [driveItem][] no OneDrive pessoal do usuário | `/me/drive/root` | Não |
| Conteúdo dentro da hierarquia da _pasta raiz_[driveItem][] no OneDrive for Business | `/drives/{id}/root`<br> `/me/drive/root` | Não |
| [Alerta][] de segurança | `/security/alerts/{id}` (a um alerta específico) <br> `/security/alerts/?$filter` (alterações em alertas filtrados) | Não |
| Equipes [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta) | `/teams/allMessages` (mensagens em todos os canais de todas as equipes)<br>`/teams/{id}/channels/{id}/messages` (mensagens em um chat específico)<br>`/chats/allMessages` (mensagens em todos os chats)<br>`/chats/{id}/messages` (mensagens em um chat específico) | Sim |

> **Observação**: qualquer trajetória de recurso que comece com o `/users/{id}` também pode aceitar `/me` referenciar o usuário conectado.

## <a name="permissions"></a>Permissions

Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.

| Tipo de permissão                        | Tipos de recurso com suporte                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegado - conta corporativa ou de estudante     | [alerta][], [contato][], [conversa][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][]|
| Delegado - conta pessoal da Microsoft | [contato][], [driveItem][], [evento][], [mensagem][]                                        |
| Aplicativo                            | [alerta][], [contato][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][]|


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
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
