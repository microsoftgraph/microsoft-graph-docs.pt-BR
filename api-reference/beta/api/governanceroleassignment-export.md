---
title: Exportar governanceRoleAssignmentRequests
description: Recupere uma coleção de governanceRoleAssignmentRequests no formato `application/octet-stream` , que pode ser analisado como um arquivo. csv no navegador.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: d37ef5fb09e937835dfe496717b58b3934ee606b
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635051"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="9c14a-103">Exportar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="9c14a-103">Export governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="9c14a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c14a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c14a-105">Recupere uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) no formato `application/octet-stream` , que pode ser analisado como um arquivo. csv no navegador.</span><span class="sxs-lookup"><span data-stu-id="9c14a-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c14a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c14a-106">Permissions</span></span>
<span data-ttu-id="9c14a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="9c14a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="9c14a-109">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="9c14a-109">Azure resources</span></span>

| <span data-ttu-id="9c14a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c14a-110">Permission type</span></span> | <span data-ttu-id="9c14a-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c14a-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="9c14a-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c14a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c14a-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9c14a-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="9c14a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c14a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c14a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c14a-115">Not supported.</span></span> |
| <span data-ttu-id="9c14a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c14a-116">Application</span></span> | <span data-ttu-id="9c14a-117">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="9c14a-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="9c14a-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="9c14a-118">Azure AD</span></span>

| <span data-ttu-id="9c14a-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c14a-119">Permission type</span></span> | <span data-ttu-id="9c14a-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c14a-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="9c14a-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c14a-121">Delegated (work or school account)</span></span> | <span data-ttu-id="9c14a-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="9c14a-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="9c14a-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c14a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c14a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c14a-124">Not supported.</span></span> |
| <span data-ttu-id="9c14a-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c14a-125">Application</span></span> | <span data-ttu-id="9c14a-126">PrivilegedAccess. Read. AzureAD</span><span class="sxs-lookup"><span data-stu-id="9c14a-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="9c14a-127">Grupos</span><span class="sxs-lookup"><span data-stu-id="9c14a-127">Groups</span></span>

|<span data-ttu-id="9c14a-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c14a-128">Permission type</span></span> | <span data-ttu-id="9c14a-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c14a-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="9c14a-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c14a-130">Delegated (work or school account)</span></span> | <span data-ttu-id="9c14a-131">PrivilegedAccess. ReadWrite. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="9c14a-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="9c14a-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c14a-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c14a-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c14a-133">Not supported.</span></span> |
| <span data-ttu-id="9c14a-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c14a-134">Application</span></span> | <span data-ttu-id="9c14a-135">PrivilegedAccess. Read. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="9c14a-135">PrivilegedAccess.Read.AzureADGroups</span></span> |


## <a name="http-request"></a><span data-ttu-id="9c14a-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c14a-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9c14a-137">Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso</span><span class="sxs-lookup"><span data-stu-id="9c14a-137">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="9c14a-138">**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="9c14a-138">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="9c14a-139">Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) de meus</span><span class="sxs-lookup"><span data-stu-id="9c14a-139">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c14a-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9c14a-140">Optional query parameters</span></span>
<span data-ttu-id="9c14a-141">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9c14a-141">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c14a-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c14a-142">Request headers</span></span>
| <span data-ttu-id="9c14a-143">Nome</span><span class="sxs-lookup"><span data-stu-id="9c14a-143">Name</span></span>      |<span data-ttu-id="9c14a-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c14a-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9c14a-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c14a-145">Authorization</span></span>  | <span data-ttu-id="9c14a-146">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9c14a-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c14a-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c14a-147">Request body</span></span>
<span data-ttu-id="9c14a-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c14a-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c14a-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c14a-149">Response</span></span>
<span data-ttu-id="9c14a-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e o conteúdo do tipo `application/octet-stream` .</span><span class="sxs-lookup"><span data-stu-id="9c14a-150">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="9c14a-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c14a-151">Example</span></span>
<span data-ttu-id="9c14a-152">Este exemplo salva todas as atribuições de função como um arquivo. csv na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="9c14a-152">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="9c14a-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c14a-153">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="9c14a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c14a-154">Response</span></span>
<span data-ttu-id="9c14a-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c14a-155">Here is an example of the response.</span></span> 
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


