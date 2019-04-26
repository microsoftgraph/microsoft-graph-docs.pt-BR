---
title: Obter governanceRoleAssignmentRequest
description: 'Obter um governanceRoleAssignmentRequest. '
localization_priority: Normal
ms.openlocfilehash: 8c07aeed9589004051c4db89397979b955bb4dfd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324170"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="fb701-103">Obter governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="fb701-103">Get governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb701-104">Obter um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="fb701-104">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="fb701-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb701-105">Permissions</span></span>
<span data-ttu-id="fb701-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb701-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb701-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb701-108">Permission type</span></span>      | <span data-ttu-id="fb701-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb701-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb701-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb701-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fb701-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="fb701-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="fb701-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb701-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb701-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb701-113">Not supported.</span></span>    |
|<span data-ttu-id="fb701-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb701-114">Application</span></span> | <span data-ttu-id="fb701-115">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="fb701-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="fb701-116">Além do escopo de permissão, ele requer o solicitante</span><span class="sxs-lookup"><span data-stu-id="fb701-116">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="fb701-117">para ter pelo menos uma atribuição de função no recurso; ou</span><span class="sxs-lookup"><span data-stu-id="fb701-117">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="fb701-118">é o assunto do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="fb701-118">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="fb701-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb701-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb701-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fb701-120">Optional query parameters</span></span>
<span data-ttu-id="fb701-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fb701-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb701-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb701-122">Request headers</span></span>
| <span data-ttu-id="fb701-123">Nome</span><span class="sxs-lookup"><span data-stu-id="fb701-123">Name</span></span>      |<span data-ttu-id="fb701-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb701-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fb701-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb701-125">Authorization</span></span>  | <span data-ttu-id="fb701-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="fb701-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb701-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb701-127">Request body</span></span>
<span data-ttu-id="fb701-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb701-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb701-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb701-129">Response</span></span>
<span data-ttu-id="fb701-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb701-130">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb701-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb701-131">Example</span></span>
<span data-ttu-id="fb701-132">Obter uma solicitação de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="fb701-132">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="fb701-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb701-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="fb701-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb701-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"e68ff888-4af5-4ccb-8b74-39156090344b",
  "resourceId":"ec3a00f7-81dc-43b3-bbe7-650d3a5f7d46",
  "roleDefinitionId":"be0767b9-2c31-4b0d-b820-726228e7ff5c",
  "subjectId":"a4c5a837-b546-4ec5-a7df-e61547a46a4b",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"2018-05-09T21:26:15.73-07:00",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
