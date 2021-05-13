---
title: Obter unifiedRoleEligibilityScheduleRequest
description: Leia as propriedades e as relações de um objeto unifiedRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 72279405e77700847b7c885e6bf77b7893377715
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475265"
---
# <a name="get-unifiedroleeligibilityschedulerequest"></a><span data-ttu-id="102db-103">Obter unifiedRoleEligibilityScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="102db-103">Get unifiedRoleEligibilityScheduleRequest</span></span>
<span data-ttu-id="102db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="102db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="102db-105">Leia as propriedades e as relações de [um objeto unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="102db-105">Read the properties and relationships of an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="102db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="102db-106">Permissions</span></span>
<span data-ttu-id="102db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="102db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="102db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="102db-109">Permission type</span></span>|<span data-ttu-id="102db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="102db-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="102db-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="102db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="102db-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="102db-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="102db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="102db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="102db-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="102db-114">Not supported</span></span>|
|<span data-ttu-id="102db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="102db-115">Application</span></span>|<span data-ttu-id="102db-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="102db-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="102db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="102db-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="102db-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="102db-118">Optional query parameters</span></span>
<span data-ttu-id="102db-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="102db-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="102db-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="102db-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="102db-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="102db-121">Request headers</span></span>
|<span data-ttu-id="102db-122">Nome</span><span class="sxs-lookup"><span data-stu-id="102db-122">Name</span></span>|<span data-ttu-id="102db-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="102db-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="102db-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="102db-124">Authorization</span></span>|<span data-ttu-id="102db-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="102db-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="102db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="102db-127">Request body</span></span>
<span data-ttu-id="102db-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="102db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="102db-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="102db-129">Response</span></span>

<span data-ttu-id="102db-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="102db-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="102db-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="102db-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="102db-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="102db-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="102db-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="102db-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```
# <a name="c"></a>[<span data-ttu-id="102db-134">C#</span><span class="sxs-lookup"><span data-stu-id="102db-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleeligibilityschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="102db-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="102db-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleeligibilityschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="102db-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="102db-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleeligibilityschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="102db-137">Java</span><span class="sxs-lookup"><span data-stu-id="102db-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleeligibilityschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="102db-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="102db-138">Response</span></span>
<span data-ttu-id="102db-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="102db-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "a2e242a0-42a0-a2e2-a042-e2a2a042e2a2",
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

