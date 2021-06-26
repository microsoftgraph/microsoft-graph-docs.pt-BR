---
title: Listar updatableAssets
description: Obter uma lista de objetos updatableAsset e suas propriedades.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: a50e24fec7c80b66eaf9ab58027cc2b3cb8814ec
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151549"
---
# <a name="list-updatableassets"></a><span data-ttu-id="64e6f-103">Listar updatableAssets</span><span class="sxs-lookup"><span data-stu-id="64e6f-103">List updatableAssets</span></span>
<span data-ttu-id="64e6f-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="64e6f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e6f-105">Obter uma lista de [objetos updatableAsset](../resources/windowsupdates-updatableasset.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="64e6f-105">Get a list of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects and their properties.</span></span>

<span data-ttu-id="64e6f-106">A listagem de ativos atualizáveis retorna os recursos **updatableAsset** dos seguintes tipos derivados: [azureADDevice](../resources/windowsupdates-azureADDevice.md) e [updatableAssetGroup](../resources/windowsupdates-updatableassetGroup.md).</span><span class="sxs-lookup"><span data-stu-id="64e6f-106">Listing updatable assets returns **updatableAsset** resources of the following derived types: [azureADDevice](../resources/windowsupdates-azureADDevice.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetGroup.md).</span></span>

<span data-ttu-id="64e6f-107">Use [os recursos list azureADDevice](windowsupdates-updates-list-updatableassets-azureaddevice.md) ou list [updatableAssetGroup para](windowsupdates-updates-list-updatableassets-updatableassetgroup.md) filtrar e obter recursos de apenas um dos tipos derivados.</span><span class="sxs-lookup"><span data-stu-id="64e6f-107">Use [list azureADDevice resources](windowsupdates-updates-list-updatableassets-azureaddevice.md) or [list updatableAssetGroup resources](windowsupdates-updates-list-updatableassets-updatableassetgroup.md) to filter and get resources of only one of the derived types.</span></span>

## <a name="permissions"></a><span data-ttu-id="64e6f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="64e6f-108">Permissions</span></span>
<span data-ttu-id="64e6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64e6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64e6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64e6f-111">Permission type</span></span>|<span data-ttu-id="64e6f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64e6f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64e6f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64e6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64e6f-114">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e6f-114">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="64e6f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64e6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64e6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64e6f-116">Not supported.</span></span>|
|<span data-ttu-id="64e6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64e6f-117">Application</span></span>|<span data-ttu-id="64e6f-118">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e6f-118">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64e6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64e6f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64e6f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64e6f-120">Optional query parameters</span></span>
<span data-ttu-id="64e6f-121">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="64e6f-121">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="64e6f-122">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="64e6f-122">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="64e6f-123">Por exemplo, para aplicar `$select` na propriedade **errors** do [azureADDevice,](../resources/windowsupdates-azureaddevice.md)use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="64e6f-123">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64e6f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64e6f-124">Request headers</span></span>
|<span data-ttu-id="64e6f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="64e6f-125">Name</span></span>|<span data-ttu-id="64e6f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="64e6f-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64e6f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="64e6f-127">Authorization</span></span>|<span data-ttu-id="64e6f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64e6f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64e6f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64e6f-130">Request body</span></span>
<span data-ttu-id="64e6f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64e6f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64e6f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="64e6f-132">Response</span></span>

<span data-ttu-id="64e6f-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64e6f-133">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64e6f-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="64e6f-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64e6f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64e6f-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64e6f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="64e6f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets
```
# <a name="c"></a>[<span data-ttu-id="64e6f-137">C#</span><span class="sxs-lookup"><span data-stu-id="64e6f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64e6f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64e6f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64e6f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64e6f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64e6f-140">Java</span><span class="sxs-lookup"><span data-stu-id="64e6f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="64e6f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="64e6f-141">Response</span></span>

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
      "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
      "errors": [],
      "enrollments": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
          "updateCategory": "feature"
        }
      ]
    }
  ]
}
```

