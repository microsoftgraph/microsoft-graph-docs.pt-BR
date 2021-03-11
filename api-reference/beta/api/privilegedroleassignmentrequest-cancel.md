---
title: Cancelar privilegedRoleAssignmentRequest
description: Cancele um privilegedRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 9ff689e661b98e2a84f998cc301e20ddb0f53424
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720558"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="f59aa-103">Cancelar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f59aa-103">Cancel privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="f59aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f59aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f59aa-105">Cancele [um privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f59aa-105">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f59aa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f59aa-106">Permissions</span></span>
<span data-ttu-id="f59aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f59aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f59aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f59aa-109">Permission type</span></span>                        | <span data-ttu-id="f59aa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f59aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f59aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f59aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f59aa-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f59aa-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f59aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f59aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f59aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f59aa-114">Not supported.</span></span> |
|<span data-ttu-id="f59aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f59aa-115">Application</span></span>                            | <span data-ttu-id="f59aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f59aa-116">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="f59aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f59aa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/{requestid}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="f59aa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f59aa-118">Request headers</span></span>
| <span data-ttu-id="f59aa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f59aa-119">Name</span></span>      |<span data-ttu-id="f59aa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f59aa-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f59aa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f59aa-121">Authorization</span></span>  | <span data-ttu-id="f59aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f59aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f59aa-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f59aa-124">Request body</span></span>
<span data-ttu-id="f59aa-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f59aa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f59aa-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f59aa-126">Response</span></span>
<span data-ttu-id="f59aa-127">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="f59aa-127">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="f59aa-128">Ele retorna [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f59aa-128">It returns [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="f59aa-129">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="f59aa-129">Error codes</span></span>
<span data-ttu-id="f59aa-130">Esta API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="f59aa-130">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="f59aa-131">Além disso, ele retorna os códigos de erro personalizados listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f59aa-131">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="f59aa-132">Código de erro</span><span class="sxs-lookup"><span data-stu-id="f59aa-132">Error code</span></span>     | <span data-ttu-id="f59aa-133">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="f59aa-133">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="f59aa-134">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f59aa-134">400 BadRequest</span></span> | <span data-ttu-id="f59aa-135">RequestId não pode ser Null.</span><span class="sxs-lookup"><span data-stu-id="f59aa-135">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="f59aa-136">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f59aa-136">400 BadRequest</span></span> | <span data-ttu-id="f59aa-137">Solicitação com ID de solicitação não encontrada.</span><span class="sxs-lookup"><span data-stu-id="f59aa-137">Request with request ID not found.</span></span> |
| <span data-ttu-id="f59aa-138">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f59aa-138">400 BadRequest</span></span> | <span data-ttu-id="f59aa-139">O cancelamento só pode ser feito no status Scheduled e PendingApproval.</span><span class="sxs-lookup"><span data-stu-id="f59aa-139">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="f59aa-140">403 Não Autorizado</span><span class="sxs-lookup"><span data-stu-id="f59aa-140">403 UnAuthorized</span></span> | <span data-ttu-id="f59aa-141">O solicitante não tem permissão para fazer cancelar chamada ou solicitação não encontrada.</span><span class="sxs-lookup"><span data-stu-id="f59aa-141">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="f59aa-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f59aa-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f59aa-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f59aa-143">Request</span></span>
<span data-ttu-id="f59aa-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f59aa-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f59aa-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f59aa-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="f59aa-146">C#</span><span class="sxs-lookup"><span data-stu-id="f59aa-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-privilegedroleassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f59aa-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f59aa-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-privilegedroleassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f59aa-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f59aa-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-privilegedroleassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f59aa-149">Java</span><span class="sxs-lookup"><span data-stu-id="f59aa-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-privilegedroleassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f59aa-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f59aa-150">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "bcfb11e3-fc0d-49ea-b3d5-7d60a48e5043",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "Cancelling",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


