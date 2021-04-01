---
title: 'applicationTemplate: instaurá-lo'
description: Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao diretório.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 5891897fb76a356be577f242b1ae5e7648b0e8fb
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473448"
---
# <a name="applicationtemplate-instantiate"></a>applicationTemplate: instaurá-lo

Namespace: microsoft.graph

Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao diretório.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)        |
| :------------------------------------- | :------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Application.ReadWrite.All, Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                     |
| Aplicativo                            | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
| :------------ | :------------ |
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro   | Tipo   | Descrição                    |
| :---------- | :----- | :----------------------------- |
| displayName | String | Nome personalizado do aplicativo |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 OK` novo [objeto applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

> Você pode usar essa API para insinuar [aplicativos que não são da galeria.](/azure/active-directory/manage-apps/add-non-gallery-app) Use a ID a seguir para **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal": {
      "accountEnabled": true,
      "addIns": [],
      "alternativeNames": ["http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired":true,
      "appRoles": [],
      "displayName": "Display name",
      "endpoints": [],
      "homepage": null,
      "id": "id-value",
      "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
      },
      "keyCredentials": [],
      "logoutUrl": null,
      "oauth2PermissionScopes": [],
      "passwordCredentials": [],
      "publisherName": null,
      "replyUrls": [],
      "servicePrincipalNames": [],
      "servicePrincipalType": null,
      "tags": [],
      "tokenEncryptionKeyId": null
   },
   "application": {
            "id": "id-value",
            "isFallbackPublicClient": null,
            "appId": "appId-value",
            "applicationTemplateId": null,
            "identifierUris": [],
            "createdDateTime": "2019-09-17T19:10:35.2742618Z",
            "displayName": "Display name",
            "isDeviceOnlyAuthSupported": null,
            "groupMembershipClaims": null,
            "optionalClaims": null,
            "addIns": [],
            "publisherDomain": "contoso.onmicrosoft.com",
            "signInAudience": "AzureADMyOrg",
            "tags": [],
            "tokenEncryptionKeyId": null,
            "api": {
                    "requestedAccessTokenVersion": 2,
                    "acceptMappedClaims": null,
                    "knownClientApplications": [],
                    "oauth2PermissionScopes": [],
                    "preAuthorizedApplications": []
            },
            "appRoles": [],
            "publicClient": {
                    "redirectUris": []
            },
            "info": {
                    "termsOfServiceUrl": null,
                    "supportUrl": null,
                    "privacyStatementUrl": null,
                    "marketingUrl": null,
                    "logoUrl": null
            },
            "keyCredentials": [],
            "parentalControlSettings": {
                    "countriesBlockedForMinors": [],
                    "legalAgeGroupRule": "Allow"
            },
            "passwordCredentials": [],
            "requiredResourceAccess": [],
            "web": {
                    "redirectUris": [],
                    "homePageUrl": null,
                    "logoutUrl": null,
                    "implicitGrantSettings": {
                            "enableIdTokenIssuance": false,
                            "enableAccessTokenIssuance": false
                    }
            }
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
