---
title: Listar governançaRoleAssignments
description: Recupere uma coleção de governanceRoleAssignments.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 07e15d23aabafd3ac775301d7fb89d765b5b642b
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350779"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="185a7-103">Listar governançaRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="185a7-103">List governanceRoleAssignments</span></span>

<span data-ttu-id="185a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="185a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="185a7-105">Recuperar uma coleção de [governanceRoleAssignments](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="185a7-105">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="185a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="185a7-106">Permissions</span></span>
<span data-ttu-id="185a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="185a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="185a7-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="185a7-109">Azure resources</span></span>

| <span data-ttu-id="185a7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="185a7-110">Permission type</span></span> | <span data-ttu-id="185a7-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="185a7-111">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="185a7-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="185a7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="185a7-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="185a7-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="185a7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="185a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="185a7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="185a7-115">Not supported.</span></span> |
| <span data-ttu-id="185a7-116">Application</span><span class="sxs-lookup"><span data-stu-id="185a7-116">Application</span></span> | <span data-ttu-id="185a7-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="185a7-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="185a7-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="185a7-118">Azure AD</span></span>

| <span data-ttu-id="185a7-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="185a7-119">Permission type</span></span> | <span data-ttu-id="185a7-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="185a7-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="185a7-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="185a7-121">Delegated (work or school account)</span></span> | <span data-ttu-id="185a7-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="185a7-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="185a7-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="185a7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="185a7-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="185a7-124">Not supported.</span></span> |
| <span data-ttu-id="185a7-125">Application</span><span class="sxs-lookup"><span data-stu-id="185a7-125">Application</span></span> | <span data-ttu-id="185a7-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="185a7-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="185a7-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="185a7-127">Groups</span></span>

|<span data-ttu-id="185a7-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="185a7-128">Permission type</span></span> | <span data-ttu-id="185a7-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="185a7-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="185a7-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="185a7-130">Delegated (work or school account)</span></span> | <span data-ttu-id="185a7-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="185a7-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="185a7-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="185a7-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="185a7-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="185a7-133">Not supported.</span></span> |
| <span data-ttu-id="185a7-134">Application</span><span class="sxs-lookup"><span data-stu-id="185a7-134">Application</span></span> | <span data-ttu-id="185a7-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="185a7-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

## <a name="http-request"></a><span data-ttu-id="185a7-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="185a7-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="185a7-137">Listar uma coleção [de governanceRoleAssignments](../resources/governanceroleassignment.md) em um recurso.</span><span class="sxs-lookup"><span data-stu-id="185a7-137">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="185a7-138">**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="185a7-138">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="185a7-139">Listar uma coleção [de governançaRoleAssignments](../resources/governanceroleassignment.md) minhas.</span><span class="sxs-lookup"><span data-stu-id="185a7-139">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="185a7-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="185a7-140">Optional query parameters</span></span>
<span data-ttu-id="185a7-141">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="185a7-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="185a7-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="185a7-142">Request headers</span></span>
| <span data-ttu-id="185a7-143">Nome</span><span class="sxs-lookup"><span data-stu-id="185a7-143">Name</span></span>      |<span data-ttu-id="185a7-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="185a7-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="185a7-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="185a7-145">Authorization</span></span>  | <span data-ttu-id="185a7-146">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="185a7-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="185a7-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="185a7-147">Request body</span></span>
<span data-ttu-id="185a7-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="185a7-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="185a7-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="185a7-149">Response</span></span>
<span data-ttu-id="185a7-150">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos governanceRoleAssignment](../resources/governanceroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="185a7-150">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="185a7-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="185a7-151">Example</span></span>

<span data-ttu-id="185a7-152">Este exemplo mostra como obter minhas atribuições de função na assinatura Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="185a7-152">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="185a7-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="185a7-153">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="185a7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="185a7-154">Response</span></span>
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


