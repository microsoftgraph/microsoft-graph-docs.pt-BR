---
title: Excluir unifiedRoleAssignmentMultiple
description: Exclua um objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 85d721888b3f64f77533e6c83c53c84c943ec824
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444851"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="d4854-103">Excluir unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d4854-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="d4854-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4854-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4854-105">[Exclua um objeto unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="d4854-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="d4854-106">Isso é aplicável a um aplicativo RBAC que oferece suporte a várias entidades e escopos.</span><span class="sxs-lookup"><span data-stu-id="d4854-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="d4854-107">O Microsoft Intune é um aplicativo assim.</span><span class="sxs-lookup"><span data-stu-id="d4854-107">Microsoft Intune is such an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4854-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4854-108">Permissions</span></span>

<span data-ttu-id="d4854-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4854-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4854-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4854-111">Permission type</span></span> | <span data-ttu-id="d4854-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4854-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="d4854-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4854-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d4854-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4854-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="d4854-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4854-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4854-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4854-116">Not supported.</span></span> |
| <span data-ttu-id="d4854-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4854-117">Application</span></span> | <span data-ttu-id="d4854-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4854-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4854-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4854-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d4854-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4854-120">Request headers</span></span>

| <span data-ttu-id="d4854-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d4854-121">Name</span></span> | <span data-ttu-id="d4854-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4854-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="d4854-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4854-123">Authorization</span></span> | <span data-ttu-id="d4854-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d4854-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4854-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4854-125">Request body</span></span>

<span data-ttu-id="d4854-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4854-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4854-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4854-127">Response</span></span>

<span data-ttu-id="d4854-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4854-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4854-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4854-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4854-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4854-131">Request</span></span>

<span data-ttu-id="d4854-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4854-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d4854-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4854-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="d4854-134">C#</span><span class="sxs-lookup"><span data-stu-id="d4854-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4854-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4854-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4854-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4854-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4854-137">Java</span><span class="sxs-lookup"><span data-stu-id="d4854-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4854-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4854-138">Response</span></span>

<span data-ttu-id="d4854-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4854-139">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


