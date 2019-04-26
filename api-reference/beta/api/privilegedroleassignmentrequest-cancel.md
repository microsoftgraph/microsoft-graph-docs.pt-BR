---
title: Cancelar privilegedRoleAssignmentRequest
description: Cancelar uma privilegedRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: 649ec481815ccb4ce903e51ecb98ccf99cdfa77f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337213"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="3c334-103">Cancelar privilegedRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="3c334-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c334-104">Cancelar uma [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="3c334-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c334-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c334-105">Permissions</span></span>
<span data-ttu-id="3c334-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c334-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c334-108">Permission type</span></span>                        | <span data-ttu-id="3c334-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c334-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c334-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c334-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c334-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="3c334-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c334-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c334-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c334-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c334-113">Not supported.</span></span> |
|<span data-ttu-id="3c334-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c334-114">Application</span></span>                            | <span data-ttu-id="3c334-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c334-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="3c334-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c334-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="3c334-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c334-117">Request headers</span></span>
| <span data-ttu-id="3c334-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3c334-118">Name</span></span>      |<span data-ttu-id="3c334-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c334-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3c334-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c334-120">Authorization</span></span>  | <span data-ttu-id="3c334-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c334-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c334-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c334-123">Request body</span></span>
<span data-ttu-id="3c334-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c334-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c334-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c334-125">Response</span></span>
<span data-ttu-id="3c334-126">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="3c334-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="3c334-127">Ele retorna [privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c334-127">It returns [privilegedRoleAssignmentRequest](../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="3c334-128">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="3c334-128">Error codes</span></span>
<span data-ttu-id="3c334-129">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="3c334-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="3c334-130">Além disso, ele retorna os códigos de erro personalizados listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="3c334-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="3c334-131">Código de erro</span><span class="sxs-lookup"><span data-stu-id="3c334-131">Error code</span></span>     | <span data-ttu-id="3c334-132">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="3c334-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="3c334-133">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="3c334-133">400 BadRequest</span></span> | <span data-ttu-id="3c334-134">RequestId não pode ser nulo.</span><span class="sxs-lookup"><span data-stu-id="3c334-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="3c334-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="3c334-135">400 BadRequest</span></span> | <span data-ttu-id="3c334-136">Solicitação com ID de solicitação não encontrada.</span><span class="sxs-lookup"><span data-stu-id="3c334-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="3c334-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="3c334-137">400 BadRequest</span></span> | <span data-ttu-id="3c334-138">O cancelamento pode ser feito apenas em status agendado e PendingApproval.</span><span class="sxs-lookup"><span data-stu-id="3c334-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="3c334-139">403 não autorizado</span><span class="sxs-lookup"><span data-stu-id="3c334-139">403 UnAuthorized</span></span> | <span data-ttu-id="3c334-140">O solicitante não tem permissão para cancelar a chamada ou a solicitação de canCelamento.</span><span class="sxs-lookup"><span data-stu-id="3c334-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="3c334-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c334-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c334-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c334-142">Request</span></span>
<span data-ttu-id="3c334-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c334-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="3c334-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c334-144">Response</span></span>
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
  "suppressions": []
}
-->
