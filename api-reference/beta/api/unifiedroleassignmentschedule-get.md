---
title: Obter unifiedRoleAssignmentSchedule
description: Leia as propriedades e as relações de um objeto unifiedRoleAssignmentSchedule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 939ae40260ed127fe36089db5874c7c880b8f8d4
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351017"
---
# <a name="get-unifiedroleassignmentschedule"></a><span data-ttu-id="0a66e-103">Obter unifiedRoleAssignmentSchedule</span><span class="sxs-lookup"><span data-stu-id="0a66e-103">Get unifiedRoleAssignmentSchedule</span></span>
<span data-ttu-id="0a66e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a66e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a66e-105">Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentSchedule.](../resources/unifiedroleassignmentschedule.md)</span><span class="sxs-lookup"><span data-stu-id="0a66e-105">Read the properties and relationships of an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a66e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a66e-106">Permissions</span></span>
<span data-ttu-id="0a66e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a66e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a66e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a66e-109">Permission type</span></span>|<span data-ttu-id="0a66e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a66e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a66e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a66e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a66e-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="0a66e-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span></span>|
|<span data-ttu-id="0a66e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a66e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a66e-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0a66e-114">Not supported</span></span>|
|<span data-ttu-id="0a66e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a66e-115">Application</span></span>|<span data-ttu-id="0a66e-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="0a66e-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a66e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a66e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules/{unifiedRoleAssignmentSchedulesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a66e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a66e-118">Optional query parameters</span></span>
<span data-ttu-id="0a66e-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a66e-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0a66e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0a66e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a66e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a66e-121">Request headers</span></span>
|<span data-ttu-id="0a66e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0a66e-122">Name</span></span>|<span data-ttu-id="0a66e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a66e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0a66e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a66e-124">Authorization</span></span>|<span data-ttu-id="0a66e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a66e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a66e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a66e-127">Request body</span></span>
<span data-ttu-id="0a66e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a66e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a66e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a66e-129">Response</span></span>

<span data-ttu-id="0a66e-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a66e-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a66e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0a66e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a66e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a66e-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules/b1477448-2cc6-4ceb-93b4-54a202a89413
```


### <a name="response"></a><span data-ttu-id="0a66e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a66e-133">Response</span></span>
<span data-ttu-id="0a66e-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0a66e-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "principalId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "roleDefinitionId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "directoryScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "appScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "createdUsing": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
    "createdDateTime": "2020-09-09T21:35:27.91Z",
    "modifiedDateTime": "2020-09-09T21:35:27.91Z",
    "status": "Provisioned",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    },
    "assignmentType": "Eligible",
    "memberType": "direct"
  }
}
```

