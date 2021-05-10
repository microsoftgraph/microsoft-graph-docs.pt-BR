---
title: Listar unifiedRoleEligibilityScheduleRequests
description: Obter uma lista dos objetos unifiedRoleEligibilityScheduleRequest e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3ff80105188d8106528805cf92b8300db25fdcec
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299072"
---
# <a name="list-unifiedroleeligibilityschedulerequests"></a><span data-ttu-id="a2e73-103">Listar unifiedRoleEligibilityScheduleRequests</span><span class="sxs-lookup"><span data-stu-id="a2e73-103">List unifiedRoleEligibilityScheduleRequests</span></span>
<span data-ttu-id="a2e73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2e73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2e73-105">Obter uma lista dos [objetos unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="a2e73-105">Get a list of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2e73-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2e73-106">Permissions</span></span>
<span data-ttu-id="a2e73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2e73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2e73-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2e73-109">Permission type</span></span>|<span data-ttu-id="a2e73-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2e73-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2e73-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2e73-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a2e73-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a2e73-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="a2e73-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2e73-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2e73-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a2e73-114">Not supported</span></span>|
|<span data-ttu-id="a2e73-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2e73-115">Application</span></span>|<span data-ttu-id="a2e73-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a2e73-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2e73-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2e73-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2e73-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a2e73-118">Optional query parameters</span></span>
<span data-ttu-id="a2e73-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a2e73-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a2e73-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a2e73-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2e73-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e73-121">Request headers</span></span>
|<span data-ttu-id="a2e73-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a2e73-122">Name</span></span>|<span data-ttu-id="a2e73-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2e73-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a2e73-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2e73-124">Authorization</span></span>|<span data-ttu-id="a2e73-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2e73-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2e73-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e73-127">Request body</span></span>
<span data-ttu-id="a2e73-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2e73-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2e73-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2e73-129">Response</span></span>

<span data-ttu-id="a2e73-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2e73-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2e73-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a2e73-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a2e73-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2e73-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityschedulerequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
```


### <a name="response"></a><span data-ttu-id="a2e73-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2e73-133">Response</span></span>
<span data-ttu-id="a2e73-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a2e73-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

