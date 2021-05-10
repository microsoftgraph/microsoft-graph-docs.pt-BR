---
title: Obter unifiedRoleAssignmentScheduleRequest
description: Leia as propriedades e as relações de um objeto unifiedRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f03d053979f8821296a9a3e59e6c7fdd0372735f
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299085"
---
# <a name="get-unifiedroleassignmentschedulerequest"></a><span data-ttu-id="e8984-103">Obter unifiedRoleAssignmentScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="e8984-103">Get unifiedRoleAssignmentScheduleRequest</span></span>
<span data-ttu-id="e8984-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8984-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8984-105">Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleRequest.](../resources/unifiedroleassignmentschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="e8984-105">Read the properties and relationships of an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8984-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8984-106">Permissions</span></span>
<span data-ttu-id="e8984-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8984-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8984-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8984-109">Permission type</span></span>|<span data-ttu-id="e8984-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8984-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8984-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8984-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8984-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e8984-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="e8984-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8984-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8984-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e8984-114">Not supported</span></span>|
|<span data-ttu-id="e8984-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8984-115">Application</span></span>|<span data-ttu-id="e8984-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e8984-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8984-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8984-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8984-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8984-118">Optional query parameters</span></span>
<span data-ttu-id="e8984-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8984-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8984-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8984-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8984-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8984-121">Request headers</span></span>
|<span data-ttu-id="e8984-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e8984-122">Name</span></span>|<span data-ttu-id="e8984-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8984-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8984-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8984-124">Authorization</span></span>|<span data-ttu-id="e8984-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8984-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8984-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8984-127">Request body</span></span>
<span data-ttu-id="e8984-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8984-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8984-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8984-129">Response</span></span>

<span data-ttu-id="e8984-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8984-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8984-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8984-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8984-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8984-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}
```


### <a name="response"></a><span data-ttu-id="e8984-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8984-133">Response</span></span>
<span data-ttu-id="e8984-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8984-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

