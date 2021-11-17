---
title: Obter tenantTag
description: Leia as propriedades e as relações de um objeto tenantTag.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c0943d1a407c6843668794914711d852f715b76b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022031"
---
# <a name="get-tenanttag"></a>Obter tenantTag
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto tenantTag.](../resources/managedtenants-tenanttag.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ManagedTenants.Read.All, ManagedTenants.WriteRead.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [tenantTag](../resources/managedtenants-tenanttag.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-tenanttag-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags/$entity",
    "id": "913391c0-5466-42b4-900d-0a7501399cb0",
    "displayName": "Onboarding",
    "description": "Tenants that we are currently onboarding",
    "tenantIds": [
        "38227791-a88b-4fcc-81c5-58cf77668320",
        "34298981-4fc8-4974-9486-c8909ed1521b",
        "4d262a25-c70a-430b-9e8e-46c31dec116b"
    ],
    "isDeleted": null,
    "createdDateTime": "2021-06-16T20:36:31.086644Z",
    "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
    "lastActionDateTime": "2021-06-28T20:46:09.0071888Z",
    "lastActionByUserId": "08ea0285-30cb-46cc-abc8-3d8422e21ecb",
    "tenants": [
        {
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
        },
        {
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
        },
        {
            "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
        }
    ]
}
```
