---
title: Usar a API do Microsoft Graph para acessar as notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira Configurar notificações para alterações nos dados de usuário.
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: e14227ad1e64aaea6bf2cfb15f9ba76d0ffeb12b
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219647"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para acessar as notificações de alteração

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira [Configurar notificações para alterações nos dados de usuário](/graph/webhooks).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

| **Resource** | **Caminhos de recurso suportados** | **Dados de recurso podem ser incluídos em notificações**                  |
|:----------------|:------------|:-----------------------------------------|
| [Mensagem][] do Outlook | Alterações em todas as mensagens na caixa de correio de um usuário: <br>`/users/{id}/messages`<br>Alterações nas mensagens na caixa de entrada de um usuário:<br>`/users/{id}/mailFolders('inbox')/messages` | Não |
| [Evento][] do Outlook | Alterações em todos os eventos na caixa de correio de um usuário:<br>`/users/{id}/events` | Não |
| [Contato][] pessoal do Outlook | Alterações em todos os contatos pessoais da caixa de correio de um usuário:<br>`/users/{id}/contacts` | Não |
| [user][] | Alterações para todos os usuários:<br>`/users` <br>Alterações para um usuário específico:<br>`/users/{id}`| Não |
| [group][] | Alterações em todos os grupos:<br>`/groups` <br>Alterações em um grupo específico:<br>`/groups/{id}` | Não |
| [Conversa][] em grupo do Office 365 | Alterações nas conversas de um grupo:<br>`groups/{id}/conversations` | Não |
| [driveItem][] no onedrive (pessoal) | Alterações no conteúdo dentro da hierarquia de _qualquer pasta_:<br>`/users/{id}/drive/root` | Não |
| [driveItem][] no onedrive for Business | Alterações no conteúdo dentro da hierarquia da _pasta raiz_:<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | Não |
| [Alerta][] de segurança | Alterações em um alerta específico:<br>`/security/alerts/{id}` <br>Alterações nos alertas filtrados:<br> `/security/alerts/?$filter`| Não |
| Teams [chat](/graph/api/resources/subscription?view=graph-rest-beta) | Alterações em mensagens de chat em todos os canais em todas as equipes:<br>`/teams/allMessages` <br>Alterações em mensagens de chat em um canal específico:<br>`/teams/{id}/channels/{id}/messages`<br>Alterações nas mensagens de chat em todos os chats:<br>`/chats/allMessages` <br>Alterações em mensagens de chat em um chat específico:<br>`/chats/{id}/messages` | Sim |

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
