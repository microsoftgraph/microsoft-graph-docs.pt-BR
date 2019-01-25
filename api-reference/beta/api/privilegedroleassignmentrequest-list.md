---
title: Lista privilegedRoleAssignmentRequests
description: 'Recupere uma coleção de privilegedRoleAssignmentRequest. '
localization_priority: Normal
ms.openlocfilehash: 06a6c66bcb566df0b6db5193bd753832bd9235a3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519980"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="88443-103">Lista privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="88443-103">List privilegedRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88443-104">Recupere uma coleção de [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="88443-104">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="88443-105">**Observação:** Deste solicitante deve ter pelo menos uma atribuição no recurso.</span><span class="sxs-lookup"><span data-stu-id="88443-105">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="88443-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="88443-106">Permissions</span></span>
<span data-ttu-id="88443-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88443-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88443-109">Permission type</span></span>                        | <span data-ttu-id="88443-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88443-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="88443-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88443-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88443-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88443-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="88443-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88443-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88443-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88443-114">Not supported.</span></span> |
|<span data-ttu-id="88443-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88443-115">Application</span></span>                            | <span data-ttu-id="88443-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88443-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88443-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88443-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88443-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88443-118">Optional query parameters</span></span>
<span data-ttu-id="88443-119">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88443-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88443-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88443-120">Request headers</span></span>
| <span data-ttu-id="88443-121">Nome</span><span class="sxs-lookup"><span data-stu-id="88443-121">Name</span></span>      |<span data-ttu-id="88443-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="88443-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88443-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88443-123">Authorization</span></span>  | <span data-ttu-id="88443-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88443-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88443-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88443-126">Request body</span></span>
<span data-ttu-id="88443-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88443-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88443-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="88443-128">Response</span></span>
<span data-ttu-id="88443-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88443-129">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88443-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88443-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88443-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88443-131">Request</span></span>
<span data-ttu-id="88443-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="88443-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
##### <a name="response"></a><span data-ttu-id="88443-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="88443-133">Response</span></span>
<span data-ttu-id="88443-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88443-134">The following is an example of the response.</span></span> <span data-ttu-id="88443-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="88443-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="88443-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88443-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "@odata.context":"https://https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests",
  "value":[
    {
      "schedule":{
        "type":"activation","startDateTime":"2018-02-07T22:55:00Z","endDateTime":null,"duration" : null
      },"id":"03ea0c3d-90a0-42d4-b220-11c049c506fb","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-02-07T22:17:37.2215343Z","status":"ApprovalAborted","duration":"1","reason":"Activate for testing","ticketNumber":"222","ticketSystem":"222"
    },{
      "schedule":{
        "type":"assignment","startDateTime":"2018-01-23T02:43:15.258242Z","endDateTime":null,"duration" : null
      },"id":"fe4450bb-6d28-4583-8fc4-25b0ea91daf5","userId": "Self"，"roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b","evaluateOnly":false,"type":"UserAdd","assignmentState":"Active","requestedDateTime":"2018-01-23T02:42:55.628338Z","status":"Completed","duration":"1","reason":"asdf","ticketNumber":null,"ticketSystem":null
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
