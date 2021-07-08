---
title: 'unifiedRoleEligibilityScheduleRequest: filterByCurrentUser'
description: Obter uma lista dos objetos unifiedRoleEligibilityScheduleRequest e suas propriedades filtradas por uma entidade de usuário específica
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8ad251e390eae9f328b425c1083f189d5c6989a5
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334672"
---
# <a name="unifiedroleeligibilityschedulerequest-filterbycurrentuser"></a><span data-ttu-id="f0937-103">unifiedRoleEligibilityScheduleRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="f0937-103">unifiedRoleEligibilityScheduleRequest: filterByCurrentUser</span></span>
<span data-ttu-id="f0937-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0937-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0937-105">Obter uma lista dos [objetos unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) e suas propriedades associadas a um objeto principal específico.</span><span class="sxs-lookup"><span data-stu-id="f0937-105">Get a list of the [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0937-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0937-106">Permissions</span></span>
<span data-ttu-id="f0937-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0937-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0937-109">Permission type</span></span>|<span data-ttu-id="f0937-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0937-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0937-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0937-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0937-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="f0937-112">RoleEligibilitySchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleEligibilitySchedule.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span> |
|<span data-ttu-id="f0937-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0937-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0937-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f0937-114">Not supported</span></span>|
|<span data-ttu-id="f0937-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0937-115">Application</span></span>|<span data-ttu-id="f0937-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="f0937-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0937-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0937-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/RoleEligibilityScheduleRequests/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="f0937-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f0937-118">Function parameters</span></span>
<span data-ttu-id="f0937-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="f0937-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f0937-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="f0937-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f0937-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f0937-121">Parameter</span></span>|<span data-ttu-id="f0937-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0937-122">Type</span></span>|<span data-ttu-id="f0937-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0937-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0937-124">on</span><span class="sxs-lookup"><span data-stu-id="f0937-124">on</span></span>|<span data-ttu-id="f0937-125">RoleEligibilityScheduleRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="f0937-125">RoleEligibilityScheduleRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="f0937-126">ID do objeto principal</span><span class="sxs-lookup"><span data-stu-id="f0937-126">ID of the principal object</span></span>|


## <a name="request-headers"></a><span data-ttu-id="f0937-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0937-127">Request headers</span></span>
|<span data-ttu-id="f0937-128">Nome</span><span class="sxs-lookup"><span data-stu-id="f0937-128">Name</span></span>|<span data-ttu-id="f0937-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0937-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f0937-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0937-130">Authorization</span></span>|<span data-ttu-id="f0937-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0937-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0937-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0937-133">Request body</span></span>
<span data-ttu-id="f0937-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0937-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0937-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0937-135">Response</span></span>

<span data-ttu-id="f0937-136">Se tiver êxito, essa função retornará um código de resposta e uma coleção `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0937-136">If successful, this function returns a `200 OK` response code and a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0937-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0937-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0937-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0937-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedRoleEligibilityScheduleRequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/RoleEligibilityScheduleRequests/filterByCurrentUser(on='parameterValue')
```


### <a name="response"></a><span data-ttu-id="f0937-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0937-139">Response</span></span>
<span data-ttu-id="f0937-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f0937-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "String (identifier)",
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

