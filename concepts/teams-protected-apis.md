---
title: APIs protegidas no Microsoft Teams
description: As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 1c7c8d18f59346387efbaa3c08de5794ad07ebab
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439881"
---
# <a name="protected-apis-in-microsoft-teams"></a>APIs protegidas no Microsoft Teams

As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas. Essas APIs exigem validação adicional, além de permissões e consentimento, para que você possa usá-las.

As seguintes APIs estão protegidas no momento:
* [Listar mensagens do canal](/graph/api/channel-list-messages?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Obter chatMessages em um delta de canal](/graph/api/chatmessage-delta.md) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber mensagens do canal](/graph/api/channel-get-message?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar respostas a uma mensagem](/graph/api/channel-list-messagereplies?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber resposta a uma mensagem](/graph/api/channel-get-messagereply?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar messagens em um chat](/graph/api/chatmessage-list?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber mensagens em um chat](/graph/api/chatmessage-get?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar todo o conteúdo hospedado](/graph/api/chatmessage-list-chatmessagehostedcontents.md) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Obter conteúdo hospedado](/graph/api/chatmessagehostedcontent-get.md) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar membros do bate-papo](/graph/api/conversationmember-list.md) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Obter membro do chat](/graph/api/conversationmember-get.md) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)

>[!NOTE]
>[Enviar mensagem](/graph/api/channel-post-messages?view=graph-rest-beta) não é uma API protegida.

Para solicitar acesso a essas APIs protegidas, complete o [formulário de solicitação](http://aka.ms/teamsgraph/requestaccess) a seguir. Analisamos as solicitações de acesso toda quarta-feira e fazemos aprovações toda sexta-feira.
Caso pretenda fornecer informações além do formulário, entre em contato com o [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).
