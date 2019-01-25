---
title: Obter governanceRoleAssignment
description: Recupere as propriedades e relacionamentos de um governanceRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: f699e1b5332652b2b87f3972d2ae47b06894b2e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508836"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="a5050-103">Obter governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a5050-103">Get governanceRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5050-104">Recupere as propriedades e relacionamentos de um [governanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a5050-104">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5050-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5050-105">Permissions</span></span>
<span data-ttu-id="a5050-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5050-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5050-108">Permission type</span></span>      | <span data-ttu-id="a5050-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5050-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5050-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5050-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5050-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a5050-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a5050-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5050-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5050-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5050-113">Not supported.</span></span>    |
|<span data-ttu-id="a5050-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5050-114">Application</span></span> | <span data-ttu-id="a5050-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a5050-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5050-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5050-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="a5050-117">Obtenha um [governanceRoleAssignment](../resources/governanceroleassignment.md) em um recurso</span><span class="sxs-lookup"><span data-stu-id="a5050-117">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="a5050-118">*Observação: Além do escopo de permissão, ele requer o solicitante ter pelo menos uma atribuição no recurso.*</span><span class="sxs-lookup"><span data-stu-id="a5050-118">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="a5050-119">Obtenha um [governanceRoleAssignment](../resources/governanceroleassignment.md) meu</span><span class="sxs-lookup"><span data-stu-id="a5050-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5050-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5050-120">Optional query parameters</span></span>
<span data-ttu-id="a5050-121">Esse método **suporta [Parâmetros de consulta OData](/graph/query-parameters) diferente de** `$filter` para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5050-121">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5050-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5050-122">Request headers</span></span>
| <span data-ttu-id="a5050-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a5050-123">Name</span></span>      |<span data-ttu-id="a5050-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5050-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5050-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5050-125">Authorization</span></span>  | <span data-ttu-id="a5050-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a5050-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5050-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5050-127">Request body</span></span>
<span data-ttu-id="a5050-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5050-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a5050-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5050-129">Response</span></span>
<span data-ttu-id="a5050-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [governanceRoleAssignment](../resources/governanceroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5050-130">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5050-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5050-131">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="a5050-132">Obtenha um [governanceRoleAssignment](../resources/governanceroleassignment.md) na assinatura "Wingtip Toys – produção"</span><span class="sxs-lookup"><span data-stu-id="a5050-132">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="a5050-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5050-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="a5050-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5050-134">Response</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
