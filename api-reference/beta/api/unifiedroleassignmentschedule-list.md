---
title: Listar unifiedRoleAssignmentSchedules
description: Obter uma lista dos objetos unifiedRoleAssignmentSchedule e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 26c52cfa2d305f23783c384deb1f2cd09c289db6
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334476"
---
# <a name="list-unifiedroleassignmentschedules"></a><span data-ttu-id="557de-103">Listar unifiedRoleAssignmentSchedules</span><span class="sxs-lookup"><span data-stu-id="557de-103">List unifiedRoleAssignmentSchedules</span></span>
<span data-ttu-id="557de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="557de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="557de-105">Obter uma lista dos [objetos unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="557de-105">Get a list of the [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="557de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="557de-106">Permissions</span></span>
<span data-ttu-id="557de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="557de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="557de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="557de-109">Permission type</span></span>|<span data-ttu-id="557de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="557de-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="557de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="557de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="557de-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="557de-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span></span>   |
|<span data-ttu-id="557de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="557de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="557de-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="557de-114">Not supported</span></span>|
|<span data-ttu-id="557de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="557de-115">Application</span></span>|<span data-ttu-id="557de-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="557de-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="557de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="557de-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="557de-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="557de-118">Optional query parameters</span></span>
<span data-ttu-id="557de-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="557de-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="557de-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="557de-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="557de-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="557de-121">Request headers</span></span>
|<span data-ttu-id="557de-122">Nome</span><span class="sxs-lookup"><span data-stu-id="557de-122">Name</span></span>|<span data-ttu-id="557de-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="557de-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="557de-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="557de-124">Authorization</span></span>|<span data-ttu-id="557de-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="557de-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="557de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="557de-127">Request body</span></span>
<span data-ttu-id="557de-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="557de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="557de-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="557de-129">Response</span></span>

<span data-ttu-id="557de-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="557de-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="557de-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="557de-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="557de-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="557de-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="557de-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="557de-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules
```
# <a name="c"></a>[<span data-ttu-id="557de-134">C#</span><span class="sxs-lookup"><span data-stu-id="557de-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleassignmentschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="557de-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="557de-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleassignmentschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="557de-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="557de-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleassignmentschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="557de-137">Java</span><span class="sxs-lookup"><span data-stu-id="557de-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleassignmentschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="557de-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="557de-138">Response</span></span>
<span data-ttu-id="557de-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="557de-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentSchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "principalId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "roleDefinitionId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "directoryScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "appScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "createdUsing": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "createdDateTime": "2020-09-09T21:35:27.91Z",
      "modifiedDateTime": "2020-09-09T21:35:27.91Z",
      "status": "Provsioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "assignmentType": "eligible",
      "memberType": "direct"
    }
  ]
}
```

