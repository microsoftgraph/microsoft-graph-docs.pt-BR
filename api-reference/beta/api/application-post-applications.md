---
title: Criar aplicativo
description: Crie um novo aplicativo.
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d6fbb458a66f31a53917d4a0a328f399cb2593
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441484"
---
# <a name="create-application"></a><span data-ttu-id="95e5f-103">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="95e5f-103">Create application</span></span>

<span data-ttu-id="95e5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95e5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95e5f-105">Crie um novo objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="95e5f-105">Create a new [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95e5f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="95e5f-106">Permissions</span></span>
<span data-ttu-id="95e5f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95e5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="95e5f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95e5f-109">Permission type</span></span>      | <span data-ttu-id="95e5f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95e5f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95e5f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95e5f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="95e5f-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="95e5f-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="95e5f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95e5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95e5f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95e5f-114">Not supported.</span></span>    |
|<span data-ttu-id="95e5f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95e5f-115">Application</span></span> | <span data-ttu-id="95e5f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5f-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95e5f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95e5f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="95e5f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95e5f-118">Request headers</span></span>
| <span data-ttu-id="95e5f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="95e5f-119">Name</span></span>       | <span data-ttu-id="95e5f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="95e5f-120">Type</span></span> | <span data-ttu-id="95e5f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="95e5f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="95e5f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="95e5f-122">Authorization</span></span>  | <span data-ttu-id="95e5f-123">string</span><span class="sxs-lookup"><span data-stu-id="95e5f-123">string</span></span>  | <span data-ttu-id="95e5f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95e5f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95e5f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95e5f-126">Request body</span></span>
<span data-ttu-id="95e5f-127">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="95e5f-127">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="95e5f-128">O corpo da solicitação deve conter **displayName**, que é uma propriedade obrigatória.</span><span class="sxs-lookup"><span data-stu-id="95e5f-128">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="95e5f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="95e5f-129">Response</span></span>

<span data-ttu-id="95e5f-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95e5f-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95e5f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="95e5f-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="95e5f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95e5f-132">Request</span></span>
<span data-ttu-id="95e5f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95e5f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95e5f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="95e5f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "displayName": "Display name"
}
```
# <a name="c"></a>[<span data-ttu-id="95e5f-135">C#</span><span class="sxs-lookup"><span data-stu-id="95e5f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95e5f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95e5f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95e5f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95e5f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="95e5f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="95e5f-138">Response</span></span>
<span data-ttu-id="95e5f-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95e5f-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="95e5f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95e5f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1145

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
    "id": "03ef14b0-ca33-4840-8f4f-d6e91916010e",
    "deletedDateTime": null,
    "isFallbackPublicClient": null,
    "appId": "631a96bc-a705-4eda-9f99-fdaf9f54f6a2",
    "applicationTemplateId": null,
    "identifierUris": [],
    "createdDateTime": "2019-09-17T19:10:35.2742618Z",
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
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
