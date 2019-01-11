---
title: Cancelar governanceRoleAssignmentRequest
description: Cancele um governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: f155a832a0c29935216dbc740e7db6ae8708f429
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809104"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="9ebff-103">Cancelar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9ebff-103">Cancel governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="9ebff-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ebff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ebff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ebff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ebff-106">Cancele um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="9ebff-106">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ebff-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9ebff-107">Permissions</span></span>
<span data-ttu-id="9ebff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ebff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ebff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ebff-110">Permission type</span></span>      | <span data-ttu-id="9ebff-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="9ebff-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ebff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ebff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9ebff-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9ebff-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9ebff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ebff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ebff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ebff-115">Not supported.</span></span>    |
|<span data-ttu-id="9ebff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ebff-116">Application</span></span> | <span data-ttu-id="9ebff-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9ebff-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="9ebff-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ebff-118">Optional query parameters</span></span>
<span data-ttu-id="9ebff-119">Esse método **não** suporta [Parâmetros da Consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9ebff-119">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="9ebff-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ebff-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="9ebff-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ebff-121">Request headers</span></span>
| <span data-ttu-id="9ebff-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9ebff-122">Name</span></span>       | <span data-ttu-id="9ebff-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ebff-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ebff-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ebff-124">Authorization</span></span>  | <span data-ttu-id="9ebff-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9ebff-125">Bearer {code}</span></span>|
| <span data-ttu-id="9ebff-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="9ebff-126">Content-type</span></span>  | <span data-ttu-id="9ebff-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ebff-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ebff-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ebff-128">Request body</span></span>
<span data-ttu-id="9ebff-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ebff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ebff-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ebff-130">Response</span></span>
<span data-ttu-id="9ebff-p103">Se bem-sucedido, este método retorna um código de resposta `204 NoContent`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ebff-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="9ebff-133">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="9ebff-133">Error codes</span></span>
<span data-ttu-id="9ebff-134">Essa API segue o padrão dos códigos HTTP.</span><span class="sxs-lookup"><span data-stu-id="9ebff-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="9ebff-135">Além disso, os códigos de erro personalizadas são mostrados abaixo.</span><span class="sxs-lookup"><span data-stu-id="9ebff-135">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="9ebff-136">Código de erro</span><span class="sxs-lookup"><span data-stu-id="9ebff-136">Error code</span></span>     | <span data-ttu-id="9ebff-137">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="9ebff-137">Error message</span></span>              | <span data-ttu-id="9ebff-138">Detalhes</span><span class="sxs-lookup"><span data-stu-id="9ebff-138">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="9ebff-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9ebff-139">400 BadRequest</span></span> | <span data-ttu-id="9ebff-140">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="9ebff-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="9ebff-141">O governanceRoleAssignmentRequest não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="9ebff-141">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="9ebff-142">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9ebff-142">400 BadRequest</span></span> | <span data-ttu-id="9ebff-143">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="9ebff-143">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="9ebff-144">Somente as solicitações em status de `Granted`, `PendingApproval`, `PendingApprovalProvisioning` e `PendingAdminDecision` pode ser cancelado.</span><span class="sxs-lookup"><span data-stu-id="9ebff-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="9ebff-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ebff-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ebff-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ebff-146">Request</span></span>
<span data-ttu-id="9ebff-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ebff-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="9ebff-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ebff-148">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
