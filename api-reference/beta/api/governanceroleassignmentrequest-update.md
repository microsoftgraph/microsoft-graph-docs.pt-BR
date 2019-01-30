---
title: Atualizar governanceRoleAssignmentRequests
description: Permitem que administradores atualizar suas decisões (`AdminApproved` ou `AdminDenied`) em governanceRoleAssignmentRequests que estão no status de `PendingAdminDecision`.
localization_priority: Normal
ms.openlocfilehash: 870cd685aade9bb722660b550ae210c6e10d1fe8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643259"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="9d2cb-103">Atualizar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="9d2cb-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d2cb-104">Permitem que administradores atualizar suas decisões (`AdminApproved` ou `AdminDenied`) em [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) que estão no status de `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d2cb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d2cb-105">Permissions</span></span>
<span data-ttu-id="9d2cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d2cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="9d2cb-108">**Observação:** Essa API também requer que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) em relação ao qual pertence o [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) recurso.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="9d2cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d2cb-109">Permission type</span></span>      | <span data-ttu-id="9d2cb-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d2cb-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d2cb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d2cb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9d2cb-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d2cb-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9d2cb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d2cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d2cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-114">Not supported.</span></span>    |
|<span data-ttu-id="9d2cb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d2cb-115">Application</span></span> | <span data-ttu-id="9d2cb-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d2cb-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d2cb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d2cb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="9d2cb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d2cb-118">Request headers</span></span>
| <span data-ttu-id="9d2cb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9d2cb-119">Name</span></span>           | <span data-ttu-id="9d2cb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d2cb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9d2cb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d2cb-121">Authorization</span></span>  | <span data-ttu-id="9d2cb-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9d2cb-122">Bearer {code}</span></span>|
| <span data-ttu-id="9d2cb-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="9d2cb-123">Content-type</span></span>  | <span data-ttu-id="9d2cb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9d2cb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d2cb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d2cb-125">Request body</span></span>

|<span data-ttu-id="9d2cb-126">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="9d2cb-126">Parameters</span></span>      |<span data-ttu-id="9d2cb-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d2cb-127">Type</span></span>                   |<span data-ttu-id="9d2cb-128">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="9d2cb-128">Required</span></span> |<span data-ttu-id="9d2cb-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d2cb-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="9d2cb-130">motivo</span><span class="sxs-lookup"><span data-stu-id="9d2cb-130">reason</span></span>        |<span data-ttu-id="9d2cb-131">String</span><span class="sxs-lookup"><span data-stu-id="9d2cb-131">String</span></span>                 |<span data-ttu-id="9d2cb-132">✓</span><span class="sxs-lookup"><span data-stu-id="9d2cb-132">✓</span></span>        |<span data-ttu-id="9d2cb-133">O motivo fornecido pelo administrador para a sua decisão.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="9d2cb-134">decisão</span><span class="sxs-lookup"><span data-stu-id="9d2cb-134">decision</span></span>        |<span data-ttu-id="9d2cb-135">String</span><span class="sxs-lookup"><span data-stu-id="9d2cb-135">String</span></span>                 |<span data-ttu-id="9d2cb-136">✓</span><span class="sxs-lookup"><span data-stu-id="9d2cb-136">✓</span></span>        |<span data-ttu-id="9d2cb-137">A decisão de administrador da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="9d2cb-138">O valor deve ser atualizado como `AdminApproved` ou `AdminDenied`.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="9d2cb-139">agenda</span><span class="sxs-lookup"><span data-stu-id="9d2cb-139">schedule</span></span>      |[<span data-ttu-id="9d2cb-140">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="9d2cb-140">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="9d2cb-141">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="9d2cb-142">Status da `AdminApproved`, é necessário.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="9d2cb-143">assignmentState</span><span class="sxs-lookup"><span data-stu-id="9d2cb-143">assignmentState</span></span>      |<span data-ttu-id="9d2cb-144">String</span><span class="sxs-lookup"><span data-stu-id="9d2cb-144">String</span></span>|         | <span data-ttu-id="9d2cb-145">O estado da atribuição e os valores pode ser `Eligible` ou `Active`.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="9d2cb-146">Decisão de `AdminApproved`, é necessário.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="9d2cb-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d2cb-147">Response</span></span>
<span data-ttu-id="9d2cb-148">Esse método só pode ser aplicado a solicitações que estejam no status de `PendingAdminDecision`.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="9d2cb-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d2cb-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d2cb-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d2cb-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d2cb-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d2cb-152">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="9d2cb-153">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d2cb-153">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="9d2cb-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d2cb-154">Response</span></span>
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
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
