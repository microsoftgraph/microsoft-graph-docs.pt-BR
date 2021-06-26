---
title: Listar membros da audiência de implantação
description: Listar os recursos updatableAsset que são membros de uma deploymentAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: c3d0ea20730f7d253600e433d96fd0e07e1391f5
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151752"
---
# <a name="list-deployment-audience-members"></a><span data-ttu-id="89e7a-103">Listar membros da audiência de implantação</span><span class="sxs-lookup"><span data-stu-id="89e7a-103">List deployment audience members</span></span>
<span data-ttu-id="89e7a-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="89e7a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89e7a-105">Listar [os recursos updatableAsset](../resources/windowsupdates-updatableasset.md) que são membros de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="89e7a-105">List the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources that are members of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89e7a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="89e7a-106">Permissions</span></span>
<span data-ttu-id="89e7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89e7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89e7a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89e7a-109">Permission type</span></span>|<span data-ttu-id="89e7a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89e7a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89e7a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89e7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89e7a-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e7a-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="89e7a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89e7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89e7a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89e7a-114">Not supported.</span></span>|
|<span data-ttu-id="89e7a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89e7a-115">Application</span></span>|<span data-ttu-id="89e7a-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e7a-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89e7a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89e7a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}/audience/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89e7a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89e7a-118">Optional query parameters</span></span>
<span data-ttu-id="89e7a-119">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="89e7a-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="89e7a-120">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="89e7a-120">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="89e7a-121">Por exemplo, para selecionar [azureADDevice,](../resources/windowsupdates-azureaddevice.md) `errors` use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="89e7a-121">For example, to select [azureADDevice](../resources/windowsupdates-azureaddevice.md) `errors`, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89e7a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7a-122">Request headers</span></span>
|<span data-ttu-id="89e7a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="89e7a-123">Name</span></span>|<span data-ttu-id="89e7a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="89e7a-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="89e7a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="89e7a-125">Authorization</span></span>|<span data-ttu-id="89e7a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89e7a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89e7a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7a-128">Request body</span></span>
<span data-ttu-id="89e7a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89e7a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89e7a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e7a-130">Response</span></span>

<span data-ttu-id="89e7a-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89e7a-131">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89e7a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89e7a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89e7a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89e7a-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="89e7a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="89e7a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/members
```
# <a name="c"></a>[<span data-ttu-id="89e7a-135">C#</span><span class="sxs-lookup"><span data-stu-id="89e7a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89e7a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89e7a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89e7a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89e7a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89e7a-138">Java</span><span class="sxs-lookup"><span data-stu-id="89e7a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="89e7a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="89e7a-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "fb95f07d-9e73-411d-99ab-7eca3a5122b1",
      "errors": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
        }
      ],
      "enrollments": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
        }
      ]
    },
  ]
}
```

