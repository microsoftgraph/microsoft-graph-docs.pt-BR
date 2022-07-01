---
title: APIs protegidas no Microsoft Teams
description: As APIs do Microsoft Teams Microsoft Graph que acessam dados confidenciais são consideradas APIs protegidas e exigem validação adicional antes que você possa usá-los.
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: a8c7de28d1ecd5784e69e2cc4774802282b8bd24
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577809"
---
# <a name="protected-apis-in-microsoft-teams"></a>APIs protegidas no Microsoft Teams

As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas. Essas APIs exigem que você tenha validação adicional além de permissões e consentimento antes de poder usá-las.

As seguintes APIs estão protegidas no momento e todas usam as [permissões do aplicativo Microsoft Graph](auth/auth-concepts.md#microsoft-graph-permissions):

* [Listar mensagens do canal](/graph/api/channel-list-messages)
* [Obter chatMessages em um delta de canal](/graph/api/chatmessage-delta)
* [Obter mensagem do canal](/graph/api/chatmessage-get)
* [Criar assinatura para novas mensagens de canal](/graph/api/subscription-post-subscriptions)
* [List replies to a message](/graph/api/chatmessage-list-replies)
* [Get a reply to a message](/graph/api/chatmessage-get)
* (Listar chats não existe, com ou sem acesso à API protegida)
* [Listar mensagens em um chat](/graph/api/chat-list-messages)
* [Receba uma mensagem no bate-papo](/graph/api/chatmessage-get)
* [Criar assinatura para novas mensagens de chat](/graph/api/subscription-post-subscriptions)
* [Listar todo o conteúdo hospedado](/graph/api/chatmessage-list-hostedcontents)
* [Obter conteúdo hospedado](/graph/api/chatmessagehostedcontent-get)
* [Obter mensagens em uma equipe excluída](/graph/api/deletedteam-getallmessages)

> [!NOTE]
> [Enviar mensagem](/graph/api/channel-post-messages) não é uma API protegida.

## <a name="request-access-to-protected-apis"></a>Solicitar acesso a APIs protegidas

Para solicitar acesso a essas APIs protegidas, complete o [formulário de solicitação](https://forms.office.com/r/v3qjyzBCxD) a seguir. Geralmente, analisamos as solicitações de acesso toda quarta-feira e implantamos aprovações toda sexta-feira ou segunda-feira, exceto durante as semanas de feriados principais nos Envios dos EUA durante essas semanas são processados na semana não feriado a seguir.

Para verificar se sua solicitação foi aprovada, teste seu acesso ao aplicativo na próxima segunda-feira aplicável. Se tivermos dúvidas adicionais sobre a solicitação, entraremos em contato pelo email especificado no formulário.

## <a name="see-also"></a>Confira também

* [Visão geral da API do Microsoft Teams](teams-concept-overview.md)