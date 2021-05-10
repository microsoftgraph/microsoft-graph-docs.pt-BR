---
title: Obter unifiedRoleEligibilityScheduleInstance
description: Leia as propriedades e as relações de um objeto unifiedRoleEligibilityScheduleInstance.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: adf95e156e4750add6f0763be17b122a3ebaf489
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299000"
---
# <a name="get-unifiedroleeligibilityscheduleinstance"></a><span data-ttu-id="ff9e0-103">Obter unifiedRoleEligibilityScheduleInstance</span><span class="sxs-lookup"><span data-stu-id="ff9e0-103">Get unifiedRoleEligibilityScheduleInstance</span></span>
<span data-ttu-id="ff9e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff9e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff9e0-105">Leia as propriedades e as relações de [um objeto unifiedRoleEligibilityScheduleInstance.](../resources/unifiedroleeligibilityscheduleinstance.md)</span><span class="sxs-lookup"><span data-stu-id="ff9e0-105">Read the properties and relationships of an [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff9e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff9e0-106">Permissions</span></span>
<span data-ttu-id="ff9e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff9e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff9e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff9e0-109">Permission type</span></span>|<span data-ttu-id="ff9e0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff9e0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff9e0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff9e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff9e0-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ff9e0-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="ff9e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff9e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff9e0-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ff9e0-114">Not supported</span></span>|
|<span data-ttu-id="ff9e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff9e0-115">Application</span></span>|<span data-ttu-id="ff9e0-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ff9e0-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff9e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff9e0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleInstances/{unifiedRoleEligibilityScheduleInstancesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff9e0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ff9e0-118">Optional query parameters</span></span>
<span data-ttu-id="ff9e0-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff9e0-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ff9e0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ff9e0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff9e0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff9e0-121">Request headers</span></span>
|<span data-ttu-id="ff9e0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ff9e0-122">Name</span></span>|<span data-ttu-id="ff9e0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff9e0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ff9e0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff9e0-124">Authorization</span></span>|<span data-ttu-id="ff9e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff9e0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff9e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff9e0-127">Request body</span></span>
<span data-ttu-id="ff9e0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff9e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff9e0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff9e0-129">Response</span></span>

<span data-ttu-id="ff9e0-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff9e0-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff9e0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ff9e0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff9e0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff9e0-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleInstances/5cfd7709-7709-5cfd-0977-fd5c0977fd5c
```


### <a name="response"></a><span data-ttu-id="ff9e0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff9e0-133">Response</span></span>
<span data-ttu-id="ff9e0-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ff9e0-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
    "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
    "startDateTime": "2020-09-09T21:35:27.91Z",
    "endDateTime": "2020-09-09T21:35:27.91Z",
    "memberType": "direct",
    "roleEligibilityScheduleId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c"
  }
}
```

