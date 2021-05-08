---
title: Listar membros da audiência de implantação
description: Listar os recursos updatableAsset que são membros de uma deploymentAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 44e9f6f93e060b8ea091c02fa008efd2ff1ade23
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52266896"
---
# <a name="list-deployment-audience-members"></a><span data-ttu-id="a4d6f-103">Listar membros da audiência de implantação</span><span class="sxs-lookup"><span data-stu-id="a4d6f-103">List deployment audience members</span></span>
<span data-ttu-id="a4d6f-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="a4d6f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4d6f-105">Listar [os recursos updatableAsset](../resources/windowsupdates-updatableasset.md) que são membros de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="a4d6f-105">List the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources that are members of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4d6f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4d6f-106">Permissions</span></span>
<span data-ttu-id="a4d6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4d6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4d6f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4d6f-109">Permission type</span></span>|<span data-ttu-id="a4d6f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4d6f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4d6f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4d6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4d6f-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4d6f-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="a4d6f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4d6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4d6f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4d6f-114">Not supported.</span></span>|
|<span data-ttu-id="a4d6f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4d6f-115">Application</span></span>|<span data-ttu-id="a4d6f-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4d6f-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4d6f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4d6f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}/audience/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4d6f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a4d6f-118">Optional query parameters</span></span>
<span data-ttu-id="a4d6f-119">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="a4d6f-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="a4d6f-120">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="a4d6f-120">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="a4d6f-121">Por exemplo, para selecionar [azureADDevice,](../resources/windowsupdates-azureaddevice.md) `errors` use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="a4d6f-121">For example, to select [azureADDevice](../resources/windowsupdates-azureaddevice.md) `errors`, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4d6f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4d6f-122">Request headers</span></span>
|<span data-ttu-id="a4d6f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="a4d6f-123">Name</span></span>|<span data-ttu-id="a4d6f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4d6f-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4d6f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4d6f-125">Authorization</span></span>|<span data-ttu-id="a4d6f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4d6f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4d6f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4d6f-128">Request body</span></span>
<span data-ttu-id="a4d6f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4d6f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4d6f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4d6f-130">Response</span></span>

<span data-ttu-id="a4d6f-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4d6f-131">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4d6f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a4d6f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4d6f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4d6f-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a4d6f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4d6f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/members
```
# <a name="c"></a>[<span data-ttu-id="a4d6f-135">C#</span><span class="sxs-lookup"><span data-stu-id="a4d6f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4d6f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4d6f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4d6f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4d6f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4d6f-138">Java</span><span class="sxs-lookup"><span data-stu-id="a4d6f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a4d6f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4d6f-139">Response</span></span>

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
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
    },
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

