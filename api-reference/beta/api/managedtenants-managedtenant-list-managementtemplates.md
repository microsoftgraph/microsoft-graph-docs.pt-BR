---
title: Gerenciamento de listasTemplates
description: Obter uma lista dos objetos managementTemplate e suas propriedades.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: ae11001e65552a35df429880b9ff891c00cc24b7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981066"
---
# <a name="list-managementtemplates"></a>Gerenciamento de listasTemplates
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos [objetos managementTemplate](../resources/managedtenants-managementtemplate.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ManagedTenants.Read.All, ManagedTenants.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementTemplates
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos managementTemplate](../resources/managedtenants-managementtemplate.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_managementtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplates
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-managementtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-managementtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-managementtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-managementtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-managementtemplate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementTemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementTemplates",
  "value": [
    {
      "id": "e5834405-43d2-4815-867d-3dd600308d1c_1",
      "displayName": "Baseline - Block Legacy Authentication",
      "description": null,
      "category": "identity",
      "parameters": [
        {
          "valueType": "string",
          "displayName": "DisplayName",
          "description": null,
          "jsonDefaultValue": "\"Baseline - Block Legacy Authentication\"",
          "jsonAllowedValues": "null"
        },
        {
          "valueType": "string",
          "displayName": "State",
          "description": null,
          "jsonDefaultValue": "\"enabledForReportingButNotEnforced\"",
          "jsonAllowedValues": "[\"enabled\",\"disabled\",\"enabledForReportingButNotEnforced\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "ClientAppTypes",
          "description": null,
          "jsonDefaultValue": "[\"exchangeActiveSync\",\"other\"]",
          "jsonAllowedValues": "[\"exchangeActiveSync\",\"other\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeApplications",
          "description": null,
          "jsonDefaultValue": "[\"All\"]",
          "jsonAllowedValues": "[\"All\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeUsers",
          "description": null,
          "jsonDefaultValue": "[\"None\"]",
          "jsonAllowedValues": "[\"All\",\"None\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeLocations",
          "description": null,
          "jsonDefaultValue": "[\"All\"]",
          "jsonAllowedValues": "[\"All\",\"AllTrusted\"]"
        },
        {
          "valueType": "string",
          "displayName": "GrantControls.Operator",
          "description": null,
          "jsonDefaultValue": "\"OR\"",
          "jsonAllowedValues": "[\"OR\",\"AND\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "GrantControls.BuiltInControls",
          "description": null,
          "jsonDefaultValue": "[\"block\"]",
          "jsonAllowedValues": "[\"block\"]"
        }
      ],
      "workloadActions": [
        {
          "actionId": "6a3ad0bc-5d7e-4a49-a105-c559aa4633e1",
          "category": "automated",
          "displayName": "ConditionalAccessPolicy",
          "description": null,
          "service": "AAD",
          "settings": [
            {
              "valueType": "string",
              "displayName": "DisplayName",
              "overwriteAllowed": false,
              "jsonValue": "\"Baseline - Block Legacy Authentication\""
            },
            {
              "valueType": "string",
              "displayName": "State",
              "overwriteAllowed": false,
              "jsonValue": "\"enabledForReportingButNotEnforced\""
            },
            {
              "valueType": "stringCollection",
              "displayName": "ClientAppTypes",
              "overwriteAllowed": false,
              "jsonValue": "[\"exchangeActiveSync\",\"other\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeApplications",
              "overwriteAllowed": false,
              "jsonValue": "[\"All\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeUsers",
              "overwriteAllowed": false,
              "jsonValue": "[\"None\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeLocations",
              "overwriteAllowed": false,
              "jsonValue": "[\"All\"]"
            },
            {
              "valueType": "string",
              "displayName": "GrantControls.Operator",
              "overwriteAllowed": false,
              "jsonValue": "\"OR\""
            },
            {
              "valueType": "stringCollection",
              "displayName": "GrantControls.BuiltInControls",
              "overwriteAllowed": false,
              "jsonValue": "[\"block\"]"
            }
          ]
        }
      ]
    }
  ]
}
```
