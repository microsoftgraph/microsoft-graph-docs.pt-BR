---
title: 'unifiedRoleAssignmentSchedule: filterByCurrentUser'
description: Obter uma lista dos objetos unifiedRoleAssignmentSchedule e suas propriedades filtradas por uma entidade de usuário específica
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bc80dc68d8ff4133d481b23295f4826d85075213
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334483"
---
# <a name="unifiedroleassignmentschedule-filterbycurrentuser"></a><span data-ttu-id="cdb21-103">unifiedRoleAssignmentSchedule: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="cdb21-103">unifiedRoleAssignmentSchedule: filterByCurrentUser</span></span>
<span data-ttu-id="cdb21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdb21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdb21-105">Obter uma lista dos [objetos unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md) e suas propriedades associadas a um objeto principal específico.</span><span class="sxs-lookup"><span data-stu-id="cdb21-105">Get a list of the [unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdb21-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdb21-106">Permissions</span></span>
<span data-ttu-id="cdb21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdb21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdb21-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdb21-109">Permission type</span></span>|<span data-ttu-id="cdb21-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdb21-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdb21-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdb21-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdb21-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="cdb21-112">RoleAssignmentSchedule.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleAssignmentSchedule.ReadWrite.Directory</span></span>|
|<span data-ttu-id="cdb21-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdb21-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdb21-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cdb21-114">Not supported</span></span>|
|<span data-ttu-id="cdb21-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdb21-115">Application</span></span>|<span data-ttu-id="cdb21-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="cdb21-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdb21-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdb21-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="cdb21-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="cdb21-118">Query parameters</span></span>
<span data-ttu-id="cdb21-119">A tabela a seguir mostra os parâmetros de consulta que podem ser usados com esse método.</span><span class="sxs-lookup"><span data-stu-id="cdb21-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="cdb21-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cdb21-120">Parameter</span></span>|<span data-ttu-id="cdb21-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdb21-121">Type</span></span>|<span data-ttu-id="cdb21-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdb21-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdb21-123">on</span><span class="sxs-lookup"><span data-stu-id="cdb21-123">on</span></span>|<span data-ttu-id="cdb21-124">roleAssignmentScheduleFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="cdb21-124">roleAssignmentScheduleFilterByCurrentUserOptions</span></span>|<span data-ttu-id="cdb21-125">ID do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="cdb21-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="cdb21-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdb21-126">Request headers</span></span>
|<span data-ttu-id="cdb21-127">Nome</span><span class="sxs-lookup"><span data-stu-id="cdb21-127">Name</span></span>|<span data-ttu-id="cdb21-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdb21-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cdb21-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdb21-129">Authorization</span></span>|<span data-ttu-id="cdb21-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdb21-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdb21-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdb21-132">Request body</span></span>
<span data-ttu-id="cdb21-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cdb21-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdb21-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdb21-134">Response</span></span>

<span data-ttu-id="cdb21-135">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdb21-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdb21-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cdb21-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cdb21-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdb21-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedule_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules/filterByCurrentUser(on='dce468b2-68b2-dce4-b268-e4dcb268e4dc')
```


### <a name="response"></a><span data-ttu-id="cdb21-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdb21-138">Response</span></span>
<span data-ttu-id="cdb21-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cdb21-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "status": "Provisioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "assignmentType": "Eligible",
      "memberType": "direct"
    }
  ]
}
```

