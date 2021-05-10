---
title: Listar unifiedRoleAssignmentSchedules
description: Obter uma lista dos objetos unifiedRoleAssignmentSchedule e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 687c8ea9ff283625c6eabc7b7746e60d572551c7
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299026"
---
# <a name="list-unifiedroleassignmentschedules"></a><span data-ttu-id="3c100-103">Listar unifiedRoleAssignmentSchedules</span><span class="sxs-lookup"><span data-stu-id="3c100-103">List unifiedRoleAssignmentSchedules</span></span>
<span data-ttu-id="3c100-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c100-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c100-105">Obter uma lista dos [objetos unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="3c100-105">Get a list of the [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c100-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c100-106">Permissions</span></span>
<span data-ttu-id="3c100-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c100-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c100-109">Permission type</span></span>|<span data-ttu-id="3c100-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c100-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c100-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c100-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c100-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="3c100-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="3c100-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c100-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c100-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3c100-114">Not supported</span></span>|
|<span data-ttu-id="3c100-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c100-115">Application</span></span>|<span data-ttu-id="3c100-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="3c100-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c100-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c100-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleAssignmentSchedules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c100-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c100-118">Optional query parameters</span></span>
<span data-ttu-id="3c100-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c100-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3c100-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3c100-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c100-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c100-121">Request headers</span></span>
|<span data-ttu-id="3c100-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3c100-122">Name</span></span>|<span data-ttu-id="3c100-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c100-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3c100-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c100-124">Authorization</span></span>|<span data-ttu-id="3c100-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c100-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c100-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c100-127">Request body</span></span>
<span data-ttu-id="3c100-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c100-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c100-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c100-129">Response</span></span>

<span data-ttu-id="3c100-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c100-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c100-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3c100-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c100-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c100-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules
```


### <a name="response"></a><span data-ttu-id="3c100-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c100-133">Response</span></span>
<span data-ttu-id="3c100-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c100-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "status": "Provsioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "assignmentType": "eligible",
      "memberType": "direct"
    }
  ]
}
```

