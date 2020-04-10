---
title: Cancelar governanceRoleAssignmentRequest
description: Cancelar uma governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 8179fa2d2bd1e8f52df9aa09bac5a965812e2122
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218882"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="4487b-103">Cancelar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="4487b-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="4487b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4487b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4487b-105">Cancelar uma [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="4487b-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4487b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4487b-106">Permissions</span></span>
<span data-ttu-id="4487b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4487b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4487b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4487b-109">Permission type</span></span>      | <span data-ttu-id="4487b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="4487b-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4487b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4487b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4487b-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4487b-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="4487b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4487b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4487b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4487b-114">Not supported.</span></span>    |
|<span data-ttu-id="4487b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4487b-115">Application</span></span> | <span data-ttu-id="4487b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4487b-116">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="4487b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4487b-117">Optional query parameters</span></span>
<span data-ttu-id="4487b-118">Este **método não oferece suporte a** parâmetros de [consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4487b-118">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="4487b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4487b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="4487b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4487b-120">Request headers</span></span>
| <span data-ttu-id="4487b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4487b-121">Name</span></span>       | <span data-ttu-id="4487b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4487b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4487b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4487b-123">Authorization</span></span>  | <span data-ttu-id="4487b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4487b-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4487b-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="4487b-126">Content-type</span></span>  | <span data-ttu-id="4487b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4487b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4487b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4487b-128">Request body</span></span>
<span data-ttu-id="4487b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4487b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4487b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4487b-130">Response</span></span>
<span data-ttu-id="4487b-p103">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4487b-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="4487b-133">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="4487b-133">Error codes</span></span>
<span data-ttu-id="4487b-134">Essa API segue o padrão de códigos HTTP.</span><span class="sxs-lookup"><span data-stu-id="4487b-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="4487b-135">Além disso, os códigos de erro personalizados são mostrados abaixo.</span><span class="sxs-lookup"><span data-stu-id="4487b-135">Besides, the custom error codes are shown below.</span></span>
| <span data-ttu-id="4487b-136">Código de erro</span><span class="sxs-lookup"><span data-stu-id="4487b-136">Error code</span></span> | <span data-ttu-id="4487b-137">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="4487b-137">Error message</span></span> | <span data-ttu-id="4487b-138">Detalhes</span><span class="sxs-lookup"><span data-stu-id="4487b-138">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="4487b-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4487b-139">400 BadRequest</span></span> | <span data-ttu-id="4487b-140">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="4487b-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="4487b-141">O governanceRoleAssignmentRequest não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="4487b-141">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="4487b-142">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="4487b-142">400 BadRequest</span></span> | <span data-ttu-id="4487b-143">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="4487b-143">RequestCannotBeCancelled</span></span> | <span data-ttu-id="4487b-144">Somente as solicitações no status `Granted`de `PendingApproval`, `PendingApprovalProvisioning` e `PendingAdminDecision` podem ser canceladas.</span><span class="sxs-lookup"><span data-stu-id="4487b-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="4487b-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4487b-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="4487b-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4487b-146">Request</span></span>
<span data-ttu-id="4487b-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4487b-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4487b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="4487b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="4487b-149">C#</span><span class="sxs-lookup"><span data-stu-id="4487b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4487b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4487b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4487b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4487b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4487b-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="4487b-152">Response</span></span>
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
