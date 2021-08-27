---
title: APIs protegidas no Microsoft Teams
description: As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 72332c41c62762a3812c65a2cdfa89327b3ff55d
ms.sourcegitcommit: 998c63e6290cfb5ad4a6bd3eb3e249d282f962a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2021
ms.locfileid: "58531225"
---
# <a name="protected-apis-in-microsoft-teams"></a>APIs protegidas no Microsoft Teams

As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas. Essas APIs exigem validação adicional, além de permissões e consentimento, para que você possa usá-las.


As seguintes APIs estão protegidas no momento:
* [Listar mensagens do canal](/graph/api/channel-list-messages) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Obter chatMessages em um delta de canal](/graph/api/chatmessage-delta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber mensagens do canal](/graph/api/chatmessage-get) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Criar assinatura para novas mensagens do canal](/graph/api/subscription-post-subscriptions) usando [permissões do aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar respostas a uma mensagem](/graph/api/chatmessage-list-replies) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber resposta a uma mensagem](/graph/api/chatmessage-get) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* (A lista de chats usando [permissões do aplicativo](auth/auth-concepts.md#microsoft-graph-permissions) não existe, com ou sem acesso protegido à API)
* [Listar messagens em um chat](/graph/api/chat-list-messages) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber mensagens em um chat](/graph/api/chatmessage-get) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Criar assinatura para novas mensagens do canal](/graph/api/subscription-post-subscriptions) usando [permissões do aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar todo o conteúdo hospedado](/graph/api/chatmessage-list-hostedcontents) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Obter conteúdo hospedado](/graph/api/chatmessagehostedcontent-get) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)

>[!NOTE]
>[Enviar mensagem](/graph/api/channel-post-messages) não é uma API protegida.

Para solicitar acesso a essas APIs protegidas, complete o [formulário de solicitação](https://aka.ms/teamsgraph/requestaccess) a seguir. Analisamos solicitações de acesso toda quarta-feira e implantamos aprovações toda sexta-feira, exceto nas principais semanas de feriado nos EUA. Os envios durante essas semanas serão processados na semana seguinte que não seja feriado.

Caso pretenda fornecer informações além do formulário, entre em contato com o [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).
Inclua o ID do aplicativo em todas as correspondências.
