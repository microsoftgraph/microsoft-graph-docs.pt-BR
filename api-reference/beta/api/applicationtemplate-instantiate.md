---
title: 'applicationTemplate: instaurá-lo'
description: Use essa API para criar um novo applicationTemplate
ms.localizationpriority: medium
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: c55b93249535bc12b26c299a3d4a916f739d0fe4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339290"
---
# <a name="applicationtemplate-instantiate"></a>applicationTemplate: instaurá-lo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao diretório.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Application.ReadWrite.All, Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String|Nome personalizado do aplicativo|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 OK` código de resposta e um novo [objeto applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
 
> Você pode usar essa API para insinuar [aplicativos que não são da galeria](/azure/active-directory/manage-apps/add-non-gallery-app). Use a ID a seguir para **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/beta/applicationTemplates/{id}/instantiate
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

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/applicationtemplate-instantiate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/applicationtemplate-instantiate-powershell-snippets.md)]
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
   "servicePrincipal":{
      "accountEnabled":true,
      "addIns":[
         {
            "id":"id-value",
            "type":"type-value",
            "properties":[
               {
                  "key":"key-value",
                  "value":"value-value"
               }
            ]
         }
      ],
      "appDisplayName":"appDisplayName-value",
      "appId":"appId-value",
      "appOwnerOrganizationId":"appOwnerOrganizationId-value",
      "appRoleAssignmentRequired":true
   },
   "application":{
      "api":{
         "acceptedAccessTokenVersion":1,
         "publishedPermissionScopes":[
            {
               "adminConsentDescription":"adminConsentDescription-value",
               "adminConsentDisplayName":"adminConsentDisplayName-value",
               "id":"id-value",
               "isEnabled":true,
               "type":"type-value",
               "userConsentDescription":"userConsentDescription-value",
               "userConsentDisplayName":"userConsentDisplayName-value",
               "value":"value-value"
            }
         ]
      },
      "allowPublicClient":true,
      "applicationAliases":[
         "applicationAliases-value"
      ],
      "createdDateTime":"datetime-value",
      "installedClients":{
         "redirectUrls":[
            "redirectUrls-value"
         ]
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

