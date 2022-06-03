---
title: Obter credentialUserRegistrationsSummary
description: Leia as propriedades e as relações de um objeto credentialUserRegistrationsSummary.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 4706e4b7ef0ea410d1442c5b79dbd3a772cf492f
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884257"
---
# <a name="get-credentialuserregistrationssummary"></a>Obter credentialUserRegistrationsSummary
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) .

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
GET /tenantRelationships/managedTenants/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummaryId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte [aos parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, `$apply`incluindo , `$count`, `$filter`, `$orderBy`, `$select`, `$skip`e `$top`.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um [objeto credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationssummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummaryId}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationssummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationssummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationssummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationssummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-credentialuserregistrationssummary-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.credentialUserRegistrationsSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b",
    "mfaAndSsprCapableUserCount": 0,
    "ssprEnabledUserCount": 1,
    "mfaRegisteredUserCount": 0,
    "mfaExcludedUserCount": 2,
    "ssprRegisteredUserCount": 0,
    "totalUserCount": 7,
    "securityDefaultsEnabled": false,
    "mfaConditionalAccessPolicyState": "enabledForReportingButNotEnforced",
    "lastRefreshedDateTime": "2021-07-11T11:15:52.9375367Z",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee"
}
```
