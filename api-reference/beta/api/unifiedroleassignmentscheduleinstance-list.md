---
title: Listar unifiedRoleAssignmentScheduleInstances
description: Obter uma lista dos objetos unifiedRoleAssignmentScheduleInstance e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e012b422498e7029bc6f205ff0878b9b5e9093fb
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680504"
---
# <a name="list-unifiedroleassignmentscheduleinstances"></a><span data-ttu-id="5e3d8-103">Listar unifiedRoleAssignmentScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="5e3d8-103">List unifiedRoleAssignmentScheduleInstances</span></span>
<span data-ttu-id="5e3d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e3d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e3d8-105">Obter uma lista dos [objetos unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="5e3d8-105">Get a list of the [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e3d8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e3d8-106">Permissions</span></span>
<span data-ttu-id="5e3d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e3d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e3d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e3d8-109">Permission type</span></span>|<span data-ttu-id="5e3d8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e3d8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e3d8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e3d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5e3d8-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="5e3d8-112">RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="5e3d8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e3d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e3d8-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5e3d8-114">Not supported</span></span>|
|<span data-ttu-id="5e3d8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e3d8-115">Application</span></span>|<span data-ttu-id="5e3d8-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="5e3d8-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e3d8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e3d8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e3d8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5e3d8-118">Optional query parameters</span></span>
<span data-ttu-id="5e3d8-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5e3d8-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5e3d8-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5e3d8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e3d8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e3d8-121">Request headers</span></span>
|<span data-ttu-id="5e3d8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5e3d8-122">Name</span></span>|<span data-ttu-id="5e3d8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e3d8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5e3d8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e3d8-124">Authorization</span></span>|<span data-ttu-id="5e3d8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e3d8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e3d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e3d8-127">Request body</span></span>
<span data-ttu-id="5e3d8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e3d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e3d8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e3d8-129">Response</span></span>

<span data-ttu-id="5e3d8-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e3d8-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e3d8-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5e3d8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e3d8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e3d8-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5e3d8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e3d8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances
```
# <a name="c"></a>[<span data-ttu-id="5e3d8-134">C#</span><span class="sxs-lookup"><span data-stu-id="5e3d8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentscheduleinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e3d8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e3d8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentscheduleinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e3d8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e3d8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentscheduleinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e3d8-137">Java</span><span class="sxs-lookup"><span data-stu-id="5e3d8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentscheduleinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5e3d8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e3d8-138">Response</span></span>
<span data-ttu-id="5e3d8-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5e3d8-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

