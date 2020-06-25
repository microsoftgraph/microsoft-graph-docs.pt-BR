---
title: Remover homeRealmDiscoveryPolicy
description: Remover um homeRealmDiscoveryPolicy de um servicePrincipalName.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 222c37a8de4880e162f5585cd8e7149c6e162e5c
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864109"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="90549-103">Remover homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="90549-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="90549-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90549-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90549-105">Remover um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) de um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="90549-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="90549-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="90549-106">Permissions</span></span>

<span data-ttu-id="90549-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="90549-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="90549-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90549-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90549-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90549-109">Permission type</span></span>                        | <span data-ttu-id="90549-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90549-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90549-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90549-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90549-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="90549-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="90549-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90549-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90549-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90549-114">Not supported.</span></span> |
| <span data-ttu-id="90549-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90549-115">Application</span></span>                            | <span data-ttu-id="90549-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="90549-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90549-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90549-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="90549-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90549-118">Request headers</span></span>

| <span data-ttu-id="90549-119">Nome</span><span class="sxs-lookup"><span data-stu-id="90549-119">Name</span></span>          | <span data-ttu-id="90549-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="90549-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="90549-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="90549-121">Authorization</span></span> | <span data-ttu-id="90549-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="90549-122">Bearer {token}.</span></span> <span data-ttu-id="90549-123">Required.</span><span class="sxs-lookup"><span data-stu-id="90549-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90549-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90549-124">Request body</span></span>

<span data-ttu-id="90549-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90549-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90549-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="90549-126">Response</span></span>

<span data-ttu-id="90549-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="90549-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="90549-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90549-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90549-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90549-129">Request</span></span>

<span data-ttu-id="90549-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90549-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="90549-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="90549-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="90549-132">C#</span><span class="sxs-lookup"><span data-stu-id="90549-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90549-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90549-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90549-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90549-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90549-135">Java</span><span class="sxs-lookup"><span data-stu-id="90549-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90549-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="90549-136">Response</span></span>

<span data-ttu-id="90549-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90549-137">The following is an example of the response.</span></span>

> <span data-ttu-id="90549-138">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="90549-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="90549-139">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="90549-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
