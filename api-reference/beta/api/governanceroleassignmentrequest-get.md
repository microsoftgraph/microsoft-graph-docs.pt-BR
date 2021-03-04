---
title: Obter governançaRoleAssignmentRequest
description: 'Obter uma governançaRoleAssignmentRequest. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 63d7e1e494d2195f5622dfa6b0c2e6403975b8da
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435867"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="f87a0-103">Obter governançaRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="f87a0-103">Get governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="f87a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f87a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f87a0-105">Obter um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f87a0-105">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="f87a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f87a0-106">Permissions</span></span>
<span data-ttu-id="f87a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="f87a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="f87a0-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="f87a0-109">Azure resources</span></span>

| <span data-ttu-id="f87a0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f87a0-110">Permission type</span></span> | <span data-ttu-id="f87a0-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f87a0-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="f87a0-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f87a0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f87a0-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f87a0-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="f87a0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f87a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f87a0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f87a0-115">Not supported.</span></span> |
| <span data-ttu-id="f87a0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f87a0-116">Application</span></span> | <span data-ttu-id="f87a0-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f87a0-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="f87a0-118">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f87a0-118">Azure AD</span></span>

| <span data-ttu-id="f87a0-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f87a0-119">Permission type</span></span> | <span data-ttu-id="f87a0-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="f87a0-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="f87a0-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f87a0-121">Delegated (work or school account)</span></span> | <span data-ttu-id="f87a0-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f87a0-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="f87a0-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f87a0-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f87a0-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f87a0-124">Not supported.</span></span> |
| <span data-ttu-id="f87a0-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f87a0-125">Application</span></span> | <span data-ttu-id="f87a0-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f87a0-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="f87a0-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="f87a0-127">Groups</span></span>

|<span data-ttu-id="f87a0-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f87a0-128">Permission type</span></span> | <span data-ttu-id="f87a0-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="f87a0-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="f87a0-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f87a0-130">Delegated (work or school account)</span></span> | <span data-ttu-id="f87a0-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="f87a0-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="f87a0-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f87a0-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f87a0-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f87a0-133">Not supported.</span></span> |
| <span data-ttu-id="f87a0-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f87a0-134">Application</span></span> | <span data-ttu-id="f87a0-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="f87a0-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="f87a0-136">Além do escopo de permissão, ele requer o solicitante</span><span class="sxs-lookup"><span data-stu-id="f87a0-136">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="f87a0-137">ter pelo menos uma atribuição de função no recurso; ou</span><span class="sxs-lookup"><span data-stu-id="f87a0-137">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="f87a0-138">é o assunto do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f87a0-138">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="f87a0-139">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f87a0-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f87a0-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f87a0-140">Optional query parameters</span></span>
<span data-ttu-id="f87a0-141">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f87a0-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f87a0-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f87a0-142">Request headers</span></span>
| <span data-ttu-id="f87a0-143">Nome</span><span class="sxs-lookup"><span data-stu-id="f87a0-143">Name</span></span>      |<span data-ttu-id="f87a0-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="f87a0-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f87a0-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="f87a0-145">Authorization</span></span>  | <span data-ttu-id="f87a0-146">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f87a0-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f87a0-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f87a0-147">Request body</span></span>
<span data-ttu-id="f87a0-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f87a0-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f87a0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f87a0-149">Response</span></span>
<span data-ttu-id="f87a0-150">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f87a0-150">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f87a0-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f87a0-151">Example</span></span>
<span data-ttu-id="f87a0-152">Obter uma solicitação de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="f87a0-152">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="f87a0-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f87a0-153">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="f87a0-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f87a0-154">Response</span></span>
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


