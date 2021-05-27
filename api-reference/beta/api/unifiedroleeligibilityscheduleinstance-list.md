---
title: Listar unifiedRoleEligibilityScheduleInstances
description: Obter uma lista dos objetos unifiedRoleEligibilityScheduleInstance e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c4662d54547beaa1e4af77c204618b5f5a935e29
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680105"
---
# <a name="list-unifiedroleeligibilityscheduleinstances"></a><span data-ttu-id="f55a6-103">Listar unifiedRoleEligibilityScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="f55a6-103">List unifiedRoleEligibilityScheduleInstances</span></span>
<span data-ttu-id="f55a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f55a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f55a6-105">Obter uma lista dos [objetos unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f55a6-105">Get a list of the [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f55a6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f55a6-106">Permissions</span></span>
<span data-ttu-id="f55a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f55a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f55a6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f55a6-109">Permission type</span></span>|<span data-ttu-id="f55a6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f55a6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f55a6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f55a6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f55a6-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f55a6-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="f55a6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f55a6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f55a6-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f55a6-114">Not supported</span></span>|
|<span data-ttu-id="f55a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f55a6-115">Application</span></span>|<span data-ttu-id="f55a6-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="f55a6-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="f55a6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f55a6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f55a6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f55a6-118">Optional query parameters</span></span>
<span data-ttu-id="f55a6-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f55a6-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f55a6-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f55a6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f55a6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f55a6-121">Request headers</span></span>
|<span data-ttu-id="f55a6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f55a6-122">Name</span></span>|<span data-ttu-id="f55a6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f55a6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f55a6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f55a6-124">Authorization</span></span>|<span data-ttu-id="f55a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f55a6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f55a6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f55a6-127">Request body</span></span>
<span data-ttu-id="f55a6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f55a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f55a6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f55a6-129">Response</span></span>

<span data-ttu-id="f55a6-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f55a6-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f55a6-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f55a6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f55a6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f55a6-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f55a6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f55a6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedroleeligibilityscheduleinstance"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleInstances
```
# <a name="c"></a>[<span data-ttu-id="f55a6-134">C#</span><span class="sxs-lookup"><span data-stu-id="f55a6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedroleeligibilityscheduleinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f55a6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f55a6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedroleeligibilityscheduleinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f55a6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f55a6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedroleeligibilityscheduleinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f55a6-137">Java</span><span class="sxs-lookup"><span data-stu-id="f55a6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedroleeligibilityscheduleinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f55a6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f55a6-138">Response</span></span>
<span data-ttu-id="f55a6-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f55a6-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "principalId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "roleDefinitionId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "directoryScopeId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "appScopeId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1",
      "startDateTime": "2020-09-09T21:35:27.91Z",
      "endDateTime": "2020-09-09T21:35:27.91Z",
      "memberType": "direct",
      "roleEligibilityScheduleId": "d12c1ab0-1ab0-d12c-b01a-2cd1b01a2cd1"
    }
  ]
}
```

