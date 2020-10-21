---
title: Obter governanceRoleAssignmentRequest
description: 'Obter um governanceRoleAssignmentRequest. '
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 1e52cf77c9dd2be0a059f7c119c416f69b109715
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635009"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="79247-103">Obter governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="79247-103">Get governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="79247-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79247-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79247-105">Obter um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="79247-105">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="79247-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="79247-106">Permissions</span></span>
<span data-ttu-id="79247-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="79247-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="79247-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="79247-109">Azure resources</span></span>

| <span data-ttu-id="79247-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79247-110">Permission type</span></span> | <span data-ttu-id="79247-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="79247-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="79247-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79247-112">Delegated (work or school account)</span></span> | <span data-ttu-id="79247-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="79247-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="79247-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79247-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79247-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79247-115">Not supported.</span></span> |
| <span data-ttu-id="79247-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79247-116">Application</span></span> | <span data-ttu-id="79247-117">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="79247-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="79247-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="79247-118">Azure AD</span></span>

| <span data-ttu-id="79247-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79247-119">Permission type</span></span> | <span data-ttu-id="79247-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="79247-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="79247-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79247-121">Delegated (work or school account)</span></span> | <span data-ttu-id="79247-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="79247-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="79247-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79247-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79247-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79247-124">Not supported.</span></span> |
| <span data-ttu-id="79247-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79247-125">Application</span></span> | <span data-ttu-id="79247-126">PrivilegedAccess. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="79247-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="79247-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="79247-127">Groups</span></span>

|<span data-ttu-id="79247-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79247-128">Permission type</span></span> | <span data-ttu-id="79247-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="79247-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="79247-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79247-130">Delegated (work or school account)</span></span> | <span data-ttu-id="79247-131">PrivilegedAccess. ReadWrite. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="79247-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="79247-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79247-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79247-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79247-133">Not supported.</span></span> |
| <span data-ttu-id="79247-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79247-134">Application</span></span> | <span data-ttu-id="79247-135">PrivilegedAccess. Read. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="79247-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="79247-136">Além do escopo de permissão, ele requer o solicitante</span><span class="sxs-lookup"><span data-stu-id="79247-136">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="79247-137">para ter pelo menos uma atribuição de função no recurso; ou</span><span class="sxs-lookup"><span data-stu-id="79247-137">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="79247-138">é o assunto do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="79247-138">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="79247-139">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79247-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79247-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79247-140">Optional query parameters</span></span>
<span data-ttu-id="79247-141">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79247-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79247-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79247-142">Request headers</span></span>
| <span data-ttu-id="79247-143">Nome</span><span class="sxs-lookup"><span data-stu-id="79247-143">Name</span></span>      |<span data-ttu-id="79247-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="79247-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79247-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="79247-145">Authorization</span></span>  | <span data-ttu-id="79247-146">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="79247-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="79247-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79247-147">Request body</span></span>
<span data-ttu-id="79247-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79247-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79247-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="79247-149">Response</span></span>
<span data-ttu-id="79247-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79247-150">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79247-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79247-151">Example</span></span>
<span data-ttu-id="79247-152">Obter uma solicitação de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="79247-152">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="79247-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79247-153">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="79247-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="79247-154">Response</span></span>
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


