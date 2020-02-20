---
title: Usar a API do Microsoft Graph para acessar as notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira Configurar notificações para alterações nos dados de usuário.
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: a2389044671be071cf1d43dcd788519ee49d6363
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159021"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para acessar as notificações de alteração

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira [Configurar notificações para alterações nos dados de usuário](/graph/webhooks).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

| **Resource** | **Caminhos de recurso suportados** | **Dados de recurso podem ser incluídos em notificações**                  |
|:----------------|:------------|:-----------------------------------------|
| [Mensagem][] do Outlook | `/users/{id}/messages`<br>`/users/{id}/mailFolders('inbox')/messages` | Não |
| [Evento][] do Outlook | `/users/{id}/events` | Não |
| [Contato][] pessoal do Outlook | `/users/{id}/contacts` | Não |
| [user][] | `/users`(alterações em todos os usuários)<br>`/users/{id}`(alterações em um usuário específico) | Não |
| [group][] | `/groups`(alterações em todos os grupos)<br>`/groups/{id}`(alterações em um grupo específico) | Não |
| [Conversa][] em grupo do Office 365 | `groups/{id}/conversations` | Não |
| Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário | `/me/drive/root` | Não |
| Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business | `/drives/{id}/root`<br> `/me/drive/root` | Não |
| [Alerta][] de segurança | `/security/alerts/{id}`(alterações em um alerta específico) <br> `/security/alerts/?$filter`(alterações nos alertas filtrados)| Não |
| Teams [chat](/graph/api/resources/subscription?view=graph-rest-beta) | `/teams/allMessages`(mensagens em todos os canais em todas as equipes)<br>`/teams/{id}/channels/{id}/messages`(mensagens em um canal específico)<br>`/chats/allMessages`(mensagens em todos os chats)<br>`/chats/{id}/messages`(mensagens em um chat específico) | Sim |

> **Observação**: qualquer caminho de recurso que comece `/users/{id}` com também pode `/me` aceitar para fazer referência ao usuário conectado.

## <a name="permissions"></a>Permissões

Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.

| Tipo de permissão                        | Tipos de recurso com suporte                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegado - conta corporativa ou de estudante     | [alerta][], [contato][], [conversa][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][]|
| Delegado - conta pessoal da Microsoft | [contato][], [driveItem][], [evento][], [mensagem][]                                        |
| Aplicativo                            | [alerta][], [contato][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][], [chat][]|

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
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
