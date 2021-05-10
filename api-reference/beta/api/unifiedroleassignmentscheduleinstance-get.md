---
title: Obter unifiedRoleAssignmentScheduleInstance
description: Leia as propriedades e as relações de um objeto unifiedRoleAssignmentScheduleInstance.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b56dcc6f0171a203a426e88c8c01a81e71a10986
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299094"
---
# <a name="get-unifiedroleassignmentscheduleinstance"></a><span data-ttu-id="1c009-103">Obter unifiedRoleAssignmentScheduleInstance</span><span class="sxs-lookup"><span data-stu-id="1c009-103">Get unifiedRoleAssignmentScheduleInstance</span></span>
<span data-ttu-id="1c009-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c009-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c009-105">Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleInstance.](../resources/unifiedroleassignmentscheduleinstance.md)</span><span class="sxs-lookup"><span data-stu-id="1c009-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c009-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c009-106">Permissions</span></span>
<span data-ttu-id="1c009-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c009-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c009-109">Permission type</span></span>|<span data-ttu-id="1c009-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c009-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c009-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c009-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c009-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="1c009-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="1c009-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c009-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c009-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1c009-114">Not supported</span></span>|
|<span data-ttu-id="1c009-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c009-115">Application</span></span>|<span data-ttu-id="1c009-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="1c009-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c009-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c009-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/{unifiedRoleAssignmentScheduleInstancesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c009-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c009-118">Optional query parameters</span></span>
<span data-ttu-id="1c009-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c009-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1c009-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1c009-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c009-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c009-121">Request headers</span></span>
|<span data-ttu-id="1c009-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1c009-122">Name</span></span>|<span data-ttu-id="1c009-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c009-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1c009-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c009-124">Authorization</span></span>|<span data-ttu-id="1c009-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c009-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c009-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c009-127">Request body</span></span>
<span data-ttu-id="1c009-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c009-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c009-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c009-129">Response</span></span>

<span data-ttu-id="1c009-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c009-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c009-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c009-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c009-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c009-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/unifiedRoleAssignmentScheduleInstances/eb18c026-c026-eb18-26c0-18eb26c018eb
```


### <a name="response"></a><span data-ttu-id="1c009-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c009-133">Response</span></span>
<span data-ttu-id="1c009-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c009-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

