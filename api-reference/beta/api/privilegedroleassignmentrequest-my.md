---
title: 'privilegedRoleAssignmentRequest: my'
description: Obter as solicitações de atribuição de função privilegiada do solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f627d7e6be3f79b7064370b9523c409882f5ca22
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037316"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="a3536-103">privilegedRoleAssignmentRequest: my</span><span class="sxs-lookup"><span data-stu-id="a3536-103">privilegedRoleAssignmentRequest: my</span></span>

<span data-ttu-id="a3536-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3536-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3536-105">Obter as solicitações de atribuição de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="a3536-105">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3536-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3536-106">Permissions</span></span>
<span data-ttu-id="a3536-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3536-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3536-109">Permission type</span></span>                        | <span data-ttu-id="a3536-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3536-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3536-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3536-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3536-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3536-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3536-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3536-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3536-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3536-114">Not supported.</span></span> |
|<span data-ttu-id="a3536-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3536-115">Application</span></span>                            | <span data-ttu-id="a3536-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3536-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3536-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3536-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a3536-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a3536-118">Optional query parameters</span></span>
<span data-ttu-id="a3536-119">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a3536-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3536-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3536-120">Request headers</span></span>
| <span data-ttu-id="a3536-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a3536-121">Name</span></span>      |<span data-ttu-id="a3536-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3536-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3536-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3536-123">Authorization</span></span>  | <span data-ttu-id="a3536-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3536-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3536-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3536-126">Request body</span></span>
<span data-ttu-id="a3536-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3536-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3536-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3536-128">Response</span></span>
<span data-ttu-id="a3536-129">Se tiver êxito, este método retornará o código de resposta e o objeto da coleção `200 OK` [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3536-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3536-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3536-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3536-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3536-131">Request</span></span>
<span data-ttu-id="a3536-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3536-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3536-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3536-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```
# <a name="c"></a>[<span data-ttu-id="a3536-134">C#</span><span class="sxs-lookup"><span data-stu-id="a3536-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignmentrequest-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3536-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3536-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignmentrequest-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3536-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3536-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignmentrequest-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3536-137">Java</span><span class="sxs-lookup"><span data-stu-id="a3536-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignmentrequest-my-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a3536-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3536-138">Response</span></span>
<span data-ttu-id="a3536-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a3536-139">The following is an example of the response.</span></span> <span data-ttu-id="a3536-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a3536-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
    "@odata.count": 4,
    "value": [{
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-08T02:35:17.903Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
         "userId": "Self",
         "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
        "status": "RequestedApproval",
        "duration": "2",
        "reason": "Activate the role for business purpose",
        "ticketNumber": "234",
        "ticketSystem": "system",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }, {
        "schedule": {
            "type": "activation",
            "startDateTime": "2018-02-07T22:55:00Z",
            "endDateTime": null,
            "duration" : null
        },
        "id": "03ea0c3d-90a0-42d4-b220-11c049c506fb",
        "userId": "Self",
        "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
        "type": "UserAdd",
        "assignmentState": "Active",
        "requestedDateTime": "2018-02-07T22:17:37.2215343Z",
        "status": "ApprovalAborted",
        "duration": "1",
        "reason": "Activate for testing",
        "ticketNumber": "222",
        "ticketSystem": "222",
        "roleInfo@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests('03ea0c3d-90a0-42d4-b220-11c049c506fb')/roleInfo/$entity",
        "roleInfo": {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "name": "Directory Readers"
        }
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignmentRequest: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


