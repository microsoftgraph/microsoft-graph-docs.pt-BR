---
title: Lista privilegedRoleAssignmentRequests
description: 'Recupere uma coleção de privilegedRoleAssignmentRequest. '
ms.openlocfilehash: c47ad101e4e4008985be6732f5f6358b705959b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038499"
---
# <a name="list-privilegedroleassignmentrequests"></a><span data-ttu-id="f1a6b-103">Lista privilegedRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f1a6b-103">List privilegedRoleAssignmentRequests</span></span>

> <span data-ttu-id="f1a6b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1a6b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f1a6b-106">Recupere uma coleção de [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f1a6b-106">Retrieve a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span> 

<span data-ttu-id="f1a6b-107">**Observação:** Deste solicitante deve ter pelo menos uma atribuição no recurso.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-107">**Note:** This requester must have at least one role assignment on the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1a6b-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="f1a6b-108">Permissions</span></span>
<span data-ttu-id="f1a6b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a6b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1a6b-111">Permission type</span></span>                        | <span data-ttu-id="f1a6b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1a6b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1a6b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1a6b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f1a6b-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f1a6b-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f1a6b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1a6b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a6b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-116">Not supported.</span></span> |
|<span data-ttu-id="f1a6b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1a6b-117">Application</span></span>                            | <span data-ttu-id="f1a6b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1a6b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a6b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1a6b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1a6b-120">Optional query parameters</span></span>
<span data-ttu-id="f1a6b-121">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1a6b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a6b-122">Request headers</span></span>
| <span data-ttu-id="f1a6b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f1a6b-123">Name</span></span>      |<span data-ttu-id="f1a6b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1a6b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f1a6b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1a6b-125">Authorization</span></span>  | <span data-ttu-id="f1a6b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1a6b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a6b-128">Request body</span></span>
<span data-ttu-id="f1a6b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1a6b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1a6b-130">Response</span></span>
<span data-ttu-id="f1a6b-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-131">If successful, this method returns a `200 OK` response code and a collection of [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1a6b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1a6b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1a6b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1a6b-133">Request</span></span>
<span data-ttu-id="f1a6b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignmentrequest"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
```
##### <a name="response"></a><span data-ttu-id="f1a6b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1a6b-135">Response</span></span>
<span data-ttu-id="f1a6b-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-136">The following is an example of the response.</span></span> <span data-ttu-id="f1a6b-137">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f1a6b-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1a6b-138">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
