---
title: Atualizar unifiedRoleAssignmentMultiple
description: Atualize um novo objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3423c216e9b0c5b6928d0473c1e7db021e1344c9
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334490"
---
# <a name="update-unifiedroleassignmentmultiple"></a><span data-ttu-id="e2256-103">Atualizar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="e2256-103">Update unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="e2256-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2256-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2256-105">Atualize um objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) existente de um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="e2256-105">Update an existing [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="e2256-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="e2256-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="e2256-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="e2256-107">cloud PC</span></span> 
- <span data-ttu-id="e2256-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="e2256-108">device management (Intune)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

<span data-ttu-id="e2256-109">Por outro lado, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) não dá suporte à atualização.</span><span class="sxs-lookup"><span data-stu-id="e2256-109">In contrast, [unifiedRoleAssignment](../resources/unifiedroleassignment.md) does not support update.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2256-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2256-110">Permissions</span></span>

<span data-ttu-id="e2256-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e2256-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="e2256-112">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2256-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="e2256-113">Para provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="e2256-113">For Cloud PC provider</span></span>

|<span data-ttu-id="e2256-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2256-114">Permission type</span></span>      | <span data-ttu-id="e2256-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2256-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2256-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2256-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="e2256-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2256-117">CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="e2256-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2256-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2256-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2256-119">Not supported.</span></span>    |
|<span data-ttu-id="e2256-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2256-120">Application</span></span> | <span data-ttu-id="e2256-121">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2256-121">CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="e2256-122">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="e2256-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="e2256-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2256-123">Permission type</span></span>      | <span data-ttu-id="e2256-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2256-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2256-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2256-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="e2256-126">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2256-126">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="e2256-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2256-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2256-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2256-128">Not supported.</span></span>    |
|<span data-ttu-id="e2256-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2256-129">Application</span></span> | <span data-ttu-id="e2256-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2256-130">DeviceManagementRBAC.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="e2256-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2256-131">HTTP request</span></span>

<span data-ttu-id="e2256-132">Para atualizar um unfiedRoleAssignmentMultiple existente para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="e2256-132">To update an existing unfiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="e2256-133">Para atualizar um unfiedRoleAssignmentMultiple existente para um provedor do Intune:</span><span class="sxs-lookup"><span data-stu-id="e2256-133">To update an existing unfiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="e2256-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2256-134">Request headers</span></span>

| <span data-ttu-id="e2256-135">Nome</span><span class="sxs-lookup"><span data-stu-id="e2256-135">Name</span></span> | <span data-ttu-id="e2256-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2256-136">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e2256-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2256-137">Authorization</span></span> | <span data-ttu-id="e2256-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2256-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2256-140">Content-type</span><span class="sxs-lookup"><span data-stu-id="e2256-140">Content-type</span></span> | <span data-ttu-id="e2256-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2256-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2256-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2256-143">Request body</span></span>

<span data-ttu-id="e2256-144">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e2256-144">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e2256-145">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e2256-145">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e2256-146">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e2256-146">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="e2256-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2256-147">Response</span></span>

<span data-ttu-id="e2256-148">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2256-148">If successful, this method returns a `200 OK` response code and an updated [unifiedAssignmentMultiple](../resources/unifiedroleassignmentMultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2256-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2256-149">Example</span></span>

### <a name="example-1-update-an-existing-unfiedroleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="e2256-150">Exemplo 1: atualizar um unfiedRoleAssignmentMultiple existente em um provedor do Intune</span><span class="sxs-lookup"><span data-stu-id="e2256-150">Example 1: Update an existing unfiedRoleAssignmentMultiple in an Intune provider</span></span>
### <a name="request"></a><span data-ttu-id="e2256-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2256-151">Request</span></span>

<span data-ttu-id="e2256-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2256-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e2256-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2256-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
Content-type: application/json

{ 
    "principalIds": ["0aeec2c1-fee7-4e02-b534-6f920d25b300", "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"]
}
```
# <a name="c"></a>[<span data-ttu-id="e2256-154">C#</span><span class="sxs-lookup"><span data-stu-id="e2256-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2256-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2256-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2256-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2256-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2256-157">Java</span><span class="sxs-lookup"><span data-stu-id="e2256-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2256-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2256-158">Response</span></span>

<span data-ttu-id="e2256-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e2256-159">The following is an example of the response.</span></span>
> <span data-ttu-id="e2256-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2256-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK

```

## <a name="example-2-update-an-existing-unfiedroleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="e2256-161">Exemplo 2: atualizar um unfiedRoleAssignmentMultiple existente em um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="e2256-161">Example 2: update an existing unfiedRoleAssignmentMultiple in a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="e2256-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2256-162">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e2256-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2256-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignmentmultiple_from_rbacapplication_cloudpc"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096
Content-type: application/json

{
    "displayName": "NewName",
    "description": "A new roleAssignment"
}
```
# <a name="c"></a>[<span data-ttu-id="e2256-164">C#</span><span class="sxs-lookup"><span data-stu-id="e2256-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2256-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2256-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2256-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2256-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2256-167">Java</span><span class="sxs-lookup"><span data-stu-id="e2256-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e2256-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2256-168">Response</span></span>

> <span data-ttu-id="e2256-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2256-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "description": "A new roleAssignment",
    "displayName": "NewName",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "0aeec2c1-fee7-4e02-b534-6f920d25b300",
        "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


