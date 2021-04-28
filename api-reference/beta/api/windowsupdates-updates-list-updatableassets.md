---
title: Listar updatableAssets
description: Obter uma lista de objetos updatableAsset e suas propriedades.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: e5eebb39af41bd31ee0e2d68404480ea84cd51dc
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067281"
---
# <a name="list-updatableassets"></a><span data-ttu-id="30547-103">Listar updatableAssets</span><span class="sxs-lookup"><span data-stu-id="30547-103">List updatableAssets</span></span>
<span data-ttu-id="30547-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="30547-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30547-105">Obter uma lista de [objetos updatableAsset](../resources/windowsupdates-updatableasset.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="30547-105">Get a list of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects and their properties.</span></span>

<span data-ttu-id="30547-106">A listagem de ativos atualizáveis retorna os recursos **updatableAsset** dos seguintes tipos derivados: [azureADDevice](../resources/windowsupdates-azureADDevice.md) e [updatableAssetGroup](../resources/windowsupdates-updatableassetGroup.md).</span><span class="sxs-lookup"><span data-stu-id="30547-106">Listing updatable assets returns **updatableAsset** resources of the following derived types: [azureADDevice](../resources/windowsupdates-azureADDevice.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetGroup.md).</span></span>

<span data-ttu-id="30547-107">Use [os recursos list azureADDevice](windowsupdates-updates-list-updatableassets-azureaddevice.md) ou list [updatableAssetGroup para](windowsupdates-updates-list-updatableassets-updatableassetgroup.md) filtrar e obter recursos de apenas um dos tipos derivados.</span><span class="sxs-lookup"><span data-stu-id="30547-107">Use [list azureADDevice resources](windowsupdates-updates-list-updatableassets-azureaddevice.md) or [list updatableAssetGroup resources](windowsupdates-updates-list-updatableassets-updatableassetgroup.md) to filter and get resources of only one of the derived types.</span></span>

## <a name="permissions"></a><span data-ttu-id="30547-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="30547-108">Permissions</span></span>
<span data-ttu-id="30547-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30547-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30547-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30547-111">Permission type</span></span>|<span data-ttu-id="30547-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30547-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30547-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30547-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30547-114">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30547-114">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="30547-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30547-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30547-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30547-116">Not supported.</span></span>|
|<span data-ttu-id="30547-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30547-117">Application</span></span>|<span data-ttu-id="30547-118">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30547-118">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30547-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30547-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30547-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30547-120">Optional query parameters</span></span>
<span data-ttu-id="30547-121">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="30547-121">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="30547-122">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="30547-122">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="30547-123">Por exemplo, para aplicar `$select` na propriedade **errors** do [azureADDevice,](../resources/windowsupdates-azureaddevice.md)use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="30547-123">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30547-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30547-124">Request headers</span></span>
|<span data-ttu-id="30547-125">Nome</span><span class="sxs-lookup"><span data-stu-id="30547-125">Name</span></span>|<span data-ttu-id="30547-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="30547-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="30547-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="30547-127">Authorization</span></span>|<span data-ttu-id="30547-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30547-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30547-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30547-130">Request body</span></span>
<span data-ttu-id="30547-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30547-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30547-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="30547-132">Response</span></span>

<span data-ttu-id="30547-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30547-133">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30547-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="30547-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30547-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30547-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets
```


### <a name="response"></a><span data-ttu-id="30547-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="30547-136">Response</span></span>

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
      "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
    },
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

