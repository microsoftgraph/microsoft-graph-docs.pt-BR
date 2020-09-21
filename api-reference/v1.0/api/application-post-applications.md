---
title: Criar aplicativo
description: Crie um novo aplicativo.
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b5187400e0881c865051522adda0398f2bac15ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966384"
---
# <a name="create-application"></a><span data-ttu-id="de1c1-103">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="de1c1-103">Create application</span></span>

<span data-ttu-id="de1c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de1c1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de1c1-105">Crie um novo objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="de1c1-105">Create a new [application](../resources/application.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="de1c1-106">Não é possível adicionar [**passwordCredential**](../resources/passwordcredential.md) ao criar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="de1c1-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating applications is not supported.</span></span> <span data-ttu-id="de1c1-107">Utilize o método [addPassword](application-addpassword.md) para adicionar senhas a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de1c1-107">Use the [addPassword](application-addpassword.md) method to add passwords for an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="de1c1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="de1c1-108">Permissions</span></span>
<span data-ttu-id="de1c1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de1c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="de1c1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de1c1-111">Permission type</span></span>      | <span data-ttu-id="de1c1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de1c1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de1c1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de1c1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="de1c1-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="de1c1-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="de1c1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de1c1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de1c1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de1c1-116">Not supported.</span></span>    |
|<span data-ttu-id="de1c1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de1c1-117">Application</span></span> | <span data-ttu-id="de1c1-118">Application.ReadWrite.All, Application.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="de1c1-118">Application.ReadWrite.All, Application.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="de1c1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de1c1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="de1c1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de1c1-120">Request headers</span></span>
| <span data-ttu-id="de1c1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="de1c1-121">Name</span></span>           | <span data-ttu-id="de1c1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="de1c1-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="de1c1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="de1c1-123">Authorization</span></span>  | <span data-ttu-id="de1c1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de1c1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="de1c1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de1c1-126">Content-Type</span></span>   | <span data-ttu-id="de1c1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de1c1-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de1c1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de1c1-129">Request body</span></span>
<span data-ttu-id="de1c1-130">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="de1c1-130">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="de1c1-131">O corpo da solicitação deve conter **displayName**, que é uma propriedade obrigatória.</span><span class="sxs-lookup"><span data-stu-id="de1c1-131">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="de1c1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="de1c1-132">Response</span></span>

<span data-ttu-id="de1c1-133">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de1c1-133">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de1c1-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="de1c1-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="de1c1-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de1c1-135">Request</span></span>
<span data-ttu-id="de1c1-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de1c1-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="de1c1-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="de1c1-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/v1.0/applications
Content-type: application/json
Content-length: 67

{
  "displayName": "Display name"
}
```
# <a name="c"></a>[<span data-ttu-id="de1c1-138">C#</span><span class="sxs-lookup"><span data-stu-id="de1c1-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de1c1-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de1c1-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de1c1-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de1c1-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de1c1-141">Java</span><span class="sxs-lookup"><span data-stu-id="de1c1-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-application-from-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de1c1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="de1c1-142">Response</span></span>
<span data-ttu-id="de1c1-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de1c1-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="de1c1-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de1c1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications/$entity",
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

