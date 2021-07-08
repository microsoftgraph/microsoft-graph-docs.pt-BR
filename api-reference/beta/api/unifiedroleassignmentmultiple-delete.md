---
title: Excluir unifiedRoleAssignmentMultiple
description: Exclua um objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 476f9a0dc37d919ea2977602298a4b438bbd1956
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334567"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="add26-103">Excluir unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="add26-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="add26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="add26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="add26-105">[Exclua um objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) de um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="add26-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="add26-106">Isso é aplicável a um aplicativo RBAC que oferece suporte a várias entidades e escopos.</span><span class="sxs-lookup"><span data-stu-id="add26-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="add26-107">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="add26-107">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="add26-108">cloud PC</span><span class="sxs-lookup"><span data-stu-id="add26-108">cloud PC</span></span> 
- <span data-ttu-id="add26-109">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="add26-109">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="add26-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="add26-110">Permissions</span></span>

<span data-ttu-id="add26-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="add26-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="add26-112">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="add26-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="add26-113">Para provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="add26-113">For Cloud PC provider</span></span>

|<span data-ttu-id="add26-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="add26-114">Permission type</span></span>      | <span data-ttu-id="add26-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="add26-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="add26-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="add26-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="add26-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="add26-117">CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="add26-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="add26-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="add26-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="add26-119">Not supported.</span></span>    |
|<span data-ttu-id="add26-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="add26-120">Application</span></span> | <span data-ttu-id="add26-121">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="add26-121">CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="add26-122">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="add26-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="add26-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="add26-123">Permission type</span></span>      | <span data-ttu-id="add26-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="add26-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="add26-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="add26-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="add26-126">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="add26-126">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="add26-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="add26-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="add26-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="add26-128">Not supported.</span></span>    |
|<span data-ttu-id="add26-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="add26-129">Application</span></span> | <span data-ttu-id="add26-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="add26-130">DeviceManagementRBAC.ReadWrite.All</span></span> |



## <a name="http-request"></a><span data-ttu-id="add26-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="add26-131">HTTP request</span></span>

<span data-ttu-id="add26-132">Para excluir um unifiedRoleAssignmentMultiple para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="add26-132">To delete a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="add26-133">Para excluir um unifiedRoleAssignmentMultiple para um provedor do Intune:</span><span class="sxs-lookup"><span data-stu-id="add26-133">To delete a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="add26-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="add26-134">Request headers</span></span>

| <span data-ttu-id="add26-135">Nome</span><span class="sxs-lookup"><span data-stu-id="add26-135">Name</span></span> | <span data-ttu-id="add26-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="add26-136">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="add26-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="add26-137">Authorization</span></span> | <span data-ttu-id="add26-138">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="add26-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="add26-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="add26-139">Request body</span></span>

<span data-ttu-id="add26-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="add26-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="add26-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="add26-141">Response</span></span>

<span data-ttu-id="add26-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="add26-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="add26-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="add26-144">Example</span></span>

### <a name="example-1-delete-a-unifiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="add26-145">Exemplo 1: Excluir um unifiedRoleAssignmentMultiple em um provedor do Intune</span><span class="sxs-lookup"><span data-stu-id="add26-145">Example 1: Delete a unifiedRoleAssignmentMultiple in an Intune provider</span></span>

### <a name="request"></a><span data-ttu-id="add26-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="add26-146">Request</span></span>

<span data-ttu-id="add26-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="add26-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="add26-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="add26-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="add26-149">C#</span><span class="sxs-lookup"><span data-stu-id="add26-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="add26-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="add26-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="add26-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="add26-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="add26-152">Java</span><span class="sxs-lookup"><span data-stu-id="add26-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="add26-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="add26-153">Response</span></span>

<span data-ttu-id="add26-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="add26-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-delete-a-unifiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="add26-155">Exemplo 2: Excluir um unifiedRoleAssignmentMultiple em um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="add26-155">Example 2: Delete a unifiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="add26-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="add26-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="add26-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="add26-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple_cloudpc"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/id
```
# <a name="c"></a>[<span data-ttu-id="add26-158">C#</span><span class="sxs-lookup"><span data-stu-id="add26-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="add26-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="add26-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="add26-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="add26-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="add26-161">Java</span><span class="sxs-lookup"><span data-stu-id="add26-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="add26-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="add26-162">Response</span></span>

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


