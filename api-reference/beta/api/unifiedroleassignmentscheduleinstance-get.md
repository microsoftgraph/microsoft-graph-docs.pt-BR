---
title: Obter unifiedRoleAssignmentScheduleInstance
description: Leia as propriedades e as relações de um objeto unifiedRoleAssignmentScheduleInstance.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f9c20f8fd4aefb7ffe9f68da9adacabe177e4065
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334455"
---
# <a name="get-unifiedroleassignmentscheduleinstance"></a><span data-ttu-id="40fea-103">Obter unifiedRoleAssignmentScheduleInstance</span><span class="sxs-lookup"><span data-stu-id="40fea-103">Get unifiedRoleAssignmentScheduleInstance</span></span>
<span data-ttu-id="40fea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40fea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40fea-105">Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleInstance.](../resources/unifiedroleassignmentscheduleinstance.md)</span><span class="sxs-lookup"><span data-stu-id="40fea-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40fea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="40fea-106">Permissions</span></span>
<span data-ttu-id="40fea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40fea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40fea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40fea-109">Permission type</span></span>|<span data-ttu-id="40fea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40fea-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40fea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40fea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40fea-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="40fea-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="40fea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40fea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40fea-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="40fea-114">Not supported</span></span>|
|<span data-ttu-id="40fea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40fea-115">Application</span></span>|<span data-ttu-id="40fea-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="40fea-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="40fea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40fea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstancesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40fea-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40fea-118">Optional query parameters</span></span>
<span data-ttu-id="40fea-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40fea-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="40fea-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="40fea-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="40fea-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40fea-121">Request headers</span></span>
|<span data-ttu-id="40fea-122">Nome</span><span class="sxs-lookup"><span data-stu-id="40fea-122">Name</span></span>|<span data-ttu-id="40fea-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="40fea-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="40fea-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="40fea-124">Authorization</span></span>|<span data-ttu-id="40fea-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40fea-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40fea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40fea-127">Request body</span></span>
<span data-ttu-id="40fea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40fea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40fea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="40fea-129">Response</span></span>

<span data-ttu-id="40fea-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40fea-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40fea-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="40fea-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40fea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40fea-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/unifiedRoleAssignmentScheduleInstances/eb18c026-c026-eb18-26c0-18eb26c018eb
```


### <a name="response"></a><span data-ttu-id="40fea-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="40fea-133">Response</span></span>
<span data-ttu-id="40fea-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40fea-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

