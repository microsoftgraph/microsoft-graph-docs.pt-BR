---
title: Obter grupo
description: Obtenha as propriedades e os relacionamentos de um objeto de grupo.
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 739ee7d59ade208bf23feb53593b8e539430c3bc
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784875"
---
# <a name="get-group"></a>Obter grupo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as propriedades e os relacionamentos de um objeto [group](../resources/group.md). 

Esta operação retorna, por padrão, apenas um subconjunto de todas as propriedades disponíveis, conforme indicado na seção [Propriedades](../resources/group.md#properties). Para obter propriedades _não_ retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData. A propriedade **hasMembersWithLicenseErrors** é uma exceção e ela não é retornada na consulta `$select`. Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **group**.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | GroupMember. Read. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All |

>**Observação:** dependendo dos recursos de grupo que você está tentando acessar, as permissões podem ser limitadas. Para obter mais informações, consulte a seção [Grupos](/graph/known-issues#groups) em [Problemas conhecidos com o Microsoft Graph](/graph/known-issues).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.

Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [group](../resources/group.md) no corpo da resposta. Retorna as propriedades padrão, a menos que você use `$select` para especificar as propriedades específicas.

## <a name="example"></a>Exemplo

### <a name="example-1-return-all-default-properties"></a>Exemplo 1: Retornar todas as propriedades padrão

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de solicitação GET. 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Este é um exemplo de resposta. Ele inclui apenas as propriedades padrão.

>**Observação:** O objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades padrão serão retornadas em uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-12-22T02:21:05Z",
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "expirationDateTime": null,
  "groupTypes": [
      "Unified"
  ],
  "isAssignableToRole": null,
  "mail": "golfassist@contoso.com",
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "membershipRule": null,
  "membershipRuleProcessingState": null,
  "onPremisesLastSyncDateTime": null,
  "onPremisesSecurityIdentifier": null,
  "onPremisesSyncEnabled": null,
  "preferredDataLocation": "CAN",
  "preferredLanguage": null,
  "proxyAddresses": [
      "smtp:golfassist@contoso.onmicrosoft.com",
      "SMTP:golfassist@contoso.com"
  ],
  "renewedDateTime": "2018-12-22T02:21:05Z",
  "resourceBehaviorOptions": [],
  "resourceProvisioningOptions": [],
  "securityEnabled": false,
  "theme": null,
  "visibility": "Public",
  "onPremisesProvisioningErrors": []
}
```


### <a name="example-2-return-additional-properties-by-using-select"></a>Exemplo 2: Retornar propriedades adicionais usando $select

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de solicitação GET. 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Veja a seguir o exemplo de uma resposta que inclui as propriedades solicitadas não retornadas por padrão.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group_non_default"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```
### <a name="example-3-read-a-specific-dynamic-group"></a>Exemplo 3: Leia um grupo dinâmico específico

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["1cdf9c18-a7dc-46b1-b47f-094d5656376d"],
  "name": "get_dynamic_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/1cdf9c18-a7dc-46b1-b47f-094d5656376d?$select=id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus)/$entity",
  "id": "1cdf9c18-a7dc-46b1-b47f-094d5656376d",
  "membershipRule": "accountEnabled eq true",
  "membershipRuleProcessingState": "On",
  "membershipRuleProcessingStatus": {
    "status" : "NotStarted",
    "lastMembershipUpdated"  : null,
    "errorMessage" : null
  }
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


