---
title: Obter governanceRoleAssignment
description: Recupere as propriedades e relacionamentos de um governanceRoleAssignment.
ms.openlocfilehash: 622fb890422ed0a4cf00542fede5ebaf662e5e71
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191071"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="bf55d-103">Obter governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bf55d-103">Get governanceRoleAssignment</span></span>

> <span data-ttu-id="bf55d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bf55d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf55d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bf55d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf55d-106">Recupere as propriedades e relacionamentos de um [governanceRoleAssignment](../resources/governanceroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bf55d-106">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf55d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf55d-107">Permissions</span></span>
<span data-ttu-id="bf55d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf55d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf55d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf55d-110">Permission type</span></span>      | <span data-ttu-id="bf55d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf55d-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf55d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf55d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf55d-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="bf55d-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="bf55d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf55d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf55d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf55d-115">Not supported.</span></span>    |
|<span data-ttu-id="bf55d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf55d-116">Application</span></span> | <span data-ttu-id="bf55d-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="bf55d-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf55d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf55d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="bf55d-119">Obtenha um [governanceRoleAssignment](../resources/governanceroleassignment.md) em um recurso</span><span class="sxs-lookup"><span data-stu-id="bf55d-119">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="bf55d-120">*Observação: Além do escopo de permissão, ele requer o solicitante ter pelo menos uma atribuição no recurso.*</span><span class="sxs-lookup"><span data-stu-id="bf55d-120">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="bf55d-121">Obtenha um [governanceRoleAssignment](../resources/governanceroleassignment.md) meu</span><span class="sxs-lookup"><span data-stu-id="bf55d-121">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf55d-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bf55d-122">Optional query parameters</span></span>
<span data-ttu-id="bf55d-123">Esse método **suporta [Parâmetros de consulta OData](/graph/query-parameters) diferente de** `$filter` para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bf55d-123">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf55d-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf55d-124">Request headers</span></span>
| <span data-ttu-id="bf55d-125">Nome</span><span class="sxs-lookup"><span data-stu-id="bf55d-125">Name</span></span>      |<span data-ttu-id="bf55d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf55d-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bf55d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf55d-127">Authorization</span></span>  | <span data-ttu-id="bf55d-128">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="bf55d-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf55d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf55d-129">Request body</span></span>
<span data-ttu-id="bf55d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bf55d-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bf55d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf55d-131">Response</span></span>
<span data-ttu-id="bf55d-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [governanceRoleAssignment](../resources/governanceroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf55d-132">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bf55d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf55d-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="bf55d-134">Obtenha um [governanceRoleAssignment](../resources/governanceroleassignment.md) na assinatura "Wingtip Toys – produção"</span><span class="sxs-lookup"><span data-stu-id="bf55d-134">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="bf55d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf55d-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="bf55d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf55d-136">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->