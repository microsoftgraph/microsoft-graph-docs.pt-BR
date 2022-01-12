---
title: Listar tenantTags
description: Obter uma lista dos objetos tenantTag e suas propriedades.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 91d7ca7c56593b7ce97c3aba02f37bae36772eb9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791235"
---
# <a name="list-tenanttags"></a>Listar tenantTags
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos objetos [tenantTag](../resources/managedtenants-tenanttag.md) e suas propriedades.

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
GET /tenantRelationships/managedTenants/tenantTags
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

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos tenantTag](../resources/managedtenants-tenanttag.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-tenanttag-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags",
    "value": [
        {
            "id": "913391c0-5466-42b4-900d-0a7501399cb0",
            "displayName": "Onboarding",
            "description": "Tenants that we are currently onboarding",
            "properties": null,
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
        },
        {
            "id": "bfd883e8-10f3-40ee-994c-111fa1c5d1db",
            "displayName": "ExtendedSupport",
            "description": "Tenants that have purchased extended support.",
            "properties": null,
            "tenantIds": [
                "38227791-a88b-4fcc-81c5-58cf77668320",
                "4d262a25-c70a-430b-9e8e-46c31dec116b"
            ],
            "isDeleted": null,
            "createdDateTime": "2021-06-16T20:43:31.8917383Z",
            "createdByUserId": "43a2424c-0fa3-446d-bee9-4ab500bb1603",
            "lastActionDateTime": "2021-06-17T03:23:31.3531635Z",
            "lastActionByUserId": "248f617e-a6a7-4d31-922d-726c24074bb6",
            "tenants": [
                {
                    "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
                },
                {
                    "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
                }
            ]
        }
    ]
}
```
