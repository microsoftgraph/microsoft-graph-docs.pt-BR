---
title: Excluir accessPackage
description: Exclua accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b48b132bc12bd35b248be0efe33b038fcd884a35
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176399"
---
# <a name="delete-accesspackage"></a><span data-ttu-id="cab9c-103">Excluir accessPackage</span><span class="sxs-lookup"><span data-stu-id="cab9c-103">Delete accessPackage</span></span>

<span data-ttu-id="cab9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cab9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cab9c-105">[Exclua um objeto accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="cab9c-105">Delete an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cab9c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cab9c-106">Permissions</span></span>

<span data-ttu-id="cab9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cab9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cab9c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cab9c-109">Permission type</span></span>                        | <span data-ttu-id="cab9c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cab9c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cab9c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cab9c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cab9c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cab9c-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="cab9c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cab9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cab9c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cab9c-114">Not supported.</span></span> |
| <span data-ttu-id="cab9c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cab9c-115">Application</span></span>                            | <span data-ttu-id="cab9c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cab9c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cab9c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cab9c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cab9c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cab9c-118">Request headers</span></span>

| <span data-ttu-id="cab9c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cab9c-119">Name</span></span>          | <span data-ttu-id="cab9c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cab9c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cab9c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cab9c-121">Authorization</span></span> | <span data-ttu-id="cab9c-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="cab9c-122">Bearer \{token\}.</span></span> <span data-ttu-id="cab9c-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cab9c-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cab9c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cab9c-124">Request body</span></span>

<span data-ttu-id="cab9c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cab9c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cab9c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab9c-126">Response</span></span>

<span data-ttu-id="cab9c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cab9c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cab9c-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cab9c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cab9c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cab9c-130">Request</span></span>

<span data-ttu-id="cab9c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cab9c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cab9c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cab9c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackage"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="cab9c-133">C#</span><span class="sxs-lookup"><span data-stu-id="cab9c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cab9c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cab9c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cab9c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cab9c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cab9c-136">Java</span><span class="sxs-lookup"><span data-stu-id="cab9c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cab9c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cab9c-137">Response</span></span>

<span data-ttu-id="cab9c-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cab9c-138">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


