---
title: Excluir unifiedRoleAssignment
description: Exclua um objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 96bff141cc3f4dfb779335100a49a8fdf99edb00
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317067"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="81afb-103">Excluir unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81afb-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="81afb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81afb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81afb-105">[Exclua um objeto unifiedRoleAssignment.](../resources/unifiedRoleAssignment.md)</span><span class="sxs-lookup"><span data-stu-id="81afb-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81afb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81afb-106">Permissions</span></span>

<span data-ttu-id="81afb-107">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="81afb-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="81afb-108">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81afb-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81afb-109">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="81afb-109">Supported provider</span></span>      | <span data-ttu-id="81afb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81afb-110">Delegated (work or school account)</span></span>  | <span data-ttu-id="81afb-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81afb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81afb-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81afb-112">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="81afb-113">Diretório</span><span class="sxs-lookup"><span data-stu-id="81afb-113">Directory</span></span> | <span data-ttu-id="81afb-114">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="81afb-114">RoleManagement.ReadWrite.Directory</span></span> | <span data-ttu-id="81afb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81afb-115">Not supported.</span></span>| <span data-ttu-id="81afb-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="81afb-116">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="81afb-117">Gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="81afb-117">Entitlement management</span></span> | <span data-ttu-id="81afb-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81afb-118">EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="81afb-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81afb-119">Not supported.</span></span> | <span data-ttu-id="81afb-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81afb-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81afb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81afb-121">HTTP request</span></span>

<span data-ttu-id="81afb-122">Remover uma atribuição de função de um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="81afb-122">Remove a role assignment from a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="81afb-123">Remova uma atribuição de função do provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="81afb-123">Remove a role assignment from the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/entitlementManagement/roleAssignments/{id}
```


## <a name="request-headers"></a><span data-ttu-id="81afb-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81afb-124">Request headers</span></span>

| <span data-ttu-id="81afb-125">Nome</span><span class="sxs-lookup"><span data-stu-id="81afb-125">Name</span></span>          | <span data-ttu-id="81afb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="81afb-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="81afb-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="81afb-127">Authorization</span></span> | <span data-ttu-id="81afb-128">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="81afb-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="81afb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81afb-129">Request body</span></span>

<span data-ttu-id="81afb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81afb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81afb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="81afb-131">Response</span></span>

<span data-ttu-id="81afb-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81afb-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81afb-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81afb-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="81afb-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81afb-135">Request</span></span>

<span data-ttu-id="81afb-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81afb-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81afb-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="81afb-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="81afb-138">C#</span><span class="sxs-lookup"><span data-stu-id="81afb-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81afb-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81afb-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81afb-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81afb-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81afb-141">Java</span><span class="sxs-lookup"><span data-stu-id="81afb-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81afb-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="81afb-142">Response</span></span>

<span data-ttu-id="81afb-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81afb-143">The following is an example of the response.</span></span>

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


