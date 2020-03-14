---
title: Obter governanceRoleAssignment
description: Recupere as propriedades e os relacionamentos de um governanceRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 038189ac8bda4b51588532cbddc022e83db9ffbf
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639846"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="f944c-103">Obter governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f944c-103">Get governanceRoleAssignment</span></span>

<span data-ttu-id="f944c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f944c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f944c-105">Recupere as propriedades e os relacionamentos de um [governanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f944c-105">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f944c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f944c-106">Permissions</span></span>
<span data-ttu-id="f944c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f944c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f944c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f944c-109">Permission type</span></span>      | <span data-ttu-id="f944c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f944c-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f944c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f944c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f944c-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="f944c-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f944c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f944c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f944c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f944c-114">Not supported.</span></span>    |
|<span data-ttu-id="f944c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f944c-115">Application</span></span> | <span data-ttu-id="f944c-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="f944c-116">PrivilegedAccess.Read.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="f944c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f944c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="f944c-118">Obter um [governanceRoleAssignment](../resources/governanceroleassignment.md) sobre um recurso</span><span class="sxs-lookup"><span data-stu-id="f944c-118">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="f944c-119">*Observação: além do escopo de permissão, ele exige que o solicitante tenha pelo menos uma atribuição de função no recurso.*</span><span class="sxs-lookup"><span data-stu-id="f944c-119">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="f944c-120">Obter uma [governanceRoleAssignment](../resources/governanceroleassignment.md) de meus</span><span class="sxs-lookup"><span data-stu-id="f944c-120">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f944c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f944c-121">Optional query parameters</span></span>
<span data-ttu-id="f944c-122">Este método não **oferece suporte** a [parâmetros de consulta OData](/graph/query-parameters) diferentes de `$filter` para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f944c-122">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f944c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f944c-123">Request headers</span></span>
| <span data-ttu-id="f944c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f944c-124">Name</span></span>      |<span data-ttu-id="f944c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f944c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f944c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f944c-126">Authorization</span></span>  | <span data-ttu-id="f944c-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f944c-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f944c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f944c-128">Request body</span></span>
<span data-ttu-id="f944c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f944c-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f944c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f944c-130">Response</span></span>
<span data-ttu-id="f944c-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [governanceRoleAssignment](../resources/governanceroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f944c-131">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f944c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f944c-132">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="f944c-133">Obtenha um [governanceRoleAssignment](../resources/governanceroleassignment.md) na assinatura "Wingtip Toys-Prod"</span><span class="sxs-lookup"><span data-stu-id="f944c-133">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="f944c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f944c-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="f944c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f944c-135">Response</span></span>
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
