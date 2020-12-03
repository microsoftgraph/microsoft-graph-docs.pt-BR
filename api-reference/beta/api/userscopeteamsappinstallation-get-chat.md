---
title: Obter chat entre o usuário e o teamsApp
description: Recupere o chat de um em um entre o usuário especificado e o aplicativo Teams.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0e9776b48fcfc64d3a3b1a1f9c5eb49f704adfc2
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564145"
---
# <a name="get-chat-between-user-and-teamsapp"></a>Obter chat entre o usuário e o teamsApp

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere o [chat](../resources/chat.md) do [usuário](../resources/user.md) especificado e o [aplicativo Teams](../resources/teamsapp.md).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps/{id}/chat
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma instância do objeto [chat](../resources/chat.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a>Exemplo 1: listar chats um-on-one entre o usuário especificado e o aplicativo Teams

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}/chat
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "name": "user_chat_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
   "id": "19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c@unq.gbl.spaces"
 }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User chat teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
