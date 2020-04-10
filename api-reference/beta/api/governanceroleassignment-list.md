---
title: Listar governanceRoleAssignments
description: Recupere uma coleção de governanceRoleAssignments.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 914dfba11cbfa80483c6406e65962d2039c0d5ae
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218889"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="87c80-103">Listar governanceRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="87c80-103">List governanceRoleAssignments</span></span>

<span data-ttu-id="87c80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87c80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87c80-105">Recupere uma coleção de [governanceRoleAssignments](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="87c80-105">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87c80-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87c80-106">Permissions</span></span>
<span data-ttu-id="87c80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87c80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87c80-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87c80-109">Permission type</span></span>      | <span data-ttu-id="87c80-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="87c80-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c80-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87c80-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87c80-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="87c80-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="87c80-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87c80-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87c80-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87c80-114">Not supported.</span></span>    |
|<span data-ttu-id="87c80-115">Application</span><span class="sxs-lookup"><span data-stu-id="87c80-115">Application</span></span> | <span data-ttu-id="87c80-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="87c80-116">PrivilegedAccess.Read.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="87c80-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87c80-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="87c80-118">Lista uma coleção de [governanceRoleAssignments](../resources/governanceroleassignment.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="87c80-118">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="87c80-119">**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="87c80-119">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="87c80-120">Liste uma coleção de [governanceRoleAssignments](../resources/governanceroleassignment.md) de meus.</span><span class="sxs-lookup"><span data-stu-id="87c80-120">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87c80-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87c80-121">Optional query parameters</span></span>
<span data-ttu-id="87c80-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87c80-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87c80-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87c80-123">Request headers</span></span>
| <span data-ttu-id="87c80-124">Nome</span><span class="sxs-lookup"><span data-stu-id="87c80-124">Name</span></span>      |<span data-ttu-id="87c80-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="87c80-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87c80-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="87c80-126">Authorization</span></span>  | <span data-ttu-id="87c80-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="87c80-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="87c80-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87c80-128">Request body</span></span>
<span data-ttu-id="87c80-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87c80-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87c80-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="87c80-130">Response</span></span>
<span data-ttu-id="87c80-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [governanceRoleAssignment](../resources/governanceroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87c80-131">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87c80-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87c80-132">Example</span></span>

<span data-ttu-id="87c80-133">Este exemplo mostra como obter minhas atribuições de função na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="87c80-133">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="87c80-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87c80-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="87c80-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="87c80-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 2062

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments",
    "value": [
        {
            "id": "20f4157d-5837-4356-9630-ebd3a832f227",
            "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-13T01:19:08.59Z",
            "endDateTime": "2018-06-11T01:18:37.08Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        {
            "id": "e327f4be-42a0-47a2-8579-0a39b025b394",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-28T16:56:48.243Z",
            "endDateTime": "2018-09-24T16:56:30.547Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        ...
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
