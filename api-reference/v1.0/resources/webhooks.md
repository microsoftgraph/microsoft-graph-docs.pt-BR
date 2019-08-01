---
title: Usar a API do Microsoft Graph para acessar as notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira Configurar notificações para alterações nos dados de usuário.
localization_priority: Priority
author: piotrci
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 1722f888cc7e29e958a84720f8e714f2379db7da
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033401"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para acessar as notificações de alteração

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira [Configurar notificações para alterações nos dados de usuário](/graph/webhooks).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

- [Mensagem][] do Outlook
- [Evento][] do Outlook
- [Contato][] pessoal do Outlook
- [user][]
- [group][]
- [Conversa][] em grupo do Office 365
- Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário
- Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business
- [Alerta][] de segurança

## <a name="permissions"></a>Permissões

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
