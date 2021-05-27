---
title: 'unifiedRoleAssignmentScheduleInstance: filterByCurrentUser'
description: Obter uma lista dos objetos unifiedRoleAssignmentScheduleInstance e suas propriedades filtradas por uma entidade de usuário específica
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cd84a9e617f582eb01afe31cad28114f22e03432
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680322"
---
# <a name="unifiedroleassignmentscheduleinstance-filterbycurrentuser"></a><span data-ttu-id="e6463-103">unifiedRoleAssignmentScheduleInstance: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="e6463-103">unifiedRoleAssignmentScheduleInstance: filterByCurrentUser</span></span>
<span data-ttu-id="e6463-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6463-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6463-105">Obter uma lista dos [objetos unifiedRoleAssignmentScheduleInstance](../resources/unifiedRoleAssignmentScheduleInstance.md) e suas propriedades associadas a um objeto principal específico.</span><span class="sxs-lookup"><span data-stu-id="e6463-105">Get a list of the [unifiedRoleAssignmentScheduleInstance](../resources/unifiedRoleAssignmentScheduleInstance.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6463-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6463-106">Permissions</span></span>
<span data-ttu-id="e6463-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6463-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6463-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6463-109">Permission type</span></span>|<span data-ttu-id="e6463-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6463-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6463-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6463-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6463-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e6463-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="e6463-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6463-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6463-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e6463-114">Not supported</span></span>|
|<span data-ttu-id="e6463-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6463-115">Application</span></span>|<span data-ttu-id="e6463-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="e6463-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6463-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6463-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="e6463-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="e6463-118">Query parameters</span></span>
<span data-ttu-id="e6463-119">A tabela a seguir mostra os parâmetros que podem ser usados com esse método.</span><span class="sxs-lookup"><span data-stu-id="e6463-119">The following table shows the parameters that can be used with this method.</span></span>

|<span data-ttu-id="e6463-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6463-120">Parameter</span></span>|<span data-ttu-id="e6463-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6463-121">Type</span></span>|<span data-ttu-id="e6463-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6463-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6463-123">on</span><span class="sxs-lookup"><span data-stu-id="e6463-123">on</span></span>|<span data-ttu-id="e6463-124">roleAssignmentScheduleInstanceFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="e6463-124">roleAssignmentScheduleInstanceFilterByCurrentUserOptions</span></span>|<span data-ttu-id="e6463-125">ID do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="e6463-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="e6463-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6463-126">Request headers</span></span>
|<span data-ttu-id="e6463-127">Nome</span><span class="sxs-lookup"><span data-stu-id="e6463-127">Name</span></span>|<span data-ttu-id="e6463-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6463-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e6463-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6463-129">Authorization</span></span>|<span data-ttu-id="e6463-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6463-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6463-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6463-132">Request body</span></span>
<span data-ttu-id="e6463-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6463-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6463-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6463-134">Response</span></span>

<span data-ttu-id="e6463-135">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6463-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6463-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e6463-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e6463-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6463-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentscheduleinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances/unifiedRoleAssignmentScheduleInstances/filterByCurrentUser(on='dce468b2-68b2-dce4-b268-e4dcb268e4dc')
```


### <a name="response"></a><span data-ttu-id="e6463-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6463-138">Response</span></span>
<span data-ttu-id="e6463-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e6463-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "principalId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "roleDefinitionId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "directoryScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "appScopeId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "startDateTime": "2020-09-09T21:35:27.91Z",
      "endDateTime": "2020-09-09T21:35:27.91Z",
      "assignmentType": "eligible",
      "memberType": "direct",
      "roleAssignmentOriginId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc",
      "roleAssignmentScheduleId": "dce468b2-68b2-dce4-b268-e4dcb268e4dc"
    }
  ]
}
```

