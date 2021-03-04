---
title: Cancelar privilegedRoleAssignmentRequest
description: Cancele um privilegedRoleAssignmentRequest.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 2a2e600b4f1c97b54aacaed9a96a2b55dd916b8d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441172"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="e642c-103">Cancelar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e642c-103">Cancel privilegedRoleAssignmentRequest</span></span>

<span data-ttu-id="e642c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e642c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e642c-105">Cancele [um privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="e642c-105">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e642c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e642c-106">Permissions</span></span>
<span data-ttu-id="e642c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e642c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e642c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e642c-109">Permission type</span></span>                        | <span data-ttu-id="e642c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e642c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e642c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e642c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e642c-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e642c-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e642c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e642c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e642c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e642c-114">Not supported.</span></span> |
|<span data-ttu-id="e642c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e642c-115">Application</span></span>                            | <span data-ttu-id="e642c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e642c-116">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="e642c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e642c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="e642c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e642c-118">Request headers</span></span>
| <span data-ttu-id="e642c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e642c-119">Name</span></span>      |<span data-ttu-id="e642c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e642c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e642c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e642c-121">Authorization</span></span>  | <span data-ttu-id="e642c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e642c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e642c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e642c-124">Request body</span></span>
<span data-ttu-id="e642c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e642c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e642c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e642c-126">Response</span></span>
<span data-ttu-id="e642c-127">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="e642c-127">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="e642c-128">Ele retorna [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e642c-128">It returns [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="e642c-129">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="e642c-129">Error codes</span></span>
<span data-ttu-id="e642c-130">Esta API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="e642c-130">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="e642c-131">Além disso, ele retorna os códigos de erro personalizados listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="e642c-131">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="e642c-132">Código de erro</span><span class="sxs-lookup"><span data-stu-id="e642c-132">Error code</span></span>     | <span data-ttu-id="e642c-133">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="e642c-133">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="e642c-134">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e642c-134">400 BadRequest</span></span> | <span data-ttu-id="e642c-135">RequestId não pode ser Null.</span><span class="sxs-lookup"><span data-stu-id="e642c-135">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="e642c-136">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e642c-136">400 BadRequest</span></span> | <span data-ttu-id="e642c-137">Solicitação com ID de solicitação não encontrada.</span><span class="sxs-lookup"><span data-stu-id="e642c-137">Request with request ID not found.</span></span> |
| <span data-ttu-id="e642c-138">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="e642c-138">400 BadRequest</span></span> | <span data-ttu-id="e642c-139">O cancelamento só pode ser feito no status Scheduled e PendingApproval.</span><span class="sxs-lookup"><span data-stu-id="e642c-139">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="e642c-140">403 Não Autorizado</span><span class="sxs-lookup"><span data-stu-id="e642c-140">403 UnAuthorized</span></span> | <span data-ttu-id="e642c-141">O solicitante não tem permissão para fazer cancelar chamada ou solicitação não encontrada.</span><span class="sxs-lookup"><span data-stu-id="e642c-141">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="e642c-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e642c-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e642c-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e642c-143">Request</span></span>
<span data-ttu-id="e642c-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e642c-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e642c-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e642c-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="c"></a>[<span data-ttu-id="e642c-146">C#</span><span class="sxs-lookup"><span data-stu-id="e642c-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-privilegedroleassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e642c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e642c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-privilegedroleassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e642c-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e642c-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-privilegedroleassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e642c-149">Java</span><span class="sxs-lookup"><span data-stu-id="e642c-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cancel-privilegedroleassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e642c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e642c-150">Response</span></span>
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


