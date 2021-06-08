---
title: Cancelar governançaRoleAssignmentRequest
description: Cancele uma governançaRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 624302e735eebf3fbbdf477636176a5e7f414bfe
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786984"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="6fa4d-103">Cancelar governançaRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="6fa4d-103">Cancel governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="6fa4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fa4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fa4d-105">Cancele [um governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="6fa4d-105">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6fa4d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6fa4d-106">Permissions</span></span>
<span data-ttu-id="6fa4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="6fa4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="6fa4d-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="6fa4d-109">Azure resources</span></span>

| <span data-ttu-id="6fa4d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fa4d-110">Permission type</span></span> | <span data-ttu-id="6fa4d-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="6fa4d-111">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="6fa4d-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fa4d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6fa4d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6fa4d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="6fa4d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fa4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fa4d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-115">Not supported.</span></span> |
| <span data-ttu-id="6fa4d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fa4d-116">Application</span></span> | <span data-ttu-id="6fa4d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-117">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="6fa4d-118">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6fa4d-118">Azure AD</span></span>

| <span data-ttu-id="6fa4d-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fa4d-119">Permission type</span></span> | <span data-ttu-id="6fa4d-120">Permissions</span><span class="sxs-lookup"><span data-stu-id="6fa4d-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="6fa4d-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fa4d-121">Delegated (work or school account)</span></span> | <span data-ttu-id="6fa4d-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6fa4d-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="6fa4d-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fa4d-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fa4d-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-124">Not supported.</span></span> |
| <span data-ttu-id="6fa4d-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fa4d-125">Application</span></span> | <span data-ttu-id="6fa4d-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-126">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="6fa4d-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="6fa4d-127">Groups</span></span>

|<span data-ttu-id="6fa4d-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fa4d-128">Permission type</span></span> | <span data-ttu-id="6fa4d-129">Permissions</span><span class="sxs-lookup"><span data-stu-id="6fa4d-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="6fa4d-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fa4d-130">Delegated (work or school account)</span></span> | <span data-ttu-id="6fa4d-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="6fa4d-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="6fa4d-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fa4d-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fa4d-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-133">Not supported.</span></span> |
| <span data-ttu-id="6fa4d-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fa4d-134">Application</span></span> | <span data-ttu-id="6fa4d-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-135">Not supported.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="6fa4d-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6fa4d-136">Optional query parameters</span></span>
<span data-ttu-id="6fa4d-137">Este método não **dá suporte** a [Parâmetros de Consulta OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="6fa4d-137">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="6fa4d-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fa4d-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="6fa4d-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa4d-139">Request headers</span></span>
| <span data-ttu-id="6fa4d-140">Nome</span><span class="sxs-lookup"><span data-stu-id="6fa4d-140">Name</span></span>       | <span data-ttu-id="6fa4d-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa4d-141">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6fa4d-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fa4d-142">Authorization</span></span>  | <span data-ttu-id="6fa4d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="6fa4d-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="6fa4d-145">Content-type</span></span>  | <span data-ttu-id="6fa4d-146">application/json</span><span class="sxs-lookup"><span data-stu-id="6fa4d-146">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fa4d-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa4d-147">Request body</span></span>
<span data-ttu-id="6fa4d-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fa4d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fa4d-149">Response</span></span>
<span data-ttu-id="6fa4d-p103">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="6fa4d-152">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="6fa4d-152">Error codes</span></span>
<span data-ttu-id="6fa4d-153">Esta API segue o padrão de códigos HTTP.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-153">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="6fa4d-154">Além disso, os códigos de erro personalizados são mostrados abaixo.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-154">Besides, the custom error codes are shown below.</span></span>

| <span data-ttu-id="6fa4d-155">Código de erro</span><span class="sxs-lookup"><span data-stu-id="6fa4d-155">Error code</span></span> | <span data-ttu-id="6fa4d-156">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="6fa4d-156">Error message</span></span> | <span data-ttu-id="6fa4d-157">Detalhes</span><span class="sxs-lookup"><span data-stu-id="6fa4d-157">Details</span></span> |
|:---------- |:------------- |:------- |
| <span data-ttu-id="6fa4d-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="6fa4d-158">400 BadRequest</span></span> | <span data-ttu-id="6fa4d-159">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="6fa4d-159">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="6fa4d-160">O governanceRoleAssignmentRequest não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-160">The governanceRoleAssignmentRequest does not exist in system.</span></span> |
| <span data-ttu-id="6fa4d-161">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="6fa4d-161">400 BadRequest</span></span> | <span data-ttu-id="6fa4d-162">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="6fa4d-162">RequestCannotBeCancelled</span></span> | <span data-ttu-id="6fa4d-163">Somente solicitações no status `Granted` de , e podem ser `PendingApproval` `PendingApprovalProvisioning` `PendingAdminDecision` canceladas.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-163">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span> |

## <a name="example"></a><span data-ttu-id="6fa4d-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fa4d-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="6fa4d-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa4d-165">Request</span></span>
<span data-ttu-id="6fa4d-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fa4d-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6fa4d-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fa4d-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="6fa4d-168">C#</span><span class="sxs-lookup"><span data-stu-id="6fa4d-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fa4d-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fa4d-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fa4d-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fa4d-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fa4d-171">Java</span><span class="sxs-lookup"><span data-stu-id="6fa4d-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-governanceroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6fa4d-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fa4d-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
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


