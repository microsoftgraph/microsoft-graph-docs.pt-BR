---
title: Cancelar governanceRoleAssignmentRequest
description: Cancelar uma governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 942ff054ab3465077bf4ace0f267121e8b7ce8e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991128"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="f602a-103">Cancelar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f602a-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="f602a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f602a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f602a-105">Cancelar uma [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f602a-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f602a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f602a-106">Permissions</span></span>
<span data-ttu-id="f602a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f602a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f602a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f602a-109">Permission type</span></span>      | <span data-ttu-id="f602a-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f602a-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f602a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f602a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f602a-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f602a-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f602a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f602a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f602a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f602a-114">Not supported.</span></span>    |
|<span data-ttu-id="f602a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f602a-115">Application</span></span> | <span data-ttu-id="f602a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f602a-116">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="f602a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f602a-117">Optional query parameters</span></span>
<span data-ttu-id="f602a-118">Este **método não oferece suporte a** parâmetros de [consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f602a-118">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="f602a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f602a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="f602a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f602a-120">Request headers</span></span>
| <span data-ttu-id="f602a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f602a-121">Name</span></span>       | <span data-ttu-id="f602a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f602a-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f602a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f602a-123">Authorization</span></span>  | <span data-ttu-id="f602a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f602a-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f602a-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f602a-126">Content-type</span></span>  | <span data-ttu-id="f602a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f602a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f602a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f602a-128">Request body</span></span>
<span data-ttu-id="f602a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f602a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f602a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f602a-130">Response</span></span>
<span data-ttu-id="f602a-p103">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f602a-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="f602a-133">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="f602a-133">Error codes</span></span>
<span data-ttu-id="f602a-134">Essa API segue o padrão de códigos HTTP.</span><span class="sxs-lookup"><span data-stu-id="f602a-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="f602a-135">Além disso, os códigos de erro personalizados são mostrados abaixo.</span><span class="sxs-lookup"><span data-stu-id="f602a-135">Besides, the custom error codes are shown below.</span></span>
| <span data-ttu-id="f602a-136">Código de erro</span><span class="sxs-lookup"><span data-stu-id="f602a-136">Error code</span></span> | <span data-ttu-id="f602a-137">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="f602a-137">Error message</span></span> | <span data-ttu-id="f602a-138">Detalhes</span><span class="sxs-lookup"><span data-stu-id="f602a-138">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="f602a-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f602a-139">400 BadRequest</span></span> | <span data-ttu-id="f602a-140">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="f602a-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="f602a-141">O governanceRoleAssignmentRequest não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="f602a-141">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="f602a-142">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f602a-142">400 BadRequest</span></span> | <span data-ttu-id="f602a-143">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="f602a-143">RequestCannotBeCancelled</span></span> | <span data-ttu-id="f602a-144">Somente as solicitações no status `Granted` de `PendingApproval` , `PendingApprovalProvisioning` e `PendingAdminDecision` podem ser canceladas.</span><span class="sxs-lookup"><span data-stu-id="f602a-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="f602a-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f602a-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="f602a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f602a-146">Request</span></span>
<span data-ttu-id="f602a-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f602a-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f602a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f602a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="f602a-149">C#</span><span class="sxs-lookup"><span data-stu-id="f602a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f602a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f602a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f602a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f602a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f602a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="f602a-152">Response</span></span>
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


