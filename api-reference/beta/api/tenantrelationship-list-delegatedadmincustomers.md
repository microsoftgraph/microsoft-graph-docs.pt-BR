---
title: Listar delegatedAdminCustomers
description: Obtenha uma lista dos objetos delegatedAdminCustomer e suas propriedades.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: 9fca3b93bea1a4c1d9597c664645f335a2368e89
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211337"
---
# <a name="list-delegatedadmincustomers"></a>Listar delegatedAdminCustomers
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos delegatedAdminCustomer](../resources/delegatedadmincustomer.md) e suas propriedades.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| DelegatedAdminRelationship.Read.All, DelegatedAdminRelationship.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)| Sem suporte. |
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminCustomers
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte aos `$select`[parâmetros](/graph/query-parameters) `$top`de consulta , `$filter`, `$orderBy`, e `$count``$skipToken` OData para ajudar a personalizar a resposta.  

`$top` dá suporte a até 300 objetos.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de objetos [delegatedAdminCustomer](../resources/delegatedadmincustomer.md) no corpo da resposta.

Cada **objeto delegatedAdminCustomer** contém uma **propriedade @odata.etag** de acordo com RFC2616.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_delegatedadmincustomer"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminCustomers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-delegatedadmincustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-delegatedadmincustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-delegatedadmincustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-delegatedadmincustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-delegatedadmincustomer-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminCustomer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#delegatedAdminCustomers",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminCustomer",
      "@odata.etag": "W/\"JyIxODAwMTMzZi0wMDAwLTAyMDAtMDAwMC02MTNjMGFhZTAwMDAiJw==\"",
      "id": "4fdbff88-9d6b-42e0-9713-45c922ba8001",
      "tenantId": "4fdbff88-9d6b-42e0-9713-45c922ba8001",
      "displayName": "Contoso Inc"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminCustomer",
      "@odata.etag": "W/\"JyIwMDAwMTEwMS0wMDAwLTAyMDAtMDAwMC02MDI1OTQyMjAwMDAiJw==\"",
      "id": "1c0fa218-5dec-49db-8247-cfa457af8116",
      "tenantId": "1c0fa218-5dec-49db-8247-cfa457af8116",
      "displayName": "Contoso subsidiary Inc"
    }
  ]
}
```

