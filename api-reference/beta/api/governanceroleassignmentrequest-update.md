---
title: Atualizar governanceRoleAssignmentRequests
description: Permitir que os administradores atualizem suas decisões ( `AdminApproved` ou `AdminDenied` ) no governanceRoleAssignmentRequests que estão no status de `PendingAdminDecision` .
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 75c6044e6fc76c0ac19e7990240b883f663cba04
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991044"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="accbe-103">Atualizar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="accbe-103">Update governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="accbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="accbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="accbe-105">Permitir que os administradores atualizem suas decisões ( `AdminApproved` ou `AdminDenied` ) no [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão no status de `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="accbe-105">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="accbe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="accbe-106">Permissions</span></span>
<span data-ttu-id="accbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="accbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="accbe-109">**Observação:** Essa API também exige que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador ( `owner` ou `user access administrator` ) no recurso ao qual o [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="accbe-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="accbe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="accbe-110">Permission type</span></span>      | <span data-ttu-id="accbe-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="accbe-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="accbe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="accbe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="accbe-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="accbe-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="accbe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="accbe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="accbe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="accbe-115">Not supported.</span></span>    |
|<span data-ttu-id="accbe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="accbe-116">Application</span></span> | <span data-ttu-id="accbe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="accbe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="accbe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="accbe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="accbe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="accbe-119">Request headers</span></span>
| <span data-ttu-id="accbe-120">Nome</span><span class="sxs-lookup"><span data-stu-id="accbe-120">Name</span></span>           | <span data-ttu-id="accbe-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="accbe-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="accbe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="accbe-122">Authorization</span></span>  | <span data-ttu-id="accbe-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="accbe-123">Bearer {code}</span></span>|
| <span data-ttu-id="accbe-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="accbe-124">Content-type</span></span>  | <span data-ttu-id="accbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="accbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="accbe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="accbe-126">Request body</span></span>

|<span data-ttu-id="accbe-127">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="accbe-127">Parameters</span></span>      |<span data-ttu-id="accbe-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="accbe-128">Type</span></span>                   |<span data-ttu-id="accbe-129">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="accbe-129">Required</span></span> |<span data-ttu-id="accbe-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="accbe-130">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="accbe-131">motivo</span><span class="sxs-lookup"><span data-stu-id="accbe-131">reason</span></span>        |<span data-ttu-id="accbe-132">String</span><span class="sxs-lookup"><span data-stu-id="accbe-132">String</span></span>                 |<span data-ttu-id="accbe-133">✓</span><span class="sxs-lookup"><span data-stu-id="accbe-133">✓</span></span>        |<span data-ttu-id="accbe-134">O motivo fornecido pelo administrador para sua decisão.</span><span class="sxs-lookup"><span data-stu-id="accbe-134">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="accbe-135">sobre</span><span class="sxs-lookup"><span data-stu-id="accbe-135">decision</span></span>        |<span data-ttu-id="accbe-136">String</span><span class="sxs-lookup"><span data-stu-id="accbe-136">String</span></span>                 |<span data-ttu-id="accbe-137">✓</span><span class="sxs-lookup"><span data-stu-id="accbe-137">✓</span></span>        |<span data-ttu-id="accbe-138">A decisão de administrador da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="accbe-138">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="accbe-139">O valor deve ser atualizado como `AdminApproved` ou `AdminDenied` .</span><span class="sxs-lookup"><span data-stu-id="accbe-139">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="accbe-140">Cronograma</span><span class="sxs-lookup"><span data-stu-id="accbe-140">schedule</span></span>      |[<span data-ttu-id="accbe-141">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="accbe-141">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="accbe-142">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="accbe-142">The schedule of the role assignment request.</span></span> <span data-ttu-id="accbe-143">Para o status de `AdminApproved` , é necessário.</span><span class="sxs-lookup"><span data-stu-id="accbe-143">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="accbe-144">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="accbe-144">assignmentState</span></span>      |<span data-ttu-id="accbe-145">String</span><span class="sxs-lookup"><span data-stu-id="accbe-145">String</span></span>|         | <span data-ttu-id="accbe-146">O estado da atribuição e os valores podem ser `Eligible` ou `Active` .</span><span class="sxs-lookup"><span data-stu-id="accbe-146">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="accbe-147">Para a decisão de `AdminApproved` , é necessário.</span><span class="sxs-lookup"><span data-stu-id="accbe-147">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="accbe-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="accbe-148">Response</span></span>
<span data-ttu-id="accbe-149">Este método só pode ser aplicado a solicitações que estão no status de `PendingAdminDecision` .</span><span class="sxs-lookup"><span data-stu-id="accbe-149">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="accbe-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="accbe-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="accbe-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="accbe-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="accbe-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="accbe-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="accbe-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="accbe-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="c"></a>[<span data-ttu-id="accbe-155">C#</span><span class="sxs-lookup"><span data-stu-id="accbe-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="accbe-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="accbe-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="accbe-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="accbe-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="accbe-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="accbe-158">Request body</span></span>
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a><span data-ttu-id="accbe-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="accbe-159">Response</span></span>
<!-- {
  "blockType": "response",
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
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


