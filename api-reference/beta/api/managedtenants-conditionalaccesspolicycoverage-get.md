---
title: Obter conditionalAccessPolicyCoverage
description: Leia as propriedades e as relações de um objeto conditionalAccessPolicyCoverage.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: cd06e544fd4439569a8e04a508b5dc123664df27
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002928"
---
# <a name="get-conditionalaccesspolicycoverage"></a>Obter conditionalAccessPolicyCoverage
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de [um objeto conditionalAccessPolicyCoverage.](../resources/managedtenants-conditionalaccesspolicycoverage.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Policy.Read.All, Policy.ReadWrite.ConditionalAccess e Application.Read.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
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

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conditionalaccesspolicycoverage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conditionalaccesspolicycoverage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conditionalaccesspolicycoverage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conditionalaccesspolicycoverage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-conditionalaccesspolicycoverage-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "38227791-a88b-4fcc-81c5-58cf77668320",
  "conditionalAccessPolicyState": "enabled",
  "requiresDeviceCompliance": false,
  "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
  "tenantDisplayName": "Consolidated Messenger"
}
```
