---
title: Trabalhar com usuários no Microsoft Graph
description: Crie experiências atraentes para aplicativos baseadas nos usuários, suas relações com outros usuários e grupos, seus emails, calendários e arquivos.
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: conceptualPageType
ms.openlocfilehash: 7c1d2df4e6d1795e1cc4965e8bfcfe4bf4e4d9c8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761780"
---
# <a name="working-with-users-in-microsoft-graph"></a>Trabalhar com usuários no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.

Você pode acessar usuários pelo Microsoft Graph de duas maneiras:

- Por sua ID, `/users/{id}`
- Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`

## <a name="authorization"></a>Autorização

Uma das seguintes [permissões](/graph/permissions-reference) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- User.ManageIdentities.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="common-properties"></a>Propriedades comuns

| Propriedade | Descrição |
|----------|-------------|
| displayName | O nome exibido no catálogo de endereços do usuário.|
|givenName| O nome do usuário. |
|surname| O sobrenome do usuário. |
|email| O endereço de email do usuário. |
|photo| A foto de perfil do usuário. |

Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).

## <a name="common-operations"></a>Operações comuns

>**Observação:** Algumas destas operações exigem permissões adicionais.

| Caminho    | Descrição |
|---------|-------------|
|[`/users`](../api/user-list.md) | Lista os usuários na organização. |
|[`/users/{id}`](../api/user-get.md) | Obtém um usuário específico pela id. |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| Obtém a foto de perfil do usuário. |
|[`/users/{id}/manager`](../api/user-list-manager.md) | Obtém o gerente do usuário. |
|[`/users/{id}/messages`](../api/user-list-messages.md)| Lista as mensagens de email do usuário em sua caixa de entrada principal. |
|[`/users/{id}/events`](../api/user-list-events.md) | Lista os eventos futuros do usuário em seu calendário. |
|[`/users/{id}/drive`](../api/drive-get.md)| Obtém o repositório de arquivos do OneDrive do usuário. |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| Lista os grupos dos quais o usuário é membro. |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| Lista as Microsoft Teams das quais o usuário é membro. |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.