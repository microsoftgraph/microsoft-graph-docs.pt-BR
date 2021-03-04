---
title: Obter governanceRoleAssignment
description: Recupere as propriedades e as relações de um governanceRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 3f01060b80c9f50712014a16987d519d19b5bf91
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435921"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="10916-103">Obter governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="10916-103">Get governanceRoleAssignment</span></span>

<span data-ttu-id="10916-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10916-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10916-105">Recupere as propriedades e as relações de um [governanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="10916-105">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="10916-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10916-106">Permissions</span></span>
<span data-ttu-id="10916-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="10916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="10916-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="10916-109">Azure resources</span></span>

| <span data-ttu-id="10916-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10916-110">Permission type</span></span> | <span data-ttu-id="10916-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="10916-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="10916-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10916-112">Delegated (work or school account)</span></span> | <span data-ttu-id="10916-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="10916-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="10916-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10916-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10916-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10916-115">Not supported.</span></span> |
| <span data-ttu-id="10916-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10916-116">Application</span></span> | <span data-ttu-id="10916-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="10916-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="10916-118">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="10916-118">Azure AD</span></span>

| <span data-ttu-id="10916-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10916-119">Permission type</span></span> | <span data-ttu-id="10916-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="10916-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="10916-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10916-121">Delegated (work or school account)</span></span> | <span data-ttu-id="10916-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="10916-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="10916-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10916-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10916-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10916-124">Not supported.</span></span> |
| <span data-ttu-id="10916-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10916-125">Application</span></span> | <span data-ttu-id="10916-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="10916-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="10916-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="10916-127">Groups</span></span>

|<span data-ttu-id="10916-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10916-128">Permission type</span></span> | <span data-ttu-id="10916-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="10916-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="10916-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10916-130">Delegated (work or school account)</span></span> | <span data-ttu-id="10916-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="10916-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="10916-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10916-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10916-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10916-133">Not supported.</span></span> |
| <span data-ttu-id="10916-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10916-134">Application</span></span> | <span data-ttu-id="10916-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="10916-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="10916-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10916-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="10916-137">Obter uma [governançaRoleAssignment](../resources/governanceroleassignment.md) em um recurso</span><span class="sxs-lookup"><span data-stu-id="10916-137">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="10916-138">*Observação: além do escopo de permissão, ele exige que o solicitante tenha pelo menos uma atribuição de função no recurso.*</span><span class="sxs-lookup"><span data-stu-id="10916-138">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="10916-139">Obter um [governanceRoleAssignment](../resources/governanceroleassignment.md) meu</span><span class="sxs-lookup"><span data-stu-id="10916-139">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10916-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10916-140">Optional query parameters</span></span>
<span data-ttu-id="10916-141">Este método não **dá suporte** a [parâmetros de consulta OData](/graph/query-parameters) que não `$filter` seja para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="10916-141">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10916-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10916-142">Request headers</span></span>
| <span data-ttu-id="10916-143">Nome</span><span class="sxs-lookup"><span data-stu-id="10916-143">Name</span></span>      |<span data-ttu-id="10916-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="10916-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10916-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="10916-145">Authorization</span></span>  | <span data-ttu-id="10916-146">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="10916-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="10916-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10916-147">Request body</span></span>
<span data-ttu-id="10916-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10916-148">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="10916-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="10916-149">Response</span></span>
<span data-ttu-id="10916-150">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto governanceRoleAssignment](../resources/governanceroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10916-150">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10916-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10916-151">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="10916-152">Obter uma [governançaRoleAssignment na](../resources/governanceroleassignment.md) assinatura "Wingtip Toys - Prod"</span><span class="sxs-lookup"><span data-stu-id="10916-152">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="10916-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10916-153">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="10916-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="10916-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 182

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments/$entity",
    "id": "0ba78f41-ee7a-4227-adb9-1499431b2164",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "74487eb5-1630-4fa8-9581-0bb076ea5de3",
    "linkedEligibleRoleAssignmentId": null,
    "externalId": null,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


