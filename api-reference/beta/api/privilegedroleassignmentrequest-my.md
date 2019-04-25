---
title: 'privilegedRoleAssignmentRequest: My'
description: Obtenha as solicitações de atribuição de função privilegiada do solicitante.
localization_priority: Normal
ms.openlocfilehash: 79545b5ea0ad88c55d7a09eb5c77982e812721eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546549"
---
# <a name="privilegedroleassignmentrequest-my"></a><span data-ttu-id="828c4-103">privilegedRoleAssignmentRequest: My</span><span class="sxs-lookup"><span data-stu-id="828c4-103">privilegedRoleAssignmentRequest: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="828c4-104">Obtenha as solicitações de atribuição de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="828c4-104">Get the requester's privileged role assignment requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="828c4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="828c4-105">Permissions</span></span>
<span data-ttu-id="828c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="828c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="828c4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="828c4-108">Permission type</span></span>                        | <span data-ttu-id="828c4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="828c4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="828c4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="828c4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="828c4-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="828c4-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="828c4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="828c4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="828c4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828c4-113">Not supported.</span></span> |
|<span data-ttu-id="828c4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="828c4-114">Application</span></span>                            | <span data-ttu-id="828c4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828c4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="828c4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="828c4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests/my
```
## <a name="optional-query-parameters"></a><span data-ttu-id="828c4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="828c4-117">Optional query parameters</span></span>
<span data-ttu-id="828c4-118">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="828c4-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="828c4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="828c4-119">Request headers</span></span>
| <span data-ttu-id="828c4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="828c4-120">Name</span></span>      |<span data-ttu-id="828c4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="828c4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="828c4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="828c4-122">Authorization</span></span>  | <span data-ttu-id="828c4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="828c4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="828c4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="828c4-125">Request body</span></span>
<span data-ttu-id="828c4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="828c4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="828c4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="828c4-127">Response</span></span>
<span data-ttu-id="828c4-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="828c4-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="828c4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="828c4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="828c4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="828c4-130">Request</span></span>
<span data-ttu-id="828c4-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="828c4-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignmentrequest_my)"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/my
```

##### <a name="response"></a><span data-ttu-id="828c4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="828c4-132">Response</span></span>
<span data-ttu-id="828c4-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="828c4-133">The following is an example of the response.</span></span> <span data-ttu-id="828c4-134">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="828c4-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="828c4-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="828c4-135">All of the properties will be returned from an actual call.</span></span>
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
         "userId": "Self"，
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
        "userId": "Self"，
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
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-my.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
