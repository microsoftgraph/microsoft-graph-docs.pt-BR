---
title: Obter unifiedRoleEligibilitySchedule
description: Leia as propriedades e as relações de um objeto unifiedRoleEligibilitySchedule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 22f90942b141cca787ea583debb718b8a05c41d8
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679943"
---
# <a name="get-unifiedroleeligibilityschedule"></a><span data-ttu-id="84396-103">Obter unifiedRoleEligibilitySchedule</span><span class="sxs-lookup"><span data-stu-id="84396-103">Get unifiedRoleEligibilitySchedule</span></span>
<span data-ttu-id="84396-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84396-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84396-105">Leia as propriedades e as relações de [um objeto unifiedRoleEligibilitySchedule.](../resources/unifiedroleeligibilityschedule.md)</span><span class="sxs-lookup"><span data-stu-id="84396-105">Read the properties and relationships of an [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84396-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="84396-106">Permissions</span></span>
<span data-ttu-id="84396-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84396-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84396-109">Permission type</span></span>|<span data-ttu-id="84396-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84396-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84396-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84396-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84396-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="84396-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="84396-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84396-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84396-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="84396-114">Not supported</span></span>|
|<span data-ttu-id="84396-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84396-115">Application</span></span>|<span data-ttu-id="84396-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="84396-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="84396-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84396-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilitySchedules/{unifiedRoleEligibilitySchedulesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84396-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="84396-118">Optional query parameters</span></span>
<span data-ttu-id="84396-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="84396-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="84396-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="84396-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="84396-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84396-121">Request headers</span></span>
|<span data-ttu-id="84396-122">Nome</span><span class="sxs-lookup"><span data-stu-id="84396-122">Name</span></span>|<span data-ttu-id="84396-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="84396-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="84396-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="84396-124">Authorization</span></span>|<span data-ttu-id="84396-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84396-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84396-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84396-127">Request body</span></span>
<span data-ttu-id="84396-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84396-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84396-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="84396-129">Response</span></span>

<span data-ttu-id="84396-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84396-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84396-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="84396-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84396-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84396-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="84396-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="84396-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleeligibilityschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules/5cfd7709-7709-5cfd-0977-fd5c0977fd5c
```
# <a name="c"></a>[<span data-ttu-id="84396-134">C#</span><span class="sxs-lookup"><span data-stu-id="84396-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleeligibilityschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84396-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84396-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleeligibilityschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84396-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84396-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleeligibilityschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84396-137">Java</span><span class="sxs-lookup"><span data-stu-id="84396-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleeligibilityschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="84396-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="84396-138">Response</span></span>
<span data-ttu-id="84396-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="84396-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilitySchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```

