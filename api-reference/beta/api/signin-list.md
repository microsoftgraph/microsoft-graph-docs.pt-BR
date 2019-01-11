---
title: Lista signIns
description: Recupera as Azure AD entradas do usuário para seu locatário. Entradas que são interativas em natureza (onde uma nome de usuário/senha é passada como parte do token de autorização) e entradas federadas bem-sucedidas atualmente estão incluídas nos logs de entrar.  Os mais recentes signIns são retornados pela primeira vez.
localization_priority: Priority
ms.openlocfilehash: 8596bd168a3e10cbea9e15e2f61d6bd668fd27b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861786"
---
# <a name="list-signins"></a>Lista signIns

Recupera as Azure AD entradas do usuário para seu locatário. Entradas que são interativas em natureza (onde uma nome de usuário/senha é passada como parte do token de autorização) e entradas federadas bem-sucedidas atualmente estão incluídas nos logs de entrar.  Os mais recentes signIns são retornados pela primeira vez.


## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | AuditLog.Read.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte   |
|Aplicativo | AuditLog.Read.All | 

Além disso, os aplicativos devem ser [registrado corretamente](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para o Windows Azure AD.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos seguintes Parâmetros de consulta OData para ajudar a personalizar a resposta. Verifique [Os parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para como usar esses parâmetros.

|Nome     |Descrição                            |Exemplo|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|Filtra os resultados (linhas). |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|Define o tamanho de página de resultados.|`/auditLogs/signIns?$top=1`|
|[$skiptoken](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|Recupera que a próxima página de resultados do resultado define que ocupar várias páginas.|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>Lista de atributos suportados pelo parâmetro $filter
|Nome do atributo |Operadores com suporte|
|:----------------|:------|
|id|eq|
|userId|eq|
|appId|eq|
|createdDateTime| EQ, le, ge|
|userDisplayName| EQ, startswith|
|userPrincipalName| EQ, startswith|
|appDisplayName| EQ, startswith|
|ipAddress| EQ, startswith|
|Cidade do local| EQ, startswith|
|local/estado| EQ, startswith|
|local/countryOrRegion| EQ, startswith|
|status/errorCode|eq|
|id/de usuário de initiatedBy|eq|
|displayName/de usuário de initiatedBy| eq|
|initiatedBy/usuário/userPrincipalName| EQ, startswith|
|clientAppUsed| eq|
|conditionalAccessStatus | eq|
|deviceDetail/navegador| EQ, startswith|
|deviceDetail/operatingSystem| EQ, startswith|
|correlationId| eq|
|riskDetail| eq|
|riskLevelAggregated| eq|
|riskLevelDuringSignIn| eq|
|riskEventTypes| eq|
|riskState| eq|
|originalRequestId| eq|
|tokenIssuerName| eq|
|tokenIssuerType| eq|
|resourceDisplayName| eq|
|resourceId| eq|


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [entrar](../resources/signin.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 264
```
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id":"b01b1726-0147-425e-a7f7-21f252050400",
        "createdDateTime":"2018-11-06T18:48:33.8527147Z",
        "userDisplayName":"Jon Doe",
         "userPrincipalName":"admin@aad171.ccsctp.net",
         "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
        "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
         "appDisplayName":"Azure Portal",
         "ipAddress":"207.254.19.10",
         "clientAppUsed":"Browser",
        "mfaDetail":null,
         "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
         "conditionalAccessStatus":"notApplied",
        "originalRequestId":null,
        "isInteractive":true,
        "tokenIssuerName":null,
        "tokenIssuerType":"AzureAD",
        "processingTimeInMilliseconds":0,
        "riskDetail":"none",
        "riskLevelAggregated":"none",
        "riskLevelDuringSignIn":"none",
        "riskState":"none",
        "riskEventTypes":[

        ],
        "resourceDisplayName":"windows azure service management api",
        "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
        "authenticationMethodsUsed":[

        ],
        "status":{
            "errorCode":50140,
            "failureReason":"This error occurred due to 'Keep me signed in' interrupt when the user was signing-in.",
            "additionalDetails":null
        },
        "deviceDetail":{
            "deviceId":null,
            "displayName":null,
            "operatingSystem":"Windows 7",
            "browser":"Chrome 63.0.3239",
            "isCompliant":null,
            "isManaged":null,
            "trustType":null
        },
        "location":{
            "city":"Lithia Springs",
            "state":"Georgia",
            "countryOrRegion":"US",
            "geoCoordinates":{
                "altitude":null,
                "latitude":33.7930908203125,
                "longitude":-84.445358276367188
            }
        },
        "appliedConditionalAccessPolicies":[
            {
            "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
            "displayName":"New Name here4",
            "enforcedGrantControls":[
                "Mfa",
                "RequireCompliantDevice"
            ],
            "enforcedSessionControls":[

            ],
            "result":"notApplied"
            },
            {
            "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
            "displayName":"PipelineTest4",
            "enforcedGrantControls":[

            ],
            "enforcedSessionControls":[

            ],
            "result":"notEnabled"
            }
        ],
        "authenticationProcessingDetails":[

        ],
        "networkLocationDetails":[

        ]
        }
    
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
