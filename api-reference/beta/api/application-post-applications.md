---
title: Criar aplicativo
description: Use esta API para criar um novo aplicativo.
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 57c7977799eeca3830adc3b0250dd5c20dbddb23
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945470"
---
# <a name="create-application"></a><span data-ttu-id="e312b-103">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="e312b-103">Create Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e312b-104">Use esta API para criar um novo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e312b-104">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="e312b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e312b-105">Permissions</span></span>
<span data-ttu-id="e312b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e312b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e312b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e312b-108">Permission type</span></span>      | <span data-ttu-id="e312b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e312b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e312b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e312b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e312b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e312b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e312b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e312b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e312b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e312b-113">Not supported.</span></span>    |
|<span data-ttu-id="e312b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e312b-114">Application</span></span> | <span data-ttu-id="e312b-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e312b-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e312b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e312b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="e312b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e312b-117">Request headers</span></span>
| <span data-ttu-id="e312b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e312b-118">Name</span></span>       | <span data-ttu-id="e312b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e312b-119">Type</span></span> | <span data-ttu-id="e312b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e312b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e312b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e312b-121">Authorization</span></span>  | <span data-ttu-id="e312b-122">string</span><span class="sxs-lookup"><span data-stu-id="e312b-122">string</span></span>  | <span data-ttu-id="e312b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e312b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e312b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e312b-125">Request body</span></span>
<span data-ttu-id="e312b-126">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="e312b-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e312b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e312b-127">Response</span></span>

<span data-ttu-id="e312b-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e312b-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e312b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e312b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e312b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e312b-130">Request</span></span>
<span data-ttu-id="e312b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e312b-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e312b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e312b-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "allowPublicClient": true,
  "displayName": "Display name"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e312b-133">C#</span><span class="sxs-lookup"><span data-stu-id="e312b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e312b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e312b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e312b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e312b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e312b-136">Java</span><span class="sxs-lookup"><span data-stu-id="e312b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-application-from-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e312b-137">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="e312b-137">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e312b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e312b-138">Response</span></span>
<span data-ttu-id="e312b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e312b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "id": "b5b2920e-a47c-43b7-91ef-25ae96fddddd",
    "deletedDateTime": null,
    "api": {
        "acceptedAccessTokenVersion": 2,
        "publishedPermissionScopes": []
    },
    "allowPublicClient": true,
    "applicationAliases": [],
    "appRoles": [],
    "createdDateTime": "2017-05-25T16:33:04.3646617Z",
    "installedClients": {
        "redirectUrls": []
    },
    "displayName": "Display name",
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "orgRestrictions": [],
    "passwordCredentials": [],
    "preAuthorizedApplications": [],
    "requiredResourceAccess": [],
    "tags": [],
    "web": {
        "redirectUrls": [],
        "logoutUrl": null,
        "oauth2AllowImplicitFlow": null
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
