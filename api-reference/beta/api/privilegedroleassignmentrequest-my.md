---
title: 'privilegedRoleAssignmentRequest: My'
description: Obtenha as solicitações de atribuição de função privilegiada do solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8d78ce8d7f9589e40b9c149c3b53a73b94b3f51c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360999"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="b0422-103">privilegedRoleAssignmentRequest: My</span><span class="sxs-lookup"><span data-stu-id="b0422-103">privilegedRoleAssignmentRequest: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0422-104">Obtenha as solicitações de atribuição de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="b0422-104">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0422-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0422-105">Permissions</span></span>
<span data-ttu-id="b0422-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0422-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0422-108">Permission type</span></span>                        | <span data-ttu-id="b0422-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0422-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0422-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0422-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b0422-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="b0422-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0422-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0422-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0422-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0422-113">Not supported.</span></span> |
|<span data-ttu-id="b0422-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0422-114">Application</span></span>                            | <span data-ttu-id="b0422-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0422-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0422-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0422-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0422-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0422-117">Optional query parameters</span></span>
<span data-ttu-id="b0422-118">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0422-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0422-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0422-119">Request headers</span></span>
| <span data-ttu-id="b0422-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b0422-120">Name</span></span>      |<span data-ttu-id="b0422-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0422-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0422-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0422-122">Authorization</span></span>  | <span data-ttu-id="b0422-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0422-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0422-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0422-125">Request body</span></span>
<span data-ttu-id="b0422-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0422-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0422-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0422-127">Response</span></span>
<span data-ttu-id="b0422-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0422-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0422-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0422-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0422-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0422-130">Request</span></span>
<span data-ttu-id="b0422-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0422-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0422-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0422-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0422-133">C#</span><span class="sxs-lookup"><span data-stu-id="b0422-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignmentrequest-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0422-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0422-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignmentrequest-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0422-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b0422-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignmentrequest-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b0422-136">Java</span><span class="sxs-lookup"><span data-stu-id="b0422-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignmentrequest-my-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b0422-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0422-137">Response</span></span>
<span data-ttu-id="b0422-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0422-138">The following is an example of the response.</span></span> <span data-ttu-id="b0422-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b0422-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b0422-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0422-140">All of the properties will be returned from an actual call.</span></span>
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
        "evaluateOnly": false,
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
        "evaluateOnly": false,
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
