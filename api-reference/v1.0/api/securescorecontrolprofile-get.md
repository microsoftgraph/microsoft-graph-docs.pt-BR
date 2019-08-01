---
title: Obter secureScoreControlProfile
description: Recupere as propriedades e os relacionamentos de um objeto secureScoreControlProfile.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: f7bf44ff70afbd54ea26a9fc579ac95e7232f1a6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975627"
---
# <a name="get-securescorecontrolprofile"></a>Obter secureScoreControlProfile

Recupere as propriedades e os relacionamentos de um objeto [securescorecontrolprofile](../resources/securescorecontrolprofile.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) |  SecurityEvents.Read.All, SecurityEvents.ReadWrite.All   |
|Delegada (conta pessoal da Microsoft) |  Sem suporte.  |
|Application | SecurityEvents.Read.All, SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /security/securescorecontrolprofiles/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | Portador {código}. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **secureScoreControlProfile** no corpo da resposta. Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um código de status `206 Partial Content` com a resposta do provedor em um cabeçalho de aviso. Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescorecontrolprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "DLPEnabled",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Config",
  "actionUrl": "https://compliance.microsoft.com/#/policies",
  "controlCategory": "Data",
  "title": "Apply Data Loss Prevention policies", 
  "deprecated": false,
  "implementationCost": "Moderate",
  "lastModifiedDateTime": null,
  "maxScore": 20.0,
  "rank": 55,
  "remediation": "You can create and manage data loss prevention policies in the Policies page of the compliance portal.",
  "remediationImpact": "This change will have a moderate impact on your users.",
  "service": "IP",
  "threats": [
    "Data Exfiltration",
    "Data Spillage"
  ],
  "tier": "Advanced",
  "userImpact": "Moderate",
  "complianceInformation": [
    {
      "certificationName": "ISO 27001:2013",
      "certificationControls": [
        {
          "name": "A.8.2.1",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": null,
      "comment": null,
      "state": "Default",
      "updatedBy": null,
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
    }
  ],
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "get secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
