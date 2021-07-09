---
title: Obter aplicativo
description: Obtenha as propriedades e os relacionamentos de um objeto application.
author: sureshja
localization_priority: Priority
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1fbfebb6a889ffae5ae6052cc1b774d335f9fb50
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350871"
---
# <a name="get-application"></a><span data-ttu-id="0d29f-103">Obter aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d29f-103">Get application</span></span>

<span data-ttu-id="0d29f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d29f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d29f-105">Obtenha as propriedades e os relacionamentos de um objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="0d29f-105">Get the properties and relationships of an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d29f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d29f-106">Permissions</span></span>
<span data-ttu-id="0d29f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d29f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d29f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d29f-109">Permission type</span></span>      | <span data-ttu-id="0d29f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d29f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d29f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d29f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d29f-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d29f-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d29f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d29f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d29f-114">Application.Read.All, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d29f-114">Application.Read.All, Application.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d29f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d29f-115">Application</span></span> | <span data-ttu-id="0d29f-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy,  Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d29f-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy,  Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d29f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d29f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0d29f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0d29f-118">Optional query parameters</span></span>
<span data-ttu-id="0d29f-119">Este método suporta o `$select` [parâmetro de consulta OData](/graph/query-parameters) para recuperar as propriedades específicas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d29f-119">This method supports the `$select` [OData query parameter](/graph/query-parameters) to retrieve specific application properties.</span></span> 
## <a name="request-headers"></a><span data-ttu-id="0d29f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d29f-120">Request headers</span></span>
| <span data-ttu-id="0d29f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0d29f-121">Name</span></span>           | <span data-ttu-id="0d29f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d29f-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="0d29f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d29f-123">Authorization</span></span>  | <span data-ttu-id="0d29f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d29f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d29f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d29f-126">Request body</span></span>
<span data-ttu-id="0d29f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d29f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d29f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d29f-128">Response</span></span>

<span data-ttu-id="0d29f-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d29f-129">If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="0d29f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d29f-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="0d29f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d29f-131">Request</span></span>
<span data-ttu-id="0d29f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d29f-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d29f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d29f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="0d29f-134">C#</span><span class="sxs-lookup"><span data-stu-id="0d29f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d29f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d29f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d29f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d29f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d29f-137">Java</span><span class="sxs-lookup"><span data-stu-id="0d29f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0d29f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d29f-138">Response</span></span>
<span data-ttu-id="0d29f-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d29f-139">Here is an example of the response.</span></span> 

><span data-ttu-id="0d29f-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0d29f-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
    "id": "03ef14b0-ca33-4840-8f4f-d6e91916010e",
    "deletedDateTime": null,
    "isFallbackPublicClient": null,
    "appId": "631a96bc-a705-4eda-9f99-fdaf9f54f6a2",
    "applicationTemplateId": null,
    "identifierUris": [],
    "createdDateTime": "2019-09-17T19:10:35.2742618Z",
    "disabledByMicrosoftStatus": null,
    "displayName": "Display name",
    "isDeviceOnlyAuthSupported": null,
    "groupMembershipClaims": null,
    "optionalClaims": null,
    "addIns": [],
    "publisherDomain": "contoso.onmicrosoft.com",
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
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
    "uniqueName": null,
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



