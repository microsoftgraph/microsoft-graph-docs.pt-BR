---
title: 'unifiedRoleAssignmentSchedule: filterByCurrentUser'
description: Obter uma lista dos objetos unifiedRoleAssignmentSchedule e suas propriedades filtradas por uma entidade de usuário específica
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7330dc3126a8ce4ba0428475d8ab21ee2f302835
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299031"
---
# <a name="unifiedroleassignmentschedule-filterbycurrentuser"></a><span data-ttu-id="31ef7-103">unifiedRoleAssignmentSchedule: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="31ef7-103">unifiedRoleAssignmentSchedule: filterByCurrentUser</span></span>
<span data-ttu-id="31ef7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31ef7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31ef7-105">Obter uma lista dos [objetos unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md) e suas propriedades associadas a um objeto principal específico.</span><span class="sxs-lookup"><span data-stu-id="31ef7-105">Get a list of the [unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31ef7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31ef7-106">Permissions</span></span>
<span data-ttu-id="31ef7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31ef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31ef7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31ef7-109">Permission type</span></span>|<span data-ttu-id="31ef7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31ef7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31ef7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31ef7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31ef7-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="31ef7-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="31ef7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31ef7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31ef7-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="31ef7-114">Not supported</span></span>|
|<span data-ttu-id="31ef7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31ef7-115">Application</span></span>|<span data-ttu-id="31ef7-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="31ef7-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="31ef7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31ef7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="31ef7-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="31ef7-118">Query parameters</span></span>
<span data-ttu-id="31ef7-119">A tabela a seguir mostra os parâmetros de consulta que podem ser usados com esse método.</span><span class="sxs-lookup"><span data-stu-id="31ef7-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="31ef7-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="31ef7-120">Parameter</span></span>|<span data-ttu-id="31ef7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="31ef7-121">Type</span></span>|<span data-ttu-id="31ef7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="31ef7-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31ef7-123">on</span><span class="sxs-lookup"><span data-stu-id="31ef7-123">on</span></span>|<span data-ttu-id="31ef7-124">roleAssignmentScheduleFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="31ef7-124">roleAssignmentScheduleFilterByCurrentUserOptions</span></span>|<span data-ttu-id="31ef7-125">ID do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="31ef7-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="31ef7-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31ef7-126">Request headers</span></span>
|<span data-ttu-id="31ef7-127">Nome</span><span class="sxs-lookup"><span data-stu-id="31ef7-127">Name</span></span>|<span data-ttu-id="31ef7-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="31ef7-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="31ef7-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="31ef7-129">Authorization</span></span>|<span data-ttu-id="31ef7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31ef7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31ef7-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31ef7-132">Request body</span></span>
<span data-ttu-id="31ef7-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31ef7-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31ef7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="31ef7-134">Response</span></span>

<span data-ttu-id="31ef7-135">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31ef7-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31ef7-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="31ef7-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31ef7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31ef7-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedule_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules/filterByCurrentUser(on='dce468b2-68b2-dce4-b268-e4dcb268e4dc')
```


### <a name="response"></a><span data-ttu-id="31ef7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="31ef7-138">Response</span></span>
<span data-ttu-id="31ef7-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="31ef7-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

