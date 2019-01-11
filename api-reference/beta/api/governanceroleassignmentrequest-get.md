---
title: Obter governanceRoleAssignmentRequest
description: 'Obtenha um governanceRoleAssignmentRequest. '
localization_priority: Normal
ms.openlocfilehash: 190e79787b32e7e21e9d321ee6f3d90dc27605ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887448"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="0e0c1-103">Obter governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="0e0c1-103">Get governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="0e0c1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0e0c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e0c1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0e0c1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e0c1-106">Obtenha um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="0e0c1-106">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0e0c1-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0e0c1-107">Permissions</span></span>
<span data-ttu-id="0e0c1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e0c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e0c1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e0c1-110">Permission type</span></span>      | <span data-ttu-id="0e0c1-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="0e0c1-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e0c1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e0c1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0e0c1-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0e0c1-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="0e0c1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e0c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e0c1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e0c1-115">Not supported.</span></span>    |
|<span data-ttu-id="0e0c1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e0c1-116">Application</span></span> | <span data-ttu-id="0e0c1-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0e0c1-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="0e0c1-118">Além do escopo de permissão, ele requer o solicitante</span><span class="sxs-lookup"><span data-stu-id="0e0c1-118">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="0e0c1-119">ter pelo menos uma atribuição no recurso; ou</span><span class="sxs-lookup"><span data-stu-id="0e0c1-119">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="0e0c1-120">é o assunto do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="0e0c1-120">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="0e0c1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e0c1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0e0c1-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e0c1-122">Optional query parameters</span></span>
<span data-ttu-id="0e0c1-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e0c1-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e0c1-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e0c1-124">Request headers</span></span>
| <span data-ttu-id="0e0c1-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0e0c1-125">Name</span></span>      |<span data-ttu-id="0e0c1-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e0c1-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0e0c1-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e0c1-127">Authorization</span></span>  | <span data-ttu-id="0e0c1-128">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0e0c1-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e0c1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e0c1-129">Request body</span></span>
<span data-ttu-id="0e0c1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e0c1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e0c1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e0c1-131">Response</span></span>
<span data-ttu-id="0e0c1-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e0c1-132">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e0c1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e0c1-133">Example</span></span>
<span data-ttu-id="0e0c1-134">Obtenha uma solicitação de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="0e0c1-134">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="0e0c1-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e0c1-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="0e0c1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e0c1-136">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
