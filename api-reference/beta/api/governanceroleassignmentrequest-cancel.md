---
title: Cancelar governanceRoleAssignmentRequest
description: Cancelar uma governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: e2f245766c826b8776504f0835a79a33b370aaba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421120"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="a00e0-103">Cancelar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a00e0-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="a00e0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a00e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a00e0-105">Cancelar uma [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a00e0-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a00e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a00e0-106">Permissions</span></span>
<span data-ttu-id="a00e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a00e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a00e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a00e0-109">Permission type</span></span>      | <span data-ttu-id="a00e0-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a00e0-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a00e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a00e0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a00e0-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a00e0-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a00e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a00e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a00e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a00e0-114">Not supported.</span></span>    |
|<span data-ttu-id="a00e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a00e0-115">Application</span></span> | <span data-ttu-id="a00e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a00e0-116">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="a00e0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a00e0-117">Optional query parameters</span></span>
<span data-ttu-id="a00e0-118">Este **método não oferece suporte a** parâmetros de [consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a00e0-118">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="a00e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a00e0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="a00e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a00e0-120">Request headers</span></span>
| <span data-ttu-id="a00e0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a00e0-121">Name</span></span>       | <span data-ttu-id="a00e0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a00e0-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a00e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a00e0-123">Authorization</span></span>  | <span data-ttu-id="a00e0-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a00e0-124">Bearer {code}</span></span>|
| <span data-ttu-id="a00e0-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="a00e0-125">Content-type</span></span>  | <span data-ttu-id="a00e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a00e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a00e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a00e0-127">Request body</span></span>
<span data-ttu-id="a00e0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a00e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a00e0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a00e0-129">Response</span></span>
<span data-ttu-id="a00e0-p102">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a00e0-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="a00e0-132">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="a00e0-132">Error codes</span></span>
<span data-ttu-id="a00e0-133">Essa API segue o padrão de códigos HTTP.</span><span class="sxs-lookup"><span data-stu-id="a00e0-133">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="a00e0-134">Além disso, os códigos de erro personalizados são mostrados abaixo.</span><span class="sxs-lookup"><span data-stu-id="a00e0-134">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="a00e0-135">Código de erro</span><span class="sxs-lookup"><span data-stu-id="a00e0-135">Error code</span></span>     | <span data-ttu-id="a00e0-136">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="a00e0-136">Error message</span></span>              | <span data-ttu-id="a00e0-137">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a00e0-137">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="a00e0-138">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a00e0-138">400 BadRequest</span></span> | <span data-ttu-id="a00e0-139">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="a00e0-139">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="a00e0-140">O governanceRoleAssignmentRequest não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="a00e0-140">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="a00e0-141">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a00e0-141">400 BadRequest</span></span> | <span data-ttu-id="a00e0-142">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="a00e0-142">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="a00e0-143">Somente as solicitações no status `Granted`de `PendingApproval`, `PendingApprovalProvisioning` e `PendingAdminDecision` podem ser canceladas.</span><span class="sxs-lookup"><span data-stu-id="a00e0-143">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="a00e0-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a00e0-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a00e0-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a00e0-145">Request</span></span>
<span data-ttu-id="a00e0-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a00e0-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a00e0-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="a00e0-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="a00e0-148">C#</span><span class="sxs-lookup"><span data-stu-id="a00e0-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a00e0-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a00e0-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a00e0-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a00e0-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a00e0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a00e0-151">Response</span></span>
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
