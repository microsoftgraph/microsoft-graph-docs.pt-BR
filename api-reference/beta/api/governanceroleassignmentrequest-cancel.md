---
title: Cancelar governanceRoleAssignmentRequest
description: Cancelar uma governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 03fe3b433b3b10aa2e7c98993f6f1a14c3a1fccb
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635016"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="11c67-103">Cancelar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="11c67-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="11c67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11c67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11c67-105">Cancelar uma [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="11c67-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="11c67-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11c67-106">Permissions</span></span>
<span data-ttu-id="11c67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="11c67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="11c67-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="11c67-109">Azure resources</span></span>

| <span data-ttu-id="11c67-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11c67-110">Permission type</span></span> | <span data-ttu-id="11c67-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="11c67-111">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="11c67-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11c67-112">Delegated (work or school account)</span></span> | <span data-ttu-id="11c67-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="11c67-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="11c67-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11c67-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11c67-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c67-115">Not supported.</span></span> |
| <span data-ttu-id="11c67-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11c67-116">Application</span></span> | <span data-ttu-id="11c67-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c67-117">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="11c67-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="11c67-118">Azure AD</span></span>

| <span data-ttu-id="11c67-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11c67-119">Permission type</span></span> | <span data-ttu-id="11c67-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="11c67-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="11c67-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11c67-121">Delegated (work or school account)</span></span> | <span data-ttu-id="11c67-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="11c67-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="11c67-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11c67-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11c67-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c67-124">Not supported.</span></span> |
| <span data-ttu-id="11c67-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11c67-125">Application</span></span> | <span data-ttu-id="11c67-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c67-126">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="11c67-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="11c67-127">Groups</span></span>

|<span data-ttu-id="11c67-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11c67-128">Permission type</span></span> | <span data-ttu-id="11c67-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="11c67-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="11c67-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11c67-130">Delegated (work or school account)</span></span> | <span data-ttu-id="11c67-131">PrivilegedAccess. ReadWrite. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="11c67-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="11c67-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11c67-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11c67-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c67-133">Not supported.</span></span> |
| <span data-ttu-id="11c67-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11c67-134">Application</span></span> | <span data-ttu-id="11c67-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c67-135">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="11c67-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="11c67-136">Optional query parameters</span></span>
<span data-ttu-id="11c67-137">Este **método não oferece suporte a** parâmetros de [consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="11c67-137">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="11c67-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11c67-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="11c67-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11c67-139">Request headers</span></span>
| <span data-ttu-id="11c67-140">Nome</span><span class="sxs-lookup"><span data-stu-id="11c67-140">Name</span></span>       | <span data-ttu-id="11c67-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="11c67-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11c67-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="11c67-142">Authorization</span></span>  | <span data-ttu-id="11c67-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11c67-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="11c67-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="11c67-145">Content-type</span></span>  | <span data-ttu-id="11c67-146">application/json</span><span class="sxs-lookup"><span data-stu-id="11c67-146">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11c67-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11c67-147">Request body</span></span>
<span data-ttu-id="11c67-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11c67-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11c67-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c67-149">Response</span></span>
<span data-ttu-id="11c67-p103">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11c67-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="11c67-152">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="11c67-152">Error codes</span></span>
<span data-ttu-id="11c67-153">Essa API segue o padrão de códigos HTTP.</span><span class="sxs-lookup"><span data-stu-id="11c67-153">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="11c67-154">Além disso, os códigos de erro personalizados são mostrados abaixo.</span><span class="sxs-lookup"><span data-stu-id="11c67-154">Besides, the custom error codes are shown below.</span></span>
| <span data-ttu-id="11c67-155">Código de erro</span><span class="sxs-lookup"><span data-stu-id="11c67-155">Error code</span></span> | <span data-ttu-id="11c67-156">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="11c67-156">Error message</span></span> | <span data-ttu-id="11c67-157">Detalhes</span><span class="sxs-lookup"><span data-stu-id="11c67-157">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="11c67-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="11c67-158">400 BadRequest</span></span> | <span data-ttu-id="11c67-159">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="11c67-159">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="11c67-160">O governanceRoleAssignmentRequest não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="11c67-160">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="11c67-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="11c67-161">400 BadRequest</span></span> | <span data-ttu-id="11c67-162">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="11c67-162">RequestCannotBeCancelled</span></span> | <span data-ttu-id="11c67-163">Somente as solicitações no status `Granted` de `PendingApproval` , `PendingApprovalProvisioning` e `PendingAdminDecision` podem ser canceladas.</span><span class="sxs-lookup"><span data-stu-id="11c67-163">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="11c67-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11c67-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="11c67-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11c67-165">Request</span></span>
<span data-ttu-id="11c67-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11c67-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11c67-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="11c67-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="11c67-168">C#</span><span class="sxs-lookup"><span data-stu-id="11c67-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11c67-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11c67-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11c67-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11c67-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11c67-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c67-171">Response</span></span>
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


