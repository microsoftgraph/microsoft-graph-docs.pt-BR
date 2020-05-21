---
title: APIs protegidas no Microsoft Teams
description: As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 4daf0575c5b9b11249c1dbb21eb11789f0057ac2
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291031"
---
# <a name="protected-apis-in-microsoft-teams"></a>APIs protegidas no Microsoft Teams

As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas. Essas APIs exigem validação adicional, além de permissões e consentimento, para que você possa usá-las.

As seguintes APIs estão protegidas no momento:
* [Listar mensagens do canal](/graph/api/channel-list-messages?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Obter chatMessages em um delta de canal](/graph/api/chatmessage-delta?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber mensagens do canal](/graph/api/channel-get-message?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Criar assinatura para novas mensagens do canal](/graph/api/subscription-post-subscriptions?view=graph-rest-beta) usando [permissões do aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar respostas a uma mensagem](/graph/api/channel-list-messagereplies?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber resposta a uma mensagem](/graph/api/channel-get-messagereply?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* (A lista de chats usando [permissões do aplicativo](auth/auth-concepts.md#microsoft-graph-permissions) não existe, com ou sem acesso protegido à API)
* [Listar messagens em um chat](/graph/api/chatmessage-list?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber mensagens em um chat](/graph/api/chatmessage-get?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Criar assinatura para novas mensagens do canal](/graph/api/subscription-post-subscriptions?view=graph-rest-beta) usando [permissões do aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar todo o conteúdo hospedado](/graph/api/chatmessage-list-chatmessagehostedcontents?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Obter conteúdo hospedado](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar membros do bate-papo](/graph/api/conversationmember-list?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Obter membro do chat](/graph/api/conversationmember-get?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)

>[!NOTE]
>[Enviar mensagem](/graph/api/channel-post-messages?view=graph-rest-beta) não é uma API protegida.

Para solicitar acesso a essas APIs protegidas, complete o [formulário de solicitação](https://aka.ms/teamsgraph/requestaccess) a seguir. Analisamos solicitações de acesso toda quarta-feira e implantamos aprovações toda sexta-feira, exceto nas principais semanas de feriado nos EUA. Os envios durante essas semanas serão processados na semana seguinte que não seja feriado.

Caso pretenda fornecer informações além do formulário, entre em contato com o [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).
