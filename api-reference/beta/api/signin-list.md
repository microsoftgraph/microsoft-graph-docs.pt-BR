---
title: Listar logons
doc_type: apiPageType
description: Obtenha uma lista das entradas do usuário em um locatário do Azure Active Directory.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: 2774b547eb38c2d02944f7187fb6aefe0c021a07
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900027"
---
# <a name="list-signins"></a>Listar logons

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista de [objetos signIn](../resources/signin.md) . A lista contém as entradas do usuário para seu locatário do Azure Active Directory. As entradas em que um nome de usuário e senha são passados como parte do token de autorização e entradas federadas bem-sucedidas estão incluídas atualmente nos logs de entrada.

O tamanho máximo e padrão da página é de 1.000 objetos e, por padrão, as entradas mais recentes são retornadas primeiro. Somente os eventos de entrada que ocorreram dentro do período de retenção padrão do Azure AD (Azure Active [Directory) estão](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data) disponíveis.

[!INCLUDE [GDPR-related-guidance](../../includes/gdpr-msgraph-export-note.md)]


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:--------------- |:------------------------------------------- |
| Delegada (conta corporativa ou de estudante) | AuditLog.Read.All e Directory.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte |
| Aplicativo | AuditLog.Read.All e Directory.Read.All | 

> [!IMPORTANT]
> Essa API tem um [problema conhecido](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports) e atualmente requer consentimento para as permissões **AuditLog.Read.All** e **Directory.Read.All** .

Os aplicativos devem [ser registrados corretamente](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.

Além das permissões delegadas, o usuário conectado precisa pertencer a uma das seguintes funções de diretório que permitem ler relatórios de entrada. Para saber mais sobre funções de diretório, confira [as funções internas do Azure AD](/azure/active-directory/roles/permissions-reference):
+ Administrador global
+ Leitor global
+ Leitor de Relatórios
+ Administrador de Segurança
+ Operador de segurança
+ Leitor de segurança

[!INCLUDE [signins-roles-for-ca-data](../../includes/signins-roles-for-ca-data.md)]

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte aos `$top`parâmetros de consulta , `$skiptoken`e `$filter` OData para ajudar a personalizar a resposta. Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta. A coleção de objetos é listada em ordem decrescente com base em **createdDateTime**.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-all-sign-ins"></a>Exemplo 1: Listar todas as entradas
Neste exemplo, o objeto de resposta mostra o usuário conectado usando a MFA que foi disparada por uma política de acesso condicional e o método de autenticação principal é por meio do FIDO.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-signins-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-signins-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"1691d37b-8579-43a7-966a-0f35583c1300",
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
      "ipAddress":"131.107.159.37",
      "clientAppUsed":"Browser",
      "clientCredentialType": "certificate",
      "userAgent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36 Edg/91.0.864.54",
      "correlationId":"5d295068-919b-4017-85d8-44be2f5f5483",
      "conditionalAccessStatus":"notApplied",
      "originalRequestId":"7dccb0d7-1041-4d82-b785-d865272e1400",
      "authenticationProtocol": "oAuth2",
      "incomingTokenType": "Primary Refresh Token",
      "isInteractive":true,
      "homeTenantId": "4f7a7bc2-28e2-46a3-b90e-5ade5bc90138",
      "homeTenantName": "",
      "isTenantRestricted": false,
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
      "resourceTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
      "homeTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
      "authenticationMethodsUsed":[],
      "authenticationRequirement":"singleFactorAuthentication",
      "azureResourceId": "/subscriptions/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/resourceGroups/testRG/providers/Microsoft.Compute/virtualMachines/testVM",
      "federatedCredentialId": "729ab02a-edd5-4ef5-a285-2d91a3c772ab",
      "uniqueTokenIdentifier": "ZTE0OTk3YTQtZjg5Mi00YjBiLWIwNTEtZmViZTA1YzJhNDli",
      "signInIdentifier":"testaccount1@contoso.com",
      "signInEventTypes":["interactiveUser"],
      "servicePrincipalId":"",
      "sessionLifetimePolicies": [
        {
          "expirationRequirement": "tenantTokenLifetimePolicy",
          "detail": "The user was required to sign in again according to the tenant session lifetime policy"
        }
      ],
      "uniqueTokenIdentifier": "ZTE0OTk3YTQtZjg5Mi00YjBiLWIwNTEtZmViZTA1YzJhNDli",
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
  ]
}
```

### <a name="example-2-retrieve-the-first-10-sign-ins-to-apps-with-the-appdisplayname-that-starts-with-azure"></a>Exemplo 2: recuperar as 10 primeiras entradas em aplicativos com o appDisplayName que começa com 'Azure'

Neste exemplo, o objeto de resposta mostra o usuário conectado usando apenas seu método de autenticação principal: uma senha de nuvem. A resposta inclui uma propriedade `@odata.nextLink` que contém uma URL que pode ser usada para recuperar os próximos 10 resultados.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signins?&$filter=startsWith(appDisplayName,'Azure')&$top=10
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-signins-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-signins-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "@odata.nextLink": "https://graph.microsoft.com/beta/auditLogs/signins?$filter=startsWith(appDisplayName%2c%27Azure%27)&$top=10&$skiptoken=3cff228c89605cc89b0dc753668deef4153e8644caa6d83ed1bb5f711b21cba4",
  "value": [
    {
      "id":"1691d37b-8579-43a7-966a-0f35583c1300",
      "createdDateTime":"2021-06-30T16:34:32Z",
      "userDisplayName":"Test contoso",
      "userPrincipalName":"testaccount1@contoso.com",
      "userId":"26be570a-1111-5555-b4e2-a37c6808512d",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"131.107.159.37",
      "clientAppUsed":"Browser",
      "userAgent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36 Edg/91.0.864.54",
      "correlationId":"5d295068-919b-4017-85d8-44be2f5f5483",
      "conditionalAccessStatus":"notApplied",
      "homeTenantId": "4f7a7bc2-28e2-46a3-b90e-5ade5bc90138",
      "homeTenantName": "",
      "isTenantRestricted": false,
      "originalRequestId":"7dccb0d7-1041-4d82-b785-d865272e1400",
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
      "resourceTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
      "homeTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
      "authenticationMethodsUsed":[],
      "authenticationRequirement":"singleFactorAuthentication",
      "authenticationProtocol": "oAuth2",
      "incomingTokenType": "Primary Refresh Token",
      "signInIdentifier":"testaccount1@contoso.com",
      "signInEventTypes":["interactiveUser"],
      "servicePrincipalId":"",
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
      "uniqueTokenIdentifier": "ZTE0OTk3YTQtZjg5Mi00YjBiLWIwNTEtZmViZTA1YzJhNDli",
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
  ]
}
```



### <a name="example-3-retrieve-the-first-10-sign-ins-where-the-signineventtype-is-not-interactiveuser-starting-with-the-latest-sign-in"></a>Exemplo 3: recuperar as 10 primeiras entradas em que o signInEventType não é interactiveUser começando com a entrada mais recente

Neste exemplo, a resposta inclui uma `@odata.nextLink` propriedade que contém uma URL que pode ser usada para recuperar os próximos 10 resultados.

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_ne_nonInteractiveUser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signins?&$filter=(signInEventTypes/any(t: t ne 'interactiveUser'))&$orderBy=createdDateTime DESC&$top=10
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-ne-noninteractiveuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-ne-noninteractiveuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-ne-noninteractiveuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-ne-noninteractiveuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-signins-ne-noninteractiveuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-signins-ne-noninteractiveuser-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "@odata.nextLink": "https://graph.microsoft.com/beta/auditLogs/signins?$filter=(signInEventTypes%2fany(t%3a+t+ne+%27interactiveUser%27))&$top=10&$orderBy=createdDateTime+DESC&$skiptoken=186ac5626b89ae2a991ff26b674ac381be50b941a40542cb66f8136f2887275b",
    "value": [
        {
            "id": "ef1e1fcc-80bd-489b-82c5-16ad80770e00",
            "createdDateTime": "2022-03-18T18:13:37Z",
            "userDisplayName": "MOD Administrator",
            "userPrincipalName": "admin@contoso.com",
            "userId": "4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph Explorer",
            "ipAddress": "197.178.9.154",
            "ipAddressFromResourceProvider": null,
            "clientAppUsed": "Browser",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.51 Safari/537.36",
            "correlationId": "17b4f05d-3659-42b8-856d-99322911d398",
            "conditionalAccessStatus": "notApplied",
            "originalRequestId": "",
            "isInteractive": false,
            "tokenIssuerName": "",
            "tokenIssuerType": "AzureAD",
            "processingTimeInMilliseconds": 132,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes_v2": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "resourceTenantId": "84841066-274d-4ec0-a5c1-276be684bdd3",
            "homeTenantId": "84841066-274d-4ec0-a5c1-276be684bdd3",
            "homeTenantName": "",
            "authenticationMethodsUsed": [],
            "authenticationRequirement": "singleFactorAuthentication",
            "signInIdentifier": "",
            "signInIdentifierType": null,
            "servicePrincipalName": "",
            "signInEventTypes": [
                "nonInteractiveUser"
            ],
            "servicePrincipalId": "",
            "federatedCredentialId": "",
            "userType": "member",
            "flaggedForReview": false,
            "isTenantRestricted": false,
            "autonomousSystemNumber": 33771,
            "crossTenantAccessType": "none",
            "servicePrincipalCredentialKeyId": "",
            "servicePrincipalCredentialThumbprint": "",
            "uniqueTokenIdentifier": "ZWYxZTFmY2MtODBiZC00ODliLTgyYzUtMTZhZDgwNzcwZTAw",
            "incomingTokenType": "none",
            "authenticationProtocol": "none",
            "resourceServicePrincipalId": "943603e4-e787-4fe9-93d1-e30f749aae39",
            "mfaDetail": null,
            "status": {
                "errorCode": 0,
                "failureReason": "Other.",
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "eab73519-780d-4d43-be6d-a4a89af2a348",
                "displayName": "DESKTOP-LK3PESR",
                "operatingSystem": "Windows 10",
                "browser": "Chrome 99.0.4844",
                "isCompliant": false,
                "isManaged": false,
                "trustType": "Azure AD registered"
            },
            "location": {
                "city": "Mombasa",
                "state": "Coast",
                "countryOrRegion": "KE",
                "geoCoordinates": {}
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "80290cf6-04c8-4a25-8252-2b4d7d88228a",
                    "displayName": "Exchange Online Requires Compliant Device",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none",
                    "includeRulesSatisfied": [],
                    "excludeRulesSatisfied": []
                },
                {
                    "id": "a00746d4-8c33-47f7-b120-91936b367a54",
                    "displayName": "Office 365 App Control",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none",
                    "includeRulesSatisfied": [],
                    "excludeRulesSatisfied": []
                }
            ],
            "authenticationProcessingDetails": [
                {
                    "key": "Root Key Type",
                    "value": "Unknown"
                },
                {
                    "key": "Oauth Scope Info",
                    "value": "[\"Application.ReadWrite.All\",\"AppRoleAssignment.ReadWrite.All\",\"DelegatedPermissionGrant.ReadWrite.All\",\"Directory.ReadWrite.All\",\"openid\",\"profile\",\"RoleManagement.Read.Directory\",\"User.Read\",\"email\",\"AuditLog.Read.All\"]"
                }
            ],
            "networkLocationDetails": [
                {
                    "networkType": "namedNetwork",
                    "networkNames": [
                        "Suspicious countries"
                    ]
                }
            ],
            "authenticationDetails": [],
            "authenticationRequirementPolicies": [],
            "sessionLifetimePolicies": [],
            "privateLinkDetails": {
                "policyId": "",
                "policyName": "",
                "resourceId": "",
                "policyTenantId": ""
            }
        }
    ]
}
```
