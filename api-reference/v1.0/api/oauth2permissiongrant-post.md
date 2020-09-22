---
title: Criar um oAuth2PermissionGrant
description: Crie um objeto oAuth2PermissionGrant, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 8f5e458738db2b0431a034e9b70d6e727853cbcb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087212"
---
# <a name="create-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="e0ad8-103">Criar uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="e0ad8-103">Create a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="e0ad8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0ad8-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="e0ad8-105">Criar uma concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="e0ad8-105">Create a delegated permission grant.</span></span> <span data-ttu-id="e0ad8-106">Uma concessão de permissão delegada é representada por um objeto [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .</span><span class="sxs-lookup"><span data-stu-id="e0ad8-106">A delegated permission grant is represented by an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

<span data-ttu-id="e0ad8-107">Uma concessão de permissão delegada autoriza uma entidade de serviço de cliente (representando um aplicativo cliente) para acessar uma entidade de serviço de recurso (representando uma API), em nome de um usuário conectado, para o nível de acesso limitado pelas permissões delegadas que foram concedidas.</span><span class="sxs-lookup"><span data-stu-id="e0ad8-107">A delegated permission grant authorizes a client service principal (representing a client application) to access a resource service principal (representing an API), on behalf of a signed-in user, for the level of access limited by the delegated permissions which were granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0ad8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0ad8-108">Permissions</span></span>

<span data-ttu-id="e0ad8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0ad8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0ad8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0ad8-111">Permission type</span></span>      | <span data-ttu-id="e0ad8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0ad8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0ad8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0ad8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e0ad8-114">DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="e0ad8-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e0ad8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0ad8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0ad8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0ad8-116">Not supported.</span></span>    |
|<span data-ttu-id="e0ad8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0ad8-117">Application</span></span> | <span data-ttu-id="e0ad8-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ad8-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0ad8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0ad8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a><span data-ttu-id="e0ad8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0ad8-120">Request headers</span></span>

| <span data-ttu-id="e0ad8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e0ad8-121">Name</span></span>       | <span data-ttu-id="e0ad8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0ad8-122">Type</span></span> | <span data-ttu-id="e0ad8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0ad8-123">Description</span></span> |
|:-----------|:------|:----------|
| <span data-ttu-id="e0ad8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0ad8-124">Authorization</span></span>  | <span data-ttu-id="e0ad8-125">string</span><span class="sxs-lookup"><span data-stu-id="e0ad8-125">string</span></span>  | <span data-ttu-id="e0ad8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0ad8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0ad8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0ad8-128">Request body</span></span>

<span data-ttu-id="e0ad8-129">No corpo da solicitação, forneça uma representação JSON de um objeto [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .</span><span class="sxs-lookup"><span data-stu-id="e0ad8-129">In the request body, supply a JSON representation of an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0ad8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0ad8-130">Response</span></span>

<span data-ttu-id="e0ad8-131">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0ad8-131">If successful, this method returns a 200-series response code and a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0ad8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0ad8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0ad8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0ad8-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e0ad8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0ad8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/v1.0/oauth2PermissionGrants
Content-Type: application/json
Content-Length: 30

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value"
}
```
# <a name="c"></a>[<span data-ttu-id="e0ad8-135">C#</span><span class="sxs-lookup"><span data-stu-id="e0ad8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0ad8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0ad8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0ad8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0ad8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0ad8-138">Java</span><span class="sxs-lookup"><span data-stu-id="e0ad8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e0ad8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0ad8-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "id-value",
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

