---
title: Obter unifiedRoleAssignmentScheduleInstance
description: Leia as propriedades e as relações de um objeto unifiedRoleAssignmentScheduleInstance.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6b7a78215ce3311d0f70f24ceba30507969532ca
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442672"
---
# <a name="get-unifiedroleassignmentscheduleinstance"></a><span data-ttu-id="d0644-103">Obter unifiedRoleAssignmentScheduleInstance</span><span class="sxs-lookup"><span data-stu-id="d0644-103">Get unifiedRoleAssignmentScheduleInstance</span></span>
<span data-ttu-id="d0644-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0644-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0644-105">Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleInstance.](../resources/unifiedroleassignmentscheduleinstance.md)</span><span class="sxs-lookup"><span data-stu-id="d0644-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0644-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d0644-106">Permissions</span></span>
<span data-ttu-id="d0644-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0644-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0644-109">Permission type</span></span>|<span data-ttu-id="d0644-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0644-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0644-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0644-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0644-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="d0644-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="d0644-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0644-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0644-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d0644-114">Not supported</span></span>|
|<span data-ttu-id="d0644-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0644-115">Application</span></span>|<span data-ttu-id="d0644-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="d0644-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0644-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0644-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstancesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0644-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0644-118">Optional query parameters</span></span>
<span data-ttu-id="d0644-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0644-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d0644-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d0644-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0644-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0644-121">Request headers</span></span>
|<span data-ttu-id="d0644-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d0644-122">Name</span></span>|<span data-ttu-id="d0644-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0644-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d0644-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0644-124">Authorization</span></span>|<span data-ttu-id="d0644-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0644-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0644-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0644-127">Request body</span></span>
<span data-ttu-id="d0644-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0644-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0644-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0644-129">Response</span></span>

<span data-ttu-id="d0644-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0644-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0644-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0644-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0644-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0644-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d0644-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0644-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances/eb18c026-c026-eb18-26c0-18eb26c018eb
```
# <a name="c"></a>[<span data-ttu-id="d0644-134">C#</span><span class="sxs-lookup"><span data-stu-id="d0644-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentscheduleinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0644-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0644-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentscheduleinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0644-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0644-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentscheduleinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0644-137">Java</span><span class="sxs-lookup"><span data-stu-id="d0644-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentscheduleinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d0644-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0644-138">Response</span></span>
<span data-ttu-id="d0644-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d0644-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "principalId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "roleDefinitionId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "directoryScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "appScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "startDateTime": "2020-09-09T21:35:27.91Z",
    "endDateTime": "2020-09-09T21:35:27.91Z",
    "assignmentType": "eligible",
    "memberType": "direct",
    "roleAssignmentOriginId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
    "roleAssignmentScheduleId": "eb18c026-c026-eb18-26c0-18eb26c018eb"
  }
}
```

