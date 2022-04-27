---
title: 'applicationTemplate: criar uma instância'
description: Usar essa API para criar um novo applicationTemplate
ms.localizationpriority: medium
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f0374ec223daba8f5df49ebb89d764eec24cee0c
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060553"
---
# <a name="applicationtemplate-instantiate"></a>applicationTemplate: criar uma instância

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione uma instância de um aplicativo da galeria de aplicativos do Azure AD ao seu diretório. Você também pode usar essa API para criar uma instância de [aplicativos que não são da galeria](/azure/active-directory/manage-apps/add-non-gallery-app). Use a seguinte ID para o **objeto applicationTemplate** : `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.

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

Para criar uma instância de aplicativos que não são da galeria, use o `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` para `{applicationTemplate-id}`.

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

Se tiver êxito, este método retornará um código `201 Created` de resposta e um novo [objeto applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. A URL de solicitação especifica `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` como a ID do modelo de aplicativo. Isso significa que a solicitação está instanciando um aplicativo que não é da galeria.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/beta/applicationTemplates/8adf8e6e-67b2-4cf2-a259-e3dc5476c621/instantiate
Content-type: application/json

{
    "displayName": "testProperties"
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
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.applicationServicePrincipal",
    "application": {
        "objectId": "428fbcb1-35bc-471d-95f2-6cc339357cb5",
        "appId": "23a223ba-bb90-4949-8232-1bf479189e9b",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "displayName": "testProperties",
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "identifierUris": [],
        "publicClient": null,
        "replyUrls": [],
        "logoutUrl": null,
        "samlMetadataUrl": null,
        "errorUrl": null,
        "groupMembershipClaims": null,
        "availableToOtherTenants": false
    },
    "servicePrincipal": {
        "objectId": "7b358fa1-7d10-4a57-bd96-b7e63c2f9be5",
        "deletionTimestamp": null,
        "accountEnabled": true,
        "appId": "23a223ba-bb90-4949-8232-1bf479189e9b",
        "appDisplayName": "testProperties",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "appOwnerTenantId": "29a4f813-9274-4e1b-858d-0afa98ae66d4",
        "appRoleAssignmentRequired": true,
        "displayName": "testProperties",
        "errorUrl": null,
        "loginUrl": null,
        "logoutUrl": null,
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "samlMetadataUrl": null,
        "microsoftFirstParty": null,
        "publisherName": "Contoso",
        "preferredSingleSignOnMode": null,
        "preferredTokenSigningKeyThumbprint": null,
        "preferredTokenSigningKeyEndDateTime": null,
        "replyUrls": [],
        "servicePrincipalNames": [
            "23a223ba-bb90-4949-8232-1bf479189e9b"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp",
            "WindowsAzureActiveDirectoryCustomSingleSignOnApplication"
        ],
        "notificationEmailAddresses": [],
        "samlSingleSignOnSettings": null,
        "keyCredentials": [],
        "passwordCredentials": []
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

