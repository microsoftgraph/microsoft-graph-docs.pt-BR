---
title: Exportar governanceRoleAssignmentRequests
description: Recuperar uma coleção de governanceRoleAssignmentRequests no formato `application/octet-stream`, que pode ser analisada como um arquivo. csv no navegador.
localization_priority: Normal
ms.openlocfilehash: 10fd7c720bf7b6f162a4d8c2189e81a9205e53ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828725"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="15255-103">Exportar governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="15255-103">Export governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="15255-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="15255-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15255-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15255-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15255-106">Recuperar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) no formato `application/octet-stream`, que pode ser analisada como um arquivo. csv no navegador.</span><span class="sxs-lookup"><span data-stu-id="15255-106">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="15255-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="15255-107">Permissions</span></span>
<span data-ttu-id="15255-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15255-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15255-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15255-110">Permission type</span></span>      | <span data-ttu-id="15255-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="15255-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15255-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15255-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15255-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="15255-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="15255-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15255-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15255-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15255-115">Not supported.</span></span>    |
|<span data-ttu-id="15255-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15255-116">Application</span></span> | <span data-ttu-id="15255-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="15255-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |


## <a name="http-request"></a><span data-ttu-id="15255-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15255-118">HTTP request</span></span>
<span data-ttu-id="15255-119"><!-- { "blockType": "ignored" } -->Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) em um recurso</span><span class="sxs-lookup"><span data-stu-id="15255-119"><!-- { "blockType": "ignored" } --> Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="15255-120">**Observação:** Além do escopo de permissão, esta solicitação requer o solicitante ter pelo menos uma atribuição no recurso.</span><span class="sxs-lookup"><span data-stu-id="15255-120">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="15255-121">Exportar uma coleção de [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) dos meus</span><span class="sxs-lookup"><span data-stu-id="15255-121">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15255-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="15255-122">Optional query parameters</span></span>
<span data-ttu-id="15255-123">Este método oferece suporte para os [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="15255-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15255-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15255-124">Request headers</span></span>
| <span data-ttu-id="15255-125">Nome</span><span class="sxs-lookup"><span data-stu-id="15255-125">Name</span></span>      |<span data-ttu-id="15255-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="15255-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15255-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="15255-127">Authorization</span></span>  | <span data-ttu-id="15255-128">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="15255-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="15255-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15255-129">Request body</span></span>
<span data-ttu-id="15255-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15255-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15255-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="15255-131">Response</span></span>
<span data-ttu-id="15255-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e o conteúdo do tipo `application/octet-stream`.</span><span class="sxs-lookup"><span data-stu-id="15255-132">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="15255-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15255-133">Example</span></span>
<span data-ttu-id="15255-134">Este exemplo salva todas as atribuições de função, como um arquivo. csv na assinatura Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="15255-134">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="15255-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15255-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="15255-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="15255-136">Response</span></span>
<span data-ttu-id="15255-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15255-137">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
