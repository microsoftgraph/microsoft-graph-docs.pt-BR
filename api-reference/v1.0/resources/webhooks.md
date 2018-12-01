---
title: Usar a API do Microsoft Graph para obter notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após as alterações. Para obter mais detalhes, incluindo como se inscrever e manipular notificações de entrada, consulte Set up notificações de alterações nos dados do usuário.
ms.openlocfilehash: c7d468b7c5064911d27d3a93bc3160d03c2a4dc3
ms.sourcegitcommit: 02ead22efd4f10cd50f89c9f5aa3b6dfda96aeec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2018
ms.locfileid: "27123942"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Usar a API do Microsoft Graph para obter notificações de alteração

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após as alterações. Para obter mais detalhes, incluindo como assinar e manipular notificações de entrada, consulte [Configurar notificações para que as alterações nos dados do usuário](/graph/webhooks).

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

- Mensagens
- Eventos
- Contatos
- Usuários
- Grupos
- Conversas em grupo
- Conteúdo compartilhado na OneDrive, incluindo as unidades associadas a sites do SharePoint
- Pastas de OneDrive pessoais dos usuários
- Alertas de segurança

## <a name="permissions"></a>Permissions

Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.

| Tipo de permissão                        | Tipos de recursos com suporte                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegado - conta corporativa ou de estudante     | [entre em contato][], [conversa][], [unidade][], [evento][], [grupo][], [mensagem][], [usuário][], [alerta][] |
| Delegado - conta pessoal da Microsoft | [entre em contato][], [unidade][], [evento][], [mensagem][]                                        |
| Aplicativo                            | [entre em contato][], [conversa][], [unidade][], [evento][], [grupo][], [mensagem][], [usuário][], [alerta][] |

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](./subscription.md)
- [Inscrições de lista](../api/subscription-list.md)
- [Obter assinatura](../api/subscription-get.md)
- [Criar assinatura](../api/subscription-post-subscriptions.md)
- [Atualizar assinatura](../api/subscription-update.md)
- [Excluir assinatura](../api/subscription-delete.md)

[contato]: ./contact.md
[conversa]: ./conversation.md
[unidade]: ./drive.md
[evento]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alerta]: ./alert.md