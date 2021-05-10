---
title: Listar unifiedRoleAssignmentScheduleInstances
description: Obter uma lista dos objetos unifiedRoleAssignmentScheduleInstance e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b38fdad1f83e62b40ce2336492fe5f49e3bc1ff0
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299093"
---
# <a name="list-unifiedroleassignmentscheduleinstances"></a><span data-ttu-id="133a5-103">Listar unifiedRoleAssignmentScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="133a5-103">List unifiedRoleAssignmentScheduleInstances</span></span>
<span data-ttu-id="133a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="133a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="133a5-105">Obter uma lista dos [objetos unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="133a5-105">Get a list of the [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="133a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="133a5-106">Permissions</span></span>
<span data-ttu-id="133a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="133a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="133a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="133a5-109">Permission type</span></span>|<span data-ttu-id="133a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="133a5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="133a5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="133a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="133a5-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="133a5-112">RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="133a5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="133a5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="133a5-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="133a5-114">Not supported</span></span>|
|<span data-ttu-id="133a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="133a5-115">Application</span></span>|<span data-ttu-id="133a5-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="133a5-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="133a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="133a5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentScheduleInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="133a5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="133a5-118">Optional query parameters</span></span>
<span data-ttu-id="133a5-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="133a5-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="133a5-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="133a5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="133a5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="133a5-121">Request headers</span></span>
|<span data-ttu-id="133a5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="133a5-122">Name</span></span>|<span data-ttu-id="133a5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="133a5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="133a5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="133a5-124">Authorization</span></span>|<span data-ttu-id="133a5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="133a5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="133a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="133a5-127">Request body</span></span>
<span data-ttu-id="133a5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="133a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="133a5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="133a5-129">Response</span></span>

<span data-ttu-id="133a5-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="133a5-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="133a5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="133a5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="133a5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="133a5-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleInstances
```


### <a name="response"></a><span data-ttu-id="133a5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="133a5-133">Response</span></span>
<span data-ttu-id="133a5-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="133a5-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  ]
}
```

