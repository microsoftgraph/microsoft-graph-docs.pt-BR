---
title: Trabalhar com usuários no Microsoft Graph
description: Crie experiências atraentes para aplicativos baseadas nos usuários, suas relações com outros usuários e grupos, seus emails, calendários e arquivos.
localization_priority: Priority
author: krbain
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 74f479ea8d713912fb875a33ac4decca47ce6c61
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353753"
---
# <a name="working-with-users-in-microsoft-graph"></a>Trabalhar com usuários no Microsoft Graph

Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.

Você pode acessar [usuários](user.md) pelo Microsoft Graph de duas maneiras:

- Por sua ID, `/users/{id | userPrincipalName}`
- Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`

## <a name="authorization"></a>Autorização

One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="common-properties"></a>Propriedades comuns

O item a seguir representa o conjunto padrão de propriedades que serão retornadas ao se obter um usuário ou listar usuários. Este é um subconjunto de todas as propriedades disponíveis. Para obter mais propriedades do usuário, use o parâmetro de consulta `$select`.

|Propriedade |Descrição |
|:----------|:-------------|
|id | O identificador exclusivo do usuário.|
|businessPhones | Os números de telefone do usuário.|
|displayName | O nome exibido no catálogo de endereços do usuário.|
|givenName| O nome do usuário. |
|jobTitle | O cargo do usuário.|
|email| O endereço de email do usuário. |
|mobilePhone | O número de telefone celular do usuário.|
|officeLocation | O local do escritório físico do usuário.|
|preferredLanguage | O idioma preferencial do usuário.|
|surname| O sobrenome do usuário. |
|userPrincipalName| O nome UPN do usuário. |

Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).

## <a name="common-operations"></a>Operações comuns

> **Observação:** Algumas destas operações exigem permissões adicionais.

| Caminho    | Descrição |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | Lista os usuários na organização. |
|[`/users/{id}`](../api/user-get.md) | Obtém um usuário específico pela id. |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| Obtém a foto de perfil do usuário. |
|[`/users/{id}/manager`](../api/user-list-manager.md) | Obtém o gerente do usuário. |
|[`/users/{id}/messages`](../api/user-list-messages.md)| Lista as mensagens de email do usuário em sua caixa de entrada principal. |
|[`/users/{id}/events`](../api/user-list-events.md) | Lista os eventos futuros do usuário em seu calendário. |
|[`/users/{id}/drive`](../api/drive-get.md)| Obtém o repositório de arquivos do OneDrive do usuário. |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| Lista os grupos dos quais o usuário é membro. |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.