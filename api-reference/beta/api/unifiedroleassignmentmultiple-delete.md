---
title: Excluir unifiedRoleAssignmentMultiple
description: Exclua um objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 14ae5e8c899378e76fb201856bea2929a0ba3168
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870056"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="57c65-103">Excluir unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="57c65-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="57c65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57c65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57c65-105">[Exclua um objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) de um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="57c65-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="57c65-106">Isso é aplicável a um aplicativo RBAC que oferece suporte a várias entidades e escopos.</span><span class="sxs-lookup"><span data-stu-id="57c65-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="57c65-107">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="57c65-107">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="57c65-108">cloud PC</span><span class="sxs-lookup"><span data-stu-id="57c65-108">cloud PC</span></span> 
- <span data-ttu-id="57c65-109">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="57c65-109">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="57c65-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="57c65-110">Permissions</span></span>

<span data-ttu-id="57c65-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="57c65-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="57c65-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57c65-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="57c65-113">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="57c65-113">Supported provider</span></span>      | <span data-ttu-id="57c65-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57c65-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="57c65-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57c65-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57c65-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57c65-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="57c65-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="57c65-117">Cloud PC</span></span> | <span data-ttu-id="57c65-118">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57c65-118">CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="57c65-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57c65-119">Not supported.</span></span> | <span data-ttu-id="57c65-120">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57c65-120">CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="57c65-121">Intune</span><span class="sxs-lookup"><span data-stu-id="57c65-121">Intune</span></span> | <span data-ttu-id="57c65-122">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57c65-122">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="57c65-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57c65-123">Not supported.</span></span>| <span data-ttu-id="57c65-124">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57c65-124">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57c65-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57c65-125">HTTP request</span></span>

<span data-ttu-id="57c65-126">Para excluir um unifiedRoleAssignmentMultiple para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="57c65-126">To delete a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="57c65-127">Para excluir um unifiedRoleAssignmentMultiple para um provedor do Intune:</span><span class="sxs-lookup"><span data-stu-id="57c65-127">To delete a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="57c65-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57c65-128">Request headers</span></span>

| <span data-ttu-id="57c65-129">Nome</span><span class="sxs-lookup"><span data-stu-id="57c65-129">Name</span></span> | <span data-ttu-id="57c65-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="57c65-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="57c65-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="57c65-131">Authorization</span></span> | <span data-ttu-id="57c65-132">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="57c65-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="57c65-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57c65-133">Request body</span></span>

<span data-ttu-id="57c65-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57c65-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57c65-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="57c65-135">Response</span></span>

<span data-ttu-id="57c65-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57c65-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57c65-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57c65-138">Example</span></span>

### <a name="example-1-delete-a-unifiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="57c65-139">Exemplo 1: Excluir um unifiedRoleAssignmentMultiple em um provedor do Intune</span><span class="sxs-lookup"><span data-stu-id="57c65-139">Example 1: Delete a unifiedRoleAssignmentMultiple in an Intune provider</span></span>

### <a name="request"></a><span data-ttu-id="57c65-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57c65-140">Request</span></span>

<span data-ttu-id="57c65-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="57c65-141">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="57c65-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="57c65-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="57c65-143">C#</span><span class="sxs-lookup"><span data-stu-id="57c65-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57c65-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57c65-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57c65-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57c65-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57c65-146">Java</span><span class="sxs-lookup"><span data-stu-id="57c65-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57c65-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="57c65-147">Response</span></span>

<span data-ttu-id="57c65-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="57c65-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-delete-a-unifiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="57c65-149">Exemplo 2: Excluir um unifiedRoleAssignmentMultiple em um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="57c65-149">Example 2: Delete a unifiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="57c65-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57c65-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="57c65-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="57c65-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple_cloudpc"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/id
```
# <a name="c"></a>[<span data-ttu-id="57c65-152">C#</span><span class="sxs-lookup"><span data-stu-id="57c65-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57c65-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57c65-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57c65-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57c65-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57c65-155">Java</span><span class="sxs-lookup"><span data-stu-id="57c65-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="57c65-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="57c65-156">Response</span></span>

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


