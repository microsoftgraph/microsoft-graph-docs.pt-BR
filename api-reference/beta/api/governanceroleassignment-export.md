---
title: Exportar governançaRoleAssignmentRequests
description: Recupere uma coleção de governanceRoleAssignmentRequests no formato , que pode ser analisado como um `application/octet-stream` arquivo .csv no navegador.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 49a555a690ce23af43af4359d6894b440df7e90e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435935"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="1e505-103">Exportar governançaRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="1e505-103">Export governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="1e505-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e505-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e505-105">Recupere uma coleção [de governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) no formato , que pode ser analisado como um `application/octet-stream` arquivo .csv no navegador.</span><span class="sxs-lookup"><span data-stu-id="1e505-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e505-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e505-106">Permissions</span></span>
<span data-ttu-id="1e505-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="1e505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="1e505-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="1e505-109">Azure resources</span></span>

| <span data-ttu-id="1e505-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e505-110">Permission type</span></span> | <span data-ttu-id="1e505-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e505-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="1e505-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e505-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e505-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1e505-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="1e505-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e505-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e505-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e505-115">Not supported.</span></span> |
| <span data-ttu-id="1e505-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e505-116">Application</span></span> | <span data-ttu-id="1e505-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="1e505-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="1e505-118">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1e505-118">Azure AD</span></span>

| <span data-ttu-id="1e505-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e505-119">Permission type</span></span> | <span data-ttu-id="1e505-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e505-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="1e505-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e505-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1e505-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="1e505-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="1e505-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e505-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e505-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e505-124">Not supported.</span></span> |
| <span data-ttu-id="1e505-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e505-125">Application</span></span> | <span data-ttu-id="1e505-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="1e505-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="1e505-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="1e505-127">Groups</span></span>

|<span data-ttu-id="1e505-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e505-128">Permission type</span></span> | <span data-ttu-id="1e505-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e505-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="1e505-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e505-130">Delegated (work or school account)</span></span> | <span data-ttu-id="1e505-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="1e505-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="1e505-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e505-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e505-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e505-133">Not supported.</span></span> |
| <span data-ttu-id="1e505-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e505-134">Application</span></span> | <span data-ttu-id="1e505-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="1e505-135">PrivilegedAccess.Read.AzureADGroups</span></span> |


## <a name="http-request"></a><span data-ttu-id="1e505-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e505-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="1e505-137">Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso</span><span class="sxs-lookup"><span data-stu-id="1e505-137">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="1e505-138">**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="1e505-138">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="1e505-139">Exportar uma coleção [de governançaRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) de minha</span><span class="sxs-lookup"><span data-stu-id="1e505-139">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e505-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1e505-140">Optional query parameters</span></span>
<span data-ttu-id="1e505-141">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e505-141">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e505-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e505-142">Request headers</span></span>
| <span data-ttu-id="1e505-143">Nome</span><span class="sxs-lookup"><span data-stu-id="1e505-143">Name</span></span>      |<span data-ttu-id="1e505-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e505-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e505-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e505-145">Authorization</span></span>  | <span data-ttu-id="1e505-146">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1e505-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e505-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e505-147">Request body</span></span>
<span data-ttu-id="1e505-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e505-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e505-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e505-149">Response</span></span>
<span data-ttu-id="1e505-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um conteúdo do tipo `application/octet-stream` .</span><span class="sxs-lookup"><span data-stu-id="1e505-150">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="1e505-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e505-151">Example</span></span>
<span data-ttu-id="1e505-152">Este exemplo salva todas as atribuições de função como um arquivo .csv na assinatura Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="1e505-152">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="1e505-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e505-153">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="1e505-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e505-154">Response</span></span>
<span data-ttu-id="1e505-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e505-155">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


