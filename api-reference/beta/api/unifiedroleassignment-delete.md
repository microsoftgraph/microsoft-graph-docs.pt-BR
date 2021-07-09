---
title: Excluir unifiedRoleAssignment
description: Exclua um objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 01ce2f1aa786c0f62147a370c00f6aed4d9d0bc6
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351031"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="98f50-103">Excluir unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="98f50-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="98f50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98f50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98f50-105">[Exclua um objeto unifiedRoleAssignment.](../resources/unifiedRoleAssignment.md)</span><span class="sxs-lookup"><span data-stu-id="98f50-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="98f50-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="98f50-106">Permissions</span></span>

<span data-ttu-id="98f50-107">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="98f50-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="98f50-108">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98f50-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="98f50-109">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="98f50-109">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="98f50-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98f50-110">Permission type</span></span>      | <span data-ttu-id="98f50-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98f50-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98f50-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98f50-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="98f50-113">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="98f50-113">RoleManagement.ReadWrite.Directory</span></span>   |
|<span data-ttu-id="98f50-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98f50-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98f50-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98f50-115">Not supported.</span></span>    |
|<span data-ttu-id="98f50-116">Application</span><span class="sxs-lookup"><span data-stu-id="98f50-116">Application</span></span> | <span data-ttu-id="98f50-117">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="98f50-117">RoleManagement.ReadWrite.Directory</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="98f50-118">Para provedor de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="98f50-118">For Entitlement management provider</span></span>

|<span data-ttu-id="98f50-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98f50-119">Permission type</span></span>      | <span data-ttu-id="98f50-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98f50-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98f50-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98f50-121">Delegated (work or school account)</span></span> |  <span data-ttu-id="98f50-122">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f50-122">EntitlementManagement.ReadWrite.All</span></span>  |
|<span data-ttu-id="98f50-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98f50-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98f50-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98f50-124">Not supported.</span></span>    |
|<span data-ttu-id="98f50-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98f50-125">Application</span></span> | <span data-ttu-id="98f50-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98f50-126">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98f50-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98f50-127">HTTP request</span></span>

<span data-ttu-id="98f50-128">Remover uma atribuição de função de um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="98f50-128">Remove a role assignment from a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="98f50-129">Remova uma atribuição de função do provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="98f50-129">Remove a role assignment from the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/entitlementManagement/roleAssignments/{id}
```


## <a name="request-headers"></a><span data-ttu-id="98f50-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98f50-130">Request headers</span></span>

| <span data-ttu-id="98f50-131">Nome</span><span class="sxs-lookup"><span data-stu-id="98f50-131">Name</span></span>          | <span data-ttu-id="98f50-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="98f50-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="98f50-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="98f50-133">Authorization</span></span> | <span data-ttu-id="98f50-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="98f50-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="98f50-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98f50-135">Request body</span></span>

<span data-ttu-id="98f50-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="98f50-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98f50-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="98f50-137">Response</span></span>

<span data-ttu-id="98f50-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98f50-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98f50-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98f50-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="98f50-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98f50-141">Request</span></span>

<span data-ttu-id="98f50-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="98f50-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98f50-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="98f50-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="98f50-144">C#</span><span class="sxs-lookup"><span data-stu-id="98f50-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98f50-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98f50-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98f50-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98f50-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98f50-147">Java</span><span class="sxs-lookup"><span data-stu-id="98f50-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98f50-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="98f50-148">Response</span></span>

<span data-ttu-id="98f50-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="98f50-149">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


