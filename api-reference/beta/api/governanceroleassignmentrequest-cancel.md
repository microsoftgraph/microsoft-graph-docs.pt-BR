---
title: Cancelar governanceRoleAssignmentRequest
description: Cancelar uma governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: 8ba825cc94dfc6108ee04706e34ca30990a36ed3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859126"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="eadc7-103">Cancelar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="eadc7-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eadc7-104">Cancelar uma [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="eadc7-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eadc7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eadc7-105">Permissions</span></span>
<span data-ttu-id="eadc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eadc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eadc7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eadc7-108">Permission type</span></span>      | <span data-ttu-id="eadc7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="eadc7-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eadc7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eadc7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eadc7-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="eadc7-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="eadc7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eadc7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eadc7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eadc7-113">Not supported.</span></span>    |
|<span data-ttu-id="eadc7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eadc7-114">Application</span></span> | <span data-ttu-id="eadc7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eadc7-115">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="eadc7-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eadc7-116">Optional query parameters</span></span>
<span data-ttu-id="eadc7-117">Este método não \*\*\*\* oferece suporte a [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="eadc7-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="eadc7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eadc7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="eadc7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eadc7-119">Request headers</span></span>
| <span data-ttu-id="eadc7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eadc7-120">Name</span></span>       | <span data-ttu-id="eadc7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eadc7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eadc7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eadc7-122">Authorization</span></span>  | <span data-ttu-id="eadc7-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="eadc7-123">Bearer {code}</span></span>|
| <span data-ttu-id="eadc7-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="eadc7-124">Content-type</span></span>  | <span data-ttu-id="eadc7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eadc7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eadc7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eadc7-126">Request body</span></span>
<span data-ttu-id="eadc7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eadc7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eadc7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eadc7-128">Response</span></span>
<span data-ttu-id="eadc7-p102">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eadc7-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="eadc7-131">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="eadc7-131">Error codes</span></span>
<span data-ttu-id="eadc7-132">Essa API segue o padrão de códigos HTTP.</span><span class="sxs-lookup"><span data-stu-id="eadc7-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="eadc7-133">Além disso, os códigos de erro personalizados são mostrados abaixo.</span><span class="sxs-lookup"><span data-stu-id="eadc7-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="eadc7-134">Código de erro</span><span class="sxs-lookup"><span data-stu-id="eadc7-134">Error code</span></span>     | <span data-ttu-id="eadc7-135">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="eadc7-135">Error message</span></span>              | <span data-ttu-id="eadc7-136">Detalhes</span><span class="sxs-lookup"><span data-stu-id="eadc7-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="eadc7-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eadc7-137">400 BadRequest</span></span> | <span data-ttu-id="eadc7-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="eadc7-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="eadc7-139">O governanceRoleAssignmentRequest não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="eadc7-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="eadc7-140">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eadc7-140">400 BadRequest</span></span> | <span data-ttu-id="eadc7-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="eadc7-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="eadc7-142">Somente as solicitações no status `Granted`de `PendingApproval`, `PendingApprovalProvisioning` e `PendingAdminDecision` podem ser canceladas.</span><span class="sxs-lookup"><span data-stu-id="eadc7-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="eadc7-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eadc7-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eadc7-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eadc7-144">Request</span></span>
<span data-ttu-id="eadc7-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eadc7-145">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eadc7-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="eadc7-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eadc7-147">C#</span><span class="sxs-lookup"><span data-stu-id="eadc7-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eadc7-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="eadc7-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eadc7-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eadc7-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eadc7-150">Java</span><span class="sxs-lookup"><span data-stu-id="eadc7-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eadc7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="eadc7-151">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
