---
title: 'unifiedRoleAssignmentScheduleRequest: filterByCurrentUser'
description: Obter uma lista dos objetos unifiedRoleAssignmentScheduleRequest e suas propriedades filtradas por uma entidade de usuário específica
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f30a2e8a7c1ac1440291d4e9e7849637c20e3be3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680273"
---
# <a name="unifiedroleassignmentschedulerequest-filterbycurrentuser"></a><span data-ttu-id="fb500-103">unifiedRoleAssignmentScheduleRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="fb500-103">unifiedRoleAssignmentScheduleRequest: filterByCurrentUser</span></span>
<span data-ttu-id="fb500-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb500-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="fb500-105">Obter uma lista dos [objetos unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) e suas propriedades associadas a um objeto principal específico.</span><span class="sxs-lookup"><span data-stu-id="fb500-105">Get a list of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb500-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb500-106">Permissions</span></span>
<span data-ttu-id="fb500-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb500-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb500-109">Permission type</span></span>|<span data-ttu-id="fb500-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb500-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb500-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb500-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb500-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="fb500-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="fb500-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb500-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb500-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fb500-114">Not supported</span></span>|
|<span data-ttu-id="fb500-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb500-115">Application</span></span>|<span data-ttu-id="fb500-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="fb500-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb500-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb500-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="fb500-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="fb500-118">Query parameters</span></span>
<span data-ttu-id="fb500-119">A tabela a seguir mostra os parâmetros de consulta que podem ser usados com esse método.</span><span class="sxs-lookup"><span data-stu-id="fb500-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="fb500-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fb500-120">Parameter</span></span>|<span data-ttu-id="fb500-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb500-121">Type</span></span>|<span data-ttu-id="fb500-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb500-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb500-123">on</span><span class="sxs-lookup"><span data-stu-id="fb500-123">on</span></span>|<span data-ttu-id="fb500-124">RoleAssignmentScheduleRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="fb500-124">RoleAssignmentScheduleRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="fb500-125">ID do objeto principal.</span><span class="sxs-lookup"><span data-stu-id="fb500-125">Id of the principal object.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="fb500-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb500-126">Request headers</span></span>
|<span data-ttu-id="fb500-127">Nome</span><span class="sxs-lookup"><span data-stu-id="fb500-127">Name</span></span>|<span data-ttu-id="fb500-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb500-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fb500-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb500-129">Authorization</span></span>|<span data-ttu-id="fb500-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb500-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb500-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb500-132">Request body</span></span>
<span data-ttu-id="fb500-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb500-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb500-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb500-134">Response</span></span>

<span data-ttu-id="fb500-135">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [unifiedRoleAssignmentScheduleRequest](../resources/unifiedRoleAssignmentScheduleRequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb500-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleAssignmentScheduleRequest](../resources/unifiedRoleAssignmentScheduleRequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb500-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb500-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb500-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb500-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/RoleAssignmentScheduleRequests/filterByCurrentUser(on='d6e4112f-112f-d6e4-2f11-e4d62f11e4d6')
```


### <a name="response"></a><span data-ttu-id="fb500-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb500-138">Response</span></span>
<span data-ttu-id="fb500-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb500-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "action": "AdminAssign",
      "principalId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "roleDefinitionId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "directoryScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "appScopeId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "isValidationOnly": false,
      "targetScheduleId": "b1477448-2cc6-4ceb-93b4-54a202a89413",
      "justification": "this is a justification",
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

