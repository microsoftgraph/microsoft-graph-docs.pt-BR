---
title: Excluir unifiedRoleAssignmentMultiple
description: Excluir um objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7119135f1019e2b1309abdaebbda2dd9ac960f09
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806379"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="e439f-103">Excluir unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="e439f-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="e439f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e439f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e439f-105">Excluir um objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="e439f-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="e439f-106">Isso se aplica a um aplicativo RBAC que oferece suporte a várias entidades de segurança e escopos.</span><span class="sxs-lookup"><span data-stu-id="e439f-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="e439f-107">O Microsoft Intune é um aplicativo desse tipo.</span><span class="sxs-lookup"><span data-stu-id="e439f-107">Microsoft Intune is such an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="e439f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e439f-108">Permissions</span></span>

<span data-ttu-id="e439f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e439f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e439f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e439f-111">Permission type</span></span> | <span data-ttu-id="e439f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e439f-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="e439f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e439f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e439f-114">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="e439f-114">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="e439f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e439f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e439f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e439f-116">Not supported.</span></span> |
| <span data-ttu-id="e439f-117">Application</span><span class="sxs-lookup"><span data-stu-id="e439f-117">Application</span></span> | <span data-ttu-id="e439f-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="e439f-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="e439f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e439f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e439f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e439f-120">Request headers</span></span>

| <span data-ttu-id="e439f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e439f-121">Name</span></span> | <span data-ttu-id="e439f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e439f-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e439f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e439f-123">Authorization</span></span> | <span data-ttu-id="e439f-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e439f-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e439f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e439f-125">Request body</span></span>

<span data-ttu-id="e439f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e439f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e439f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e439f-127">Response</span></span>

<span data-ttu-id="e439f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e439f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e439f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e439f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e439f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e439f-131">Request</span></span>

<span data-ttu-id="e439f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e439f-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e439f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e439f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="e439f-134">C#</span><span class="sxs-lookup"><span data-stu-id="e439f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e439f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e439f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e439f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e439f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e439f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e439f-137">Response</span></span>

<span data-ttu-id="e439f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e439f-138">The following is an example of the response.</span></span>

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
