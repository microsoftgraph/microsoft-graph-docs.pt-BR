---
title: Lista governanceRoleAssignments
description: Recupere uma coleção de governanceRoleAssignments.
ms.openlocfilehash: 0f4680c8998191fa07af993e8ee3712557b7010d
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191064"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="b6f83-103">Lista governanceRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="b6f83-103">List governanceRoleAssignments</span></span>

> <span data-ttu-id="b6f83-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6f83-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6f83-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6f83-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6f83-106">Recupere uma coleção de [governanceRoleAssignments](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b6f83-106">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6f83-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6f83-107">Permissions</span></span>
<span data-ttu-id="b6f83-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f83-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6f83-110">Permission type</span></span>      | <span data-ttu-id="b6f83-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6f83-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6f83-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6f83-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6f83-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b6f83-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b6f83-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6f83-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6f83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f83-115">Not supported.</span></span>    |
|<span data-ttu-id="b6f83-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6f83-116">Application</span></span> | <span data-ttu-id="b6f83-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="b6f83-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="b6f83-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f83-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b6f83-119">Uma coleção de [governanceRoleAssignments](../resources/governanceroleassignment.md) em um recurso de lista.</span><span class="sxs-lookup"><span data-stu-id="b6f83-119">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="b6f83-120">**Observação:** Além do escopo de permissão, esta solicitação requer o solicitante ter pelo menos uma atribuição no recurso.</span><span class="sxs-lookup"><span data-stu-id="b6f83-120">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="b6f83-121">Uma coleção de [governanceRoleAssignments](../resources/governanceroleassignment.md) dos meus de lista.</span><span class="sxs-lookup"><span data-stu-id="b6f83-121">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6f83-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6f83-122">Optional query parameters</span></span>
<span data-ttu-id="b6f83-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f83-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6f83-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f83-124">Request headers</span></span>
| <span data-ttu-id="b6f83-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b6f83-125">Name</span></span>      |<span data-ttu-id="b6f83-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6f83-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6f83-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6f83-127">Authorization</span></span>  | <span data-ttu-id="b6f83-128">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b6f83-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f83-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f83-129">Request body</span></span>
<span data-ttu-id="b6f83-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6f83-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6f83-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f83-131">Response</span></span>
<span data-ttu-id="b6f83-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [governanceRoleAssignment](../resources/governanceroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f83-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6f83-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6f83-133">Example</span></span>

<span data-ttu-id="b6f83-134">Este exemplo mostra como obter minhas atribuições de função na subscrição Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="b6f83-134">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="b6f83-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f83-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="b6f83-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f83-136">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
