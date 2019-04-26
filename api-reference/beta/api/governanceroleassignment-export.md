---
title: Exportar governanceRoleAssignmentRequests
description: Recupere uma coleção de governanceRoleAssignmentRequests no formato `application/octet-stream`, que pode ser analisado como um arquivo. csv no navegador.
localization_priority: Normal
ms.openlocfilehash: c01234ce4976d6f900530bdd06d31a4df8e325b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324154"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="d0912-103">Exportar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="d0912-103">Export governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0912-104">Recupere uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) no formato `application/octet-stream`, que pode ser analisado como um arquivo. csv no navegador.</span><span class="sxs-lookup"><span data-stu-id="d0912-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0912-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0912-105">Permissions</span></span>
<span data-ttu-id="d0912-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0912-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0912-108">Permission type</span></span>      | <span data-ttu-id="d0912-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0912-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0912-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0912-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d0912-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="d0912-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d0912-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0912-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0912-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0912-113">Not supported.</span></span>    |
|<span data-ttu-id="d0912-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0912-114">Application</span></span> | <span data-ttu-id="d0912-115">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="d0912-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="d0912-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0912-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d0912-117">Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso</span><span class="sxs-lookup"><span data-stu-id="d0912-117">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="d0912-118">**Observação:** Além do escopo de permissão, essa solicitação exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="d0912-118">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="d0912-119">Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) de meus</span><span class="sxs-lookup"><span data-stu-id="d0912-119">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d0912-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0912-120">Optional query parameters</span></span>
<span data-ttu-id="d0912-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0912-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0912-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0912-122">Request headers</span></span>
| <span data-ttu-id="d0912-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d0912-123">Name</span></span>      |<span data-ttu-id="d0912-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0912-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d0912-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0912-125">Authorization</span></span>  | <span data-ttu-id="d0912-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d0912-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0912-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0912-127">Request body</span></span>
<span data-ttu-id="d0912-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0912-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0912-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0912-129">Response</span></span>
<span data-ttu-id="d0912-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o `application/octet-stream`conteúdo do tipo.</span><span class="sxs-lookup"><span data-stu-id="d0912-130">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="d0912-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0912-131">Example</span></span>
<span data-ttu-id="d0912-132">Este exemplo salva todas as atribuições de função como um arquivo. csv na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="d0912-132">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="d0912-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0912-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="d0912-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0912-134">Response</span></span>
<span data-ttu-id="d0912-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0912-135">Here is an example of the response.</span></span> 
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
