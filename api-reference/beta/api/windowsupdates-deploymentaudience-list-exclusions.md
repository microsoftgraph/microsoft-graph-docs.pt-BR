---
title: Listar exclusões de audiência de implantação
description: Listar os recursos updatableAsset excluídos de uma deploymentAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 2fbe216e4f37df197934611e60478df9dda71387
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351136"
---
# <a name="list-deployment-audience-exclusions"></a><span data-ttu-id="5bfa0-103">Listar exclusões de audiência de implantação</span><span class="sxs-lookup"><span data-stu-id="5bfa0-103">List deployment audience exclusions</span></span>

<span data-ttu-id="5bfa0-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="5bfa0-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bfa0-105">Listar [os recursos updatableAsset](../resources/windowsupdates-updatableasset.md) excluídos de uma [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="5bfa0-105">List the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources that are excluded from a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

> [!NOTE]
> <span data-ttu-id="5bfa0-106">Essa API tem um [problema conhecido relacionado](/Graph/known-issues#accessing-and-updating-deployment-audiences) a implantações criadas por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-106">This API has a [known issue](/Graph/known-issues#accessing-and-updating-deployment-audiences) related to deployments created via Intune.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bfa0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5bfa0-107">Permissions</span></span>
<span data-ttu-id="5bfa0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bfa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bfa0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bfa0-110">Permission type</span></span>|<span data-ttu-id="5bfa0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bfa0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bfa0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bfa0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5bfa0-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bfa0-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="5bfa0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bfa0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bfa0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-115">Not supported.</span></span>|
|<span data-ttu-id="5bfa0-116">Application</span><span class="sxs-lookup"><span data-stu-id="5bfa0-116">Application</span></span>|<span data-ttu-id="5bfa0-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bfa0-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bfa0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bfa0-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}/audience/exclusions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bfa0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5bfa0-119">Optional query parameters</span></span>
<span data-ttu-id="5bfa0-120">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="5bfa0-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="5bfa0-121">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="5bfa0-122">Por exemplo, para selecionar [azureADDevice,](../resources/windowsupdates-azureaddevice.md) `errors` use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="5bfa0-122">For example, to select [azureADDevice](../resources/windowsupdates-azureaddevice.md) `errors`, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="5bfa0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfa0-123">Request headers</span></span>
|<span data-ttu-id="5bfa0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5bfa0-124">Name</span></span>|<span data-ttu-id="5bfa0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bfa0-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5bfa0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bfa0-126">Authorization</span></span>|<span data-ttu-id="5bfa0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bfa0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfa0-129">Request body</span></span>
<span data-ttu-id="5bfa0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bfa0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfa0-131">Response</span></span>

<span data-ttu-id="5bfa0-132">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-132">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5bfa0-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5bfa0-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5bfa0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfa0-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5bfa0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bfa0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/exclusions
```
# <a name="c"></a>[<span data-ttu-id="5bfa0-136">C#</span><span class="sxs-lookup"><span data-stu-id="5bfa0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bfa0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bfa0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bfa0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bfa0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bfa0-139">Java</span><span class="sxs-lookup"><span data-stu-id="5bfa0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5bfa0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfa0-140">Response</span></span>

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

