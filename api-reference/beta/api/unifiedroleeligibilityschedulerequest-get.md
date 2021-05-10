---
title: Obter unifiedRoleEligibilityScheduleRequest
description: Leia as propriedades e as relações de um objeto unifiedRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0ea5ed510740770b6103275d89d03c01c65e77f6
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299073"
---
# <a name="get-unifiedroleeligibilityschedulerequest"></a><span data-ttu-id="6174f-103">Obter unifiedRoleEligibilityScheduleRequest</span><span class="sxs-lookup"><span data-stu-id="6174f-103">Get unifiedRoleEligibilityScheduleRequest</span></span>
<span data-ttu-id="6174f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6174f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6174f-105">Leia as propriedades e as relações de [um objeto unifiedRoleEligibilityScheduleRequest.](../resources/unifiedroleeligibilityschedulerequest.md)</span><span class="sxs-lookup"><span data-stu-id="6174f-105">Read the properties and relationships of an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6174f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6174f-106">Permissions</span></span>
<span data-ttu-id="6174f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6174f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6174f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6174f-109">Permission type</span></span>|<span data-ttu-id="6174f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6174f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6174f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6174f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6174f-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6174f-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="6174f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6174f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6174f-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6174f-114">Not supported</span></span>|
|<span data-ttu-id="6174f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6174f-115">Application</span></span>|<span data-ttu-id="6174f-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="6174f-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="6174f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6174f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6174f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6174f-118">Optional query parameters</span></span>
<span data-ttu-id="6174f-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6174f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6174f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6174f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6174f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6174f-121">Request headers</span></span>
|<span data-ttu-id="6174f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6174f-122">Name</span></span>|<span data-ttu-id="6174f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6174f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6174f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6174f-124">Authorization</span></span>|<span data-ttu-id="6174f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6174f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6174f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6174f-127">Request body</span></span>
<span data-ttu-id="6174f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6174f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6174f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6174f-129">Response</span></span>

<span data-ttu-id="6174f-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6174f-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6174f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6174f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6174f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6174f-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```


### <a name="response"></a><span data-ttu-id="6174f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6174f-133">Response</span></span>
<span data-ttu-id="6174f-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6174f-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

