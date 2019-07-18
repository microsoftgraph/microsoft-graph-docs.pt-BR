---
title: APIs protegidas no Microsoft Teams
description: As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ebf0bbda324f62c6413bbe3d70ade33a5052da0d
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778758"
---
# <a name="protected-apis-in-microsoft-teams"></a>APIs protegidas no Microsoft Teams

As APIs do Microsoft Teams no Microsoft Graph, que acessam dados confidenciais, são consideradas APIs protegidas. Essas APIs exigem validação adicional, além de permissões e consentimento, para que você possa usá-las.

As seguintes APIs estão protegidas no momento:
* [Listar mensagens do canal](/graph/api/channel-list-messages?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber mensagens do canal](/graph/api/channel-get-message?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar respostas a uma mensagem](/graph/api/channel-list-messagereplies?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber resposta a uma mensagem](/graph/api/channel-get-messagereply?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Listar messagens em um chat](/graph/api/chatmessage-list?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)
* [Receber messagens em um chat](/graph/api/chatmessage-get?view=graph-rest-beta) usando [permissões de aplicativo](auth/auth-concepts.md#microsoft-graph-permissions)

Para solicitar acesso a essas APIs protegidas, complete o [ formulário de solicitação](http://aka.ms/teamsgraph/requestaccess) a seguir. Analisamos as solicitações de acesso semanalmente. Caso pretenda fornecer informações além do formulário, entre em contato com o [teamsAppPerms@microsoft.com](mailto:teamsAppPerms@microsoft.com).
