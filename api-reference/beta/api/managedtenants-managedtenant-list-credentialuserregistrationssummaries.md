---
title: Listar credentialUserRegistrationsSummaries
description: Obter uma lista dos objetos credentialUserRegistrationsSummary e suas propriedades.
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 20b3900022122f3cab9769b1b5c6cea0d0ee3800
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022129"
---
# <a name="list-credentialuserregistrationssummaries"></a>Listar credentialUserRegistrationsSummaries
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos [objetos credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Reports.Read.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
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

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_credentialuserregistrationssummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-credentialuserregistrationssummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-credentialuserregistrationssummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-credentialuserregistrationssummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-credentialuserregistrationssummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-credentialuserregistrationssummary-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.credentialUserRegistrationsSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#credentialUserRegistrationsSummaries",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "mfaAndSsprCapableUserCount": 2,
      "ssprEnabledUserCount": 9,
      "mfaRegisteredUserCount": 3,
      "ssprRegisteredUserCount": 2,
      "totalUserCount": 9,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabled",
      "lastRefreshedDateTime": "2021-07-11T09:58:11.5730661Z",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b",
      "mfaAndSsprCapableUserCount": 0,
      "ssprEnabledUserCount": 1,
      "mfaRegisteredUserCount": 0,
      "ssprRegisteredUserCount": 0,
      "totalUserCount": 7,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabledForReportingButNotEnforced",
      "lastRefreshedDateTime": "2021-07-11T11:15:52.9375367Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    }
  ]
}
```
