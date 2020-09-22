---
title: Obter governanceRoleAssignmentRequest
description: 'Obter um governanceRoleAssignmentRequest. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 4e63269d627f83e6287e544eb7c6a59ac0e777e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991100"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="dbc1c-103">Obter governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="dbc1c-103">Get governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="dbc1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbc1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbc1c-105">Obter um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="dbc1c-105">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="dbc1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbc1c-106">Permissions</span></span>
<span data-ttu-id="dbc1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbc1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbc1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbc1c-109">Permission type</span></span>      | <span data-ttu-id="dbc1c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbc1c-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbc1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbc1c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dbc1c-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="dbc1c-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="dbc1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbc1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbc1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbc1c-114">Not supported.</span></span>    |
|<span data-ttu-id="dbc1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbc1c-115">Application</span></span> | <span data-ttu-id="dbc1c-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="dbc1c-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="dbc1c-117">Além do escopo de permissão, ele requer o solicitante</span><span class="sxs-lookup"><span data-stu-id="dbc1c-117">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="dbc1c-118">para ter pelo menos uma atribuição de função no recurso; ou</span><span class="sxs-lookup"><span data-stu-id="dbc1c-118">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="dbc1c-119">é o assunto do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="dbc1c-119">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="dbc1c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbc1c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dbc1c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dbc1c-121">Optional query parameters</span></span>
<span data-ttu-id="dbc1c-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dbc1c-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbc1c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbc1c-123">Request headers</span></span>
| <span data-ttu-id="dbc1c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="dbc1c-124">Name</span></span>      |<span data-ttu-id="dbc1c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbc1c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dbc1c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbc1c-126">Authorization</span></span>  | <span data-ttu-id="dbc1c-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="dbc1c-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbc1c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbc1c-128">Request body</span></span>
<span data-ttu-id="dbc1c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbc1c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbc1c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbc1c-130">Response</span></span>
<span data-ttu-id="dbc1c-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbc1c-131">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbc1c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbc1c-132">Example</span></span>
<span data-ttu-id="dbc1c-133">Obter uma solicitação de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="dbc1c-133">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="dbc1c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbc1c-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="dbc1c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbc1c-135">Response</span></span>
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


