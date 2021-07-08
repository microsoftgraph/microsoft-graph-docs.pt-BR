---
title: Listar unifiedRoleEligibilityScheduleRequests
description: Obter uma lista dos objetos unifiedRoleEligibilityScheduleRequest e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: eaee624680315655f7e2326338ef684043c392f8
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334658"
---
# <a name="list-unifiedroleeligibilityschedulerequests"></a><span data-ttu-id="805a0-103">Listar unifiedRoleEligibilityScheduleRequests</span><span class="sxs-lookup"><span data-stu-id="805a0-103">List unifiedRoleEligibilityScheduleRequests</span></span>
<span data-ttu-id="805a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="805a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="805a0-105">Obter uma lista dos [objetos unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="805a0-105">Get a list of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="805a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="805a0-106">Permissions</span></span>
<span data-ttu-id="805a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="805a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="805a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="805a0-109">Permission type</span></span>|<span data-ttu-id="805a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="805a0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="805a0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="805a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="805a0-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="805a0-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span> |
|<span data-ttu-id="805a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="805a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="805a0-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="805a0-114">Not supported</span></span>|
|<span data-ttu-id="805a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="805a0-115">Application</span></span>|<span data-ttu-id="805a0-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="805a0-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="805a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="805a0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="805a0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="805a0-118">Optional query parameters</span></span>
<span data-ttu-id="805a0-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="805a0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="805a0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="805a0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="805a0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="805a0-121">Request headers</span></span>
|<span data-ttu-id="805a0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="805a0-122">Name</span></span>|<span data-ttu-id="805a0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="805a0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="805a0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="805a0-124">Authorization</span></span>|<span data-ttu-id="805a0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="805a0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="805a0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="805a0-127">Request body</span></span>
<span data-ttu-id="805a0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="805a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="805a0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="805a0-129">Response</span></span>

<span data-ttu-id="805a0-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="805a0-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="805a0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="805a0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="805a0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="805a0-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="805a0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="805a0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
```
# <a name="c"></a>[<span data-ttu-id="805a0-134">C#</span><span class="sxs-lookup"><span data-stu-id="805a0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleeligibilityschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="805a0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="805a0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleeligibilityschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="805a0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="805a0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleeligibilityschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="805a0-137">Java</span><span class="sxs-lookup"><span data-stu-id="805a0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleeligibilityschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="805a0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="805a0-138">Response</span></span>
<span data-ttu-id="805a0-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="805a0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```

