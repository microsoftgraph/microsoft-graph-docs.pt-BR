---
title: Exportar governanceRoleAssignmentRequests
description: Recupere uma coleção de governanceRoleAssignmentRequests no formato `application/octet-stream` , que pode ser analisado como um arquivo. csv no navegador.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: a975205ffdfcca831bfd7e2a17c4ceeb51988fd3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991156"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="113c8-103">Exportar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="113c8-103">Export governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="113c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="113c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="113c8-105">Recupere uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) no formato `application/octet-stream` , que pode ser analisado como um arquivo. csv no navegador.</span><span class="sxs-lookup"><span data-stu-id="113c8-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="113c8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="113c8-106">Permissions</span></span>
<span data-ttu-id="113c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="113c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="113c8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="113c8-109">Permission type</span></span>      | <span data-ttu-id="113c8-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="113c8-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="113c8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="113c8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="113c8-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="113c8-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="113c8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="113c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="113c8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="113c8-114">Not supported.</span></span>    |
|<span data-ttu-id="113c8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="113c8-115">Application</span></span> | <span data-ttu-id="113c8-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="113c8-116">PrivilegedAccess.Read.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="113c8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="113c8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="113c8-118">Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso</span><span class="sxs-lookup"><span data-stu-id="113c8-118">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="113c8-119">**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="113c8-119">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="113c8-120">Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) de meus</span><span class="sxs-lookup"><span data-stu-id="113c8-120">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="113c8-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="113c8-121">Optional query parameters</span></span>
<span data-ttu-id="113c8-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="113c8-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="113c8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="113c8-123">Request headers</span></span>
| <span data-ttu-id="113c8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="113c8-124">Name</span></span>      |<span data-ttu-id="113c8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="113c8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="113c8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="113c8-126">Authorization</span></span>  | <span data-ttu-id="113c8-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="113c8-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="113c8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="113c8-128">Request body</span></span>
<span data-ttu-id="113c8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="113c8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="113c8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="113c8-130">Response</span></span>
<span data-ttu-id="113c8-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o conteúdo do tipo `application/octet-stream` .</span><span class="sxs-lookup"><span data-stu-id="113c8-131">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="113c8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="113c8-132">Example</span></span>
<span data-ttu-id="113c8-133">Este exemplo salva todas as atribuições de função como um arquivo. csv na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="113c8-133">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="113c8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="113c8-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="113c8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="113c8-135">Response</span></span>
<span data-ttu-id="113c8-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="113c8-136">Here is an example of the response.</span></span> 
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


