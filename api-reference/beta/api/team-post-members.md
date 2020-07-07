---
title: Adicionar membros à equipe
description: Adicionar um novo membro a uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 77c70173dd029c7a92f6e31bffa5d092528aa008
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050987"
---
# <a name="create-members"></a>Criar membros
Namespace: microsoft.graph

Adicione um novo [conversationMember](../resources/conversationmember.md) a uma [equipe](../resources/team.md).

## <a name="permissions"></a>Permissões
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| TeamMember. ReadWrite. All|
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo| TeamMember. ReadWrite. All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamsId}/members
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md) .

## <a name="response"></a>Resposta

Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_conversationmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{id}/members
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": [
        "owner"
    ],
    "userId": "50dffbae-ad0f-428e-a86f-f53b0acfc641",
    "displayName": "Cameron White",
    "email": "CameronW@M365x987948.OnMicrosoft.com"
}
```


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "3c02af05-9312-4966-bc84-c1a0818791c4",
    "roles": [
        "owner"
    ],
    "userId": "50dffbae-ad0f-428e-a86f-f53b0acfc641",
    "displayName": "Cameron White",
    "email": "CameronW@M365x987948.OnMicrosoft.com"
}
```
