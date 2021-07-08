---
title: Obter unifiedRoleAssignmentScheduleRequest
description: Leia as propriedades e as relações de um objeto unifiedRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e7b33eea1551bcf0d5bd661cc4f097e8f0e01a82
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334406"
---
# <a name="get-unifiedroleassignmentschedulerequest"></a><span data-ttu-id="ccc57-103">Obter unifiedRoleAssignmentScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="ccc57-103">Get unifiedRoleAssignmentScheduleRequest</span></span>
<span data-ttu-id="ccc57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccc57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccc57-105">Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="ccc57-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccc57-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccc57-106">Permissions</span></span>
<span data-ttu-id="ccc57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccc57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccc57-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccc57-109">Permission type</span></span>|<span data-ttu-id="ccc57-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccc57-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccc57-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccc57-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ccc57-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="ccc57-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="ccc57-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccc57-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccc57-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ccc57-114">Not supported</span></span>|
|<span data-ttu-id="ccc57-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccc57-115">Application</span></span>|<span data-ttu-id="ccc57-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="ccc57-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccc57-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccc57-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccc57-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ccc57-118">Optional query parameters</span></span>
<span data-ttu-id="ccc57-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ccc57-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ccc57-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ccc57-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccc57-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccc57-121">Request headers</span></span>
|<span data-ttu-id="ccc57-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ccc57-122">Name</span></span>|<span data-ttu-id="ccc57-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccc57-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ccc57-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccc57-124">Authorization</span></span>|<span data-ttu-id="ccc57-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccc57-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccc57-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccc57-127">Request body</span></span>
<span data-ttu-id="ccc57-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ccc57-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccc57-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccc57-129">Response</span></span>

<span data-ttu-id="ccc57-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccc57-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccc57-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ccc57-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ccc57-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccc57-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ccc57-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccc57-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```
# <a name="c"></a>[<span data-ttu-id="ccc57-134">C#</span><span class="sxs-lookup"><span data-stu-id="ccc57-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccc57-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccc57-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccc57-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccc57-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccc57-137">Java</span><span class="sxs-lookup"><span data-stu-id="ccc57-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ccc57-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccc57-138">Response</span></span>
<span data-ttu-id="ccc57-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ccc57-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
    "action": "String",
    "principalId": "String",
    "roleDefinitionId": "String",
    "directoryScopeId": "String",
    "appScopeId": "String",
    "isValidationOnly": "Boolean",
    "targetScheduleId": "String",
    "justification": "String",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    },
    "ticketInfo": {
      "@odata.type": "microsoft.graph.ticketInfo"
    }
  }
}
```

