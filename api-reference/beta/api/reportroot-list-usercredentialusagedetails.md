---
title: Listar userCredentialUsageDetails
description: Obter uma lista de objetos userCredentialUsageDetails para um determinado locatário.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 3b2efb78529fe0a066ce17f1306574f5ff5f7691
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011063"
---
# <a name="list-usercredentialusagedetails"></a>Listar userCredentialUsageDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista [de objetos userCredentialUsageDetails](../resources/usercredentialusagedetails.md) para um determinado locatário. Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Reports.Read.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Reports.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esta função dá suporte ao parâmetro opcional de consulta OData **$filter**. Você pode aplicar **$filter** em uma ou mais das seguintes propriedades do [recurso userCredentialUsageDetails.](../resources/usercredentialusagedetails.md)

| Propriedades | Descrição e exemplo |
|:--------- |:----------- |
| feature | Filtrar por tipo de dados de uso que você deseja (registro versus redefinição). Por exemplo: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`. Operadores de filtro com suporte: `eq` |
| userDisplayName | Filtrar pelo nome de exibição do usuário. Por exemplo: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`. Operadores de filtro com suporte: `eq` e `startswith()` . Oferece suporte a maiúsculas e minúsculas. |
| userPrincipalName  | Filtrar pelo nome principal do usuário. Por exemplo: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.    Operadores de filtro com suporte: `eq` e `startswith()` . Oferece suporte a maiúsculas e minúsculas. |
| isSuccess | Filtrar por status da atividade. Por exemplo: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`. Operadores de filtro com suporte: `eq` e `orderby` . |
| authMethod  | Filtrar pelos métodos de autenticação que usam durante o registro. Por exemplo: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`. Operadores de filtro com suporte: `eq` . |
| failureReason | Filtrar por motivo de falha (se a atividade tiver falhado). Por exemplo: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`. Operadores de filtro com suporte: `eq` e `startswith()` . Oferece suporte a maiúsculas e minúsculas. |


## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userCredentialUsageDetails](../resources/usercredentialusagedetails.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-usercredentialusagedetails-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades são retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getUserCredentialUsageDetails)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "userPrincipalName":"userPrincipalName-value",
      "userDisplayName": "userDisplayName-value",
      "isSuccess" : true,
      "authMethod": "email",
      "failureReason": "User contacted an admin after trying the email verification option",
      "eventDateTime" : "2019-04-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userCredentialUsageDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


