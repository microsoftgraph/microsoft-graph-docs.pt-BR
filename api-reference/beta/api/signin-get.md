---
title: Obter entrada
doc_type: apiPageType
description: Obter um objeto signIn que contenha todas as logins de um locatário do Azure Active Directory.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: 139ee4c8ae45699f284d866740c494a86fcb05a9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134124"
---
# <a name="get-signin"></a>Obter entrada

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter um [objeto signIn](../resources/signin.md) que contém um evento de login de usuário específico para seu locatário. Isso inclui as entrada em que um usuário é solicitado a inserir um nome de usuário ou senha e tokens de sessão.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
| Delegado (conta corporativa ou de estudante) | AuditLog.Read.All, Directory.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte |
| Aplicativo | AuditLog.Read.All, Directory.Read.All | 

Além disso, os aplicativos devem ser [corretamente registrados](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta. Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [signIn](../resources/signin.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a>Exemplo 1: o usuário faz o acesso usando a MFA, que é disparada por uma política de acesso condicional. A autenticação principal é por meio do FIDO.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
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

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [
        {
            "id": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-1111-5555-b4e2-a37c6808512d",
            "appId": "de8bc8b5-5555-6666-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "authenticationRequirement": "MultifactorAuthentication",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Safari/537.36 Edg/80.0.361.66",
            "correlationId": "d79f5bee-blah-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "originalRequestId": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "isInteractive": true,
            "tokenIssuerName": "",
            "tokenIssuerType": "AzureAD",
            "processingTimeInMilliseconds": 541,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "riskEventTypes_v2": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "authenticationMethodsUsed": [],
            "alternateSignInName": "testaccount2@contoso.com",
            "servicePrincipalName": null,
            "servicePrincipalId": "",
            "mfaDetail": null,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "",
                "displayName": null,
                "operatingSystem": "Windows 10",
                "browser": "Edge 80.0.361",
                "isCompliant": null,
                "isManaged": null,
                "trustType": null
            },
            "location": {
                "city": "Redmond",
                "state": "Washington",
                "countryOrRegion": "US",
                "geoCoordinates": {
                    "altitude": null,
                    "latitude": 47.68050003051758,
                    "longitude": -122.12094116210938
                }
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "de7e60eb-ed89-4d73-8205-2227def6b7c9",
                    "displayName": "SharePoint limited access for guest workers",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
               
            ],
            "authenticationProcessingDetails": [],
            "networkLocationDetails": [],
            "authenticationDetails": [
                    {
              "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
              "authenticationMethod":"FIDO2",
              "authenticationMethodDetail":"1G54395783",
              "succeeded":true,
              "authenticationStepResultDetail":"methodSucceeded",
              "authenticationStepRequirement":"Primary authentication"
            },
            {
              "authenticationStepDateTime":"2018-11-06T18:48:12.94725647Z",
              "authenticationMethod":"Claim in access token",
              "authenticationMethodDetail":null,
              "succeeded":true,
              "authenticationStepResultDetail":"methodSucceeded",
              "authenticationStepRequirement":"MFA"
            }
            ],
            "authenticationRequirementPolicies": []
        }
    ]
}
```

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a>Exemplo 2: o usuário se insi com apenas a autenticação principal. A autenticação principal é por meio da senha da nuvem.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
       "authenticationRequirement": "singleFactorAuthentication",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"Password",
          "authenticationMethodDetail":"Cloud password",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"notApplied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```
