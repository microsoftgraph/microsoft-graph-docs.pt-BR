---
title: Listar unifiedRoleAssignmentScheduleInstances
description: Obter uma lista dos objetos unifiedRoleAssignmentScheduleInstance e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 382c5a7ff8b75da06f1d75b06a2bb382137c275d
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334385"
---
# <a name="list-unifiedroleassignmentscheduleinstances"></a><span data-ttu-id="fcf30-103">Listar unifiedRoleAssignmentScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="fcf30-103">List unifiedRoleAssignmentScheduleInstances</span></span>
<span data-ttu-id="fcf30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcf30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcf30-105">Obter uma lista dos [objetos unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="fcf30-105">Get a list of the [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcf30-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fcf30-106">Permissions</span></span>
<span data-ttu-id="fcf30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcf30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcf30-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcf30-109">Permission type</span></span>|<span data-ttu-id="fcf30-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fcf30-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcf30-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcf30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fcf30-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="fcf30-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="fcf30-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcf30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcf30-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fcf30-114">Not supported</span></span>|
|<span data-ttu-id="fcf30-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcf30-115">Application</span></span>|<span data-ttu-id="fcf30-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="fcf30-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcf30-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcf30-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcf30-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fcf30-118">Optional query parameters</span></span>
<span data-ttu-id="fcf30-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fcf30-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fcf30-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fcf30-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcf30-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf30-121">Request headers</span></span>
|<span data-ttu-id="fcf30-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fcf30-122">Name</span></span>|<span data-ttu-id="fcf30-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcf30-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fcf30-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcf30-124">Authorization</span></span>|<span data-ttu-id="fcf30-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcf30-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcf30-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf30-127">Request body</span></span>
<span data-ttu-id="fcf30-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fcf30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcf30-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf30-129">Response</span></span>

<span data-ttu-id="fcf30-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcf30-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fcf30-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fcf30-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fcf30-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf30-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fcf30-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcf30-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances
```
# <a name="c"></a>[<span data-ttu-id="fcf30-134">C#</span><span class="sxs-lookup"><span data-stu-id="fcf30-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentscheduleinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcf30-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcf30-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentscheduleinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcf30-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcf30-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentscheduleinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fcf30-137">Java</span><span class="sxs-lookup"><span data-stu-id="fcf30-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentscheduleinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fcf30-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf30-138">Response</span></span>
<span data-ttu-id="fcf30-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fcf30-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```

