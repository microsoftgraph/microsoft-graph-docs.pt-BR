---
title: Obter entrada
doc_type: apiPageType
description: Obter um objeto signIn que contém todas as assinaturas de um Azure Active Directory locatário.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: ce2fa2046e563e2d294d9022e08354af37038436
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125366"
---
# <a name="get-signin"></a>Obter entrada

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter um [objeto signIn](../resources/signin.md) que contém um evento de login de usuário específico para seu locatário. Isso inclui as ingressações em que um usuário é solicitado a inserir um nome de usuário ou senha e tokens de sessão.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
| Delegado (conta corporativa ou de estudante) | AuditLog.Read.All e Directory.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte |
| Aplicativo | AuditLog.Read.All e Directory.Read.All | 

> [!IMPORTANT]
> Esta API tem um [problema conhecido](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports) e atualmente requer consentimento para as permissões **AuditLog.Read.All** e **Directory.Read.All.**

Os aplicativos devem [estar registrados corretamente](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.

Além das permissões delegadas, o usuário inscreveu precisa pertencer a uma das seguintes funções de diretório que permitem ler relatórios de logons. Para saber mais sobre funções de diretório, consulte Funções do [Azure AD integrados](/azure/active-directory/roles/permissions-reference):
+ Administrador global
+ Leitor global
+ Leitor de Relatórios
+ Administrador de Segurança
+ Operador de segurança
+ Leitor de segurança

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta. Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto signIn](../resources/signin.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/66ea54eb-blah-4ee5-be62-ff5a759b0100
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-signin-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-signin-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id":"66ea54eb-blah-4ee5-be62-ff5a759b0100",
  "createdDateTime":"2021-06-30T16:34:32Z",
  "userDisplayName":"Test contoso",
  "userPrincipalName":"testaccount1@contoso.com",
  "userId":"26be570a-1111-5555-b4e2-a37c6808512d",
  "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
  "appDisplayName":"Azure Portal",
  "authenticationContextClassReferences": [
      {
        "id":"C1",
        "details":"required"
      }
  ],
  "authenticationProtocol": "oAuth2",
  "incomingTokenType": "Primary Refresh Token",
  "ipAddress":"131.107.159.37",
  "clientAppUsed":"Browser",
  "userAgent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36 Edg/91.0.864.54",
  "correlationId":"5d295068-919b-4017-85d8-44be2f5f5483",
  "conditionalAccessStatus":"notApplied",
  "originalRequestId":"7dccb0d7-1041-4d82-b785-d865272e1400",
  "homeTenantId": "4f7a7bc2-28e2-46a3-b90e-5ade5bc90138",
  "homeTenantName": "",
  "isTenantRestricted": false,
  "isInteractive":true,
  "tokenIssuerName":"",
  "tokenIssuerType":"AzureAD",
  "processingTimeInMilliseconds":761,
  "riskDetail":"none",
  "riskLevelAggregated":"none",
  "riskLevelDuringSignIn":"none",
  "riskState":"none",
  "riskEventTypes_v2":[],
  "resourceDisplayName":"Windows Azure Service Management API",
  "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
  "resourceServicePrincipalId": "a6033f22-27f9-45cb-8f63-7dd8a0590e4e",
  "uniqueTokenIdentifier": "ZTE0OTk3YTQtZjg5Mi00YjBiLWIwNTEtZmViZTA1YzJhNDli",
  "resourceTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
  "homeTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
  "authenticationMethodsUsed":[],
  "authenticationRequirement":"singleFactorAuthentication",
  "azureResourceId": "/subscriptions/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/resourceGroups/testRG/providers/Microsoft.Compute/virtualMachines/testVM",
  "federatedCredentialId": "729ab02a-edd5-4ef5-a285-2d91a3c772ab",
  "signInIdentifier":"testaccount1@contoso.com",
  "signInEventTypes":["interactiveUser"],
  "servicePrincipalId":"",
  "sessionLifetimePolicies": [
    {
      "expirationRequirement": "tenantTokenLifetimePolicy",
      "detail": "The user was required to sign in again according to the tenant session lifetime policy"
    }
  ],
  "userType":"member",
  "flaggedForReview":false,
  "isTenantRestricted":false,
  "autonomousSystemNumber":3598,
  "crossTenantAccessType":"none",
  "status":{
      "errorCode":50126,
      "failureReason":"Error validating credentials due to invalid username or password.",
      "additionalDetails":"The user didn't enter the right credentials. \u00a0It's expected to see some number of these errors in your logs due to users making mistakes."
    },
  "deviceDetail":{
      "deviceId":"",
      "displayName":"",
      "operatingSystem":"Windows 10",
      "browser":"Edge 91.0.864",
      "isCompliant":false,
      "isManaged":false,
      "trustType":""
    },
  "location":{
      "city":"Redmond",
      "state":"Washington",
      "countryOrRegion":"US",
      "geoCoordinates":{
        "altitude":null,
        "latitude":47.6807,
        "longitude":-122.1231
      }
    },
  "appliedConditionalAccessPolicies":[],
  "authenticationProcessingDetails":[
      {
        "key":"Login Hint Present",
        "value":"True"
      }
    ],
  "networkLocationDetails":[
      {
        "networkType":"namedNetwork",
        "networkNames":["North America"]
      }
    ],
  "authenticationDetails":[
      {
        "authenticationStepDateTime":"2021-06-30T16:34:32Z",
        "authenticationMethod":"Password",
        "authenticationMethodDetail":"Password in the cloud",
        "succeeded":false,
        "authenticationStepResultDetail":"Invalid username or password or Invalid on-premise username or password.",
        "authenticationStepRequirement":"Primary authentication"
      }
    ],
  "authenticationRequirementPolicies":[],
  "sessionLifetimePolicies":[]
}
```
