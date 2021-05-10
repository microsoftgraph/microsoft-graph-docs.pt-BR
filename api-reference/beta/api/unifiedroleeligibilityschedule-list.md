---
title: Listar unifiedRoleEligibilitySchedules
description: Obter uma lista dos objetos unifiedRoleEligibilitySchedule e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6d4a2c4ad3475b0f5a6a12f43248213cf3cf56af
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298997"
---
# <a name="list-unifiedroleeligibilityschedules"></a><span data-ttu-id="2a7d6-103">Listar unifiedRoleEligibilitySchedules</span><span class="sxs-lookup"><span data-stu-id="2a7d6-103">List unifiedRoleEligibilitySchedules</span></span>
<span data-ttu-id="2a7d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a7d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a7d6-105">Obter uma lista dos [objetos unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="2a7d6-105">Get a list of the [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a7d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a7d6-106">Permissions</span></span>
<span data-ttu-id="2a7d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a7d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a7d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a7d6-109">Permission type</span></span>|<span data-ttu-id="2a7d6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a7d6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a7d6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a7d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a7d6-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="2a7d6-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="2a7d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a7d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a7d6-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2a7d6-114">Not supported</span></span>|
|<span data-ttu-id="2a7d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a7d6-115">Application</span></span>|<span data-ttu-id="2a7d6-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="2a7d6-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a7d6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a7d6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilitySchedules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a7d6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a7d6-118">Optional query parameters</span></span>
<span data-ttu-id="2a7d6-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a7d6-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2a7d6-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2a7d6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a7d6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a7d6-121">Request headers</span></span>
|<span data-ttu-id="2a7d6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2a7d6-122">Name</span></span>|<span data-ttu-id="2a7d6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a7d6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2a7d6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a7d6-124">Authorization</span></span>|<span data-ttu-id="2a7d6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a7d6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a7d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a7d6-127">Request body</span></span>
<span data-ttu-id="2a7d6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a7d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a7d6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a7d6-129">Response</span></span>

<span data-ttu-id="2a7d6-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a7d6-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a7d6-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2a7d6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a7d6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a7d6-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules
```


### <a name="response"></a><span data-ttu-id="2a7d6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a7d6-133">Response</span></span>
<span data-ttu-id="2a7d6-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2a7d6-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilitySchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "createdUsing": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "createdDateTime": "2020-09-09T21:35:27.91Z",
      "modifiedDateTime": "2020-09-09T21:35:27.91Z",
      "status": "Provisioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "memberType": "direct"
    }
  ]
}
```

